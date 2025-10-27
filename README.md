# Dynamics 365 Customer Insights Forms Documentation

Comprehensive documentation for creating, customizing, and managing forms in Dynamics 365 Customer Insights - Journeys.

## 📚 Table of Contents

- [Getting Started](#getting-started)
- [Guides](#guides)
- [How-To Articles](#how-to-articles)
- [Reference](#reference)
- [Quick Links](#quick-links)

---

## 🚀 Getting Started

New to D365 forms? Start here:

- **[Overview](getting-started/overview.md)** - Understanding forms, security, and best practices
- **[Creating Your First Form](getting-started/creating-your-first-form.md)** - Step-by-step tutorial for beginners

---

## 📖 Guides

Detailed guides for working with forms:

- **[Editing Forms](guides/editing-forms.md)** - Edit, unpublish, and manage duplicate records
- **[Styling Forms](guides/styling-forms.md)** - Themes, CSS, and visual customization
- **[Advanced Customization](guides/advanced-customization.md)** - JavaScript, events, and the HTML editor
- **[Form Capture](guides/form-capture.md)** - Integrate existing external forms with D365

---

## 🛠️ How-To Articles

Task-focused solutions for specific scenarios:

- **[Customize Submission Images](how-to/customize-submission-images.md)** - Change or hide the confirmation checkmark
- **[Create Form Templates](how-to/create-form-templates.md)** - Build reusable form templates

---

## 📋 Reference

Quick reference and troubleshooting:

- **[FAQ](reference/faq.md)** - Frequently asked questions
- **[Troubleshooting](reference/troubleshooting.md)** - Common issues and solutions
- **[Technical Reference](reference/technical-reference.md)** - Form structure, elements, and implementation details

---

## 🔗 Quick Links

### Common Tasks

| Task | Guide |
|------|-------|
| Create a new form | [Creating Your First Form](getting-started/creating-your-first-form.md) |
| Change form colors and fonts | [Styling Forms](guides/styling-forms.md) |
| Add custom JavaScript | [Advanced Customization](guides/advanced-customization.md) |
| Connect existing form to D365 | [Form Capture](guides/form-capture.md) |
| Fix submission issues | [Troubleshooting](reference/troubleshooting.md) |
| Create reusable templates | [Create Form Templates](how-to/create-form-templates.md) |
| Understand form structure | [Technical Reference](reference/technical-reference.md) |

### Key Concepts

- **Form Capture**: Integrate external forms without rebuilding them in D365
- **CDN Caching**: Forms are cached globally; changes take up to 10 minutes
- **Domain Authentication**: Required for forms to work on your domain
- **Rate Limiting**: 2,000 requests/minute per organization

---

## 🔒 Security Features

D365 Forms include:
- ✅ Approved domains only
- ✅ Bot protection (CAPTCHA)
- ✅ Traffic control (rate limiting)
- ✅ Data encryption in transit
- ✅ No cookies used for tracking

---

## 🎯 Best Practices

### Performance
- Keep forms short (5-7 fields maximum)
- Use conditional logic to show/hide fields
- Enable progressive profiling
- Minimize required fields

### Compliance
- Include clear consent checkboxes
- Link to privacy policies
- Use preference centers for opt-out management
- Maintain audit trails of consent

### Data Quality
- Use dropdown lists for standardized data
- Implement proper validation patterns
- Set clear error messages
- Use placeholder text for guidance

---

## 📞 Support

- **Official Docs**: https://docs.microsoft.com/dynamics365/marketing
- **Community Forum**: https://community.dynamics.com
- **Microsoft Learn**: Free training courses

---

## 📄 Version

**Documentation Version**: 1.0.0  
**Last Updated**: October 2025  
**D365 Version Compatibility**: Customer Insights - Journeys (all versions)
