# Creating Your First Form

## Overview

Learn how to effectively create and deploy forms in D365 Customer Insights to capture customer data and manage preferences across your marketing campaigns.

## Step-by-Step Guide

### 1. Access the Form Editor

1. Navigate to Customer Insights - Journeys
2. Go to **Channels > Forms**
3. Click **New** on the command bar

### 2. Configure Basic Settings

- **Name your form**: Choose a descriptive name for internal use
- **Select target audience**: This is important for field mapping (Contacts, Leads, etc.)
- **Set form type**: Standard form, event registration, or landing page form

### 3. Add Form Fields

The form editor uses a drag-and-drop interface:

1. From the **toolbox panel**, drag field elements onto your canvas
2. Click each field to configure:
   - **Field mapping**: Link to the correct entity attribute
   - **Display name**: Set user-friendly labels
   - **Validation rules**: Make fields required or set specific formats
   - **Default values**: Pre-populate where appropriate

### 4. Essential Fields to Include

For marketing forms, typically include:

- First Name and Last Name
- Email Address (always required)
- Company Name
- Phone Number
- Marketing preferences checkboxes

### 5. Add a Submit Button

Every form requires a submit button for validation and submission processing.

### 6. Publish Your Form

1. Click **Publish** in the command bar
2. Copy the form embed code or capture script
3. Add it to your website or landing page

## Next Steps

- Learn about [styling forms](../guides/styling-forms.md)
- Set up [form capture](../guides/form-capture.md) for existing forms
- Create [reusable templates](../how-to/create-form-templates.md)
