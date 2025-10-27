# Frequently Asked Questions (FAQ)

## General Questions

### What is form capture?

Form capture lets you capture submissions from existing forms and map them to Dynamics 365 without using the native form editor.

### When should I use Form Capture vs. native forms?

**Use Form Capture when:**
- Your form sends data to multiple systems
- Your form has complex custom logic
- You want to keep your existing form design

**Use Native Forms when:**
- Starting fresh with D365
- You want full integration with Customer Insights
- You need built-in analytics

### Do D365 Forms use cookies?

No. Marketing and event registration forms don't use cookies. Form interactions use a journey-id to identify known users.

### How secure are Forms in Dynamics 365?

D365 Forms include:
- Approved domains only
- Bot protection (CAPTCHA)
- Traffic control (2,000 requests/minute)
- Data encryption in transit

## Publishing & Caching

### Why aren't my form changes showing up?

Forms are cached on a CDN. Changes take up to 10 minutes to propagate.

**Quick testing**: Append `#d365mkt-nocache` to your form URL (don't share publicly).

### How do I unpublish a form?

1. Open the form
2. Click **Stop**
3. Status changes to **Draft**

## Technical Issues

### Why is my form not accepting submissions?

Check:
1. Domain authentication
2. Form is published
3. Rate limiting (2,000 requests/minute)
4. Required fields are mapped
5. No CORS errors in console

### Why is my data not syncing to CRM?

Common causes:
1. Field mapping errors
2. Entity permissions
3. Duplicate detection rules
4. Data type mismatches

### Why am I getting CORS errors?

Your domain isn't enabled for external form hosting.

**Solution**: Go to **Settings > Domain Authentication** and add your domain.

### How do I enable Form Capture?

1. **Settings > Feature switches**
2. Navigate to **Forms**
3. Toggle on **Form capture**
4. Requires version 1.1.35355+

## Styling & Customization

### Why won't my custom CSS apply?

Common issues:
1. Inline styles override theme
2. Cache (wait 10 minutes)
3. CSS specificity too low
4. Syntax errors

### Can I use JavaScript in forms?

Yes! Add custom JavaScript in the HTML editor. Use `addEventListener` instead of inline event attributes.

### How do I hide the submission checkmark?

```css
div[data-cached-form-url] .onFormSubmittedFeedbackIcon {
  display: none;
}
```

See [Customize Submission Images](../how-to/customize-submission-images.md)

## Performance & Limits

### What are the form submission rate limits?

- 2,000 requests per minute per organization
- Translates to 100-500 valid submissions per minute

### How many fields should a form have?

**Best practice**: 5-7 fields maximum for optimal completion rates.

## Related Resources

- [Troubleshooting Guide](troubleshooting.md)
- [Form Capture Setup](../guides/form-capture.md)
- [Advanced Customization](../guides/advanced-customization.md)
