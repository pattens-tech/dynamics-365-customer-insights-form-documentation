# Troubleshooting Guide

## Quick Diagnostic Checklist

Before diving into specific issues:

- [ ] Is the form published (not Draft)?
- [ ] Is the domain authenticated?
- [ ] Within rate limits (2,000 requests/minute)?
- [ ] Waited 10 minutes for CDN cache?
- [ ] Any errors in browser console (F12)?
- [ ] All required fields mapped?

## Form Not Accepting Submissions

### Possible Causes & Solutions

#### 1. Form Not Published
**Check**: Verify status is "Live" not "Draft"
**Solution**: Click Publish

#### 2. Domain Not Authenticated
**Check**: Settings > Domain Authentication
**Solution**: Add domain, complete DNS verification

#### 3. Rate Limit Exceeded
**Check**: Monitor requests in form insights
**Solution**: Implement client-side throttling

#### 4. Required Fields Missing
**Check**: Browser console for validation errors
**Solution**: Ensure all required fields present

## Data Not Syncing to CRM

### Possible Causes & Solutions

#### 1. Incorrect Field Mapping
**Check**: Field names match D365 attributes exactly

**Solution**: 
```javascript
// Correct
'email': 'emailaddress1'  // ✅

// Incorrect  
'email': 'email'  // ❌
```

#### 2. Data Type Mismatch
**Check**: Source and destination types match
**Solution**: Text to Text, Number to Number, etc.

#### 3. Duplicate Detection Rules
**Check**: Duplicate detection settings
**Solution**: Review and adjust matching criteria

## CORS Errors

### Symptom
"Cross-Origin Request Blocked" in browser console

### Solution

1. Go to **Settings > Domain Authentication**
2. Add your domain
3. Complete DNS verification
4. Allow 24 hours for propagation

## Styling Issues

### CSS Not Applying

**Causes:**
1. Cache not cleared (wait 10 minutes)
2. Inline styles override
3. CSS specificity too low

**Solution**: Use `#d365mkt-nocache` for testing

## Form Capture Problems

### Submissions Not Captured

**Causes:**
1. Feature not enabled
2. Version too old (need 1.1.35355+)
3. Field mapping errors

**Solution**: Enable in Settings > Feature switches > Forms

## Getting Help

### Browser Console
Press F12 > Console tab > Look for red errors

### Contact Support
Provide: Form URL, browser version, console logs, steps to reproduce
