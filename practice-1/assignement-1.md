# Assignment 1: B2B Vendor Onboarding & Compliance Portal

## Client Brief

Nexus Logistics Corp. is digitizing its supplier intake process. Currently, prospective freight and warehouse vendors email PDFs and spreadsheets to procurement officers, causing missing data and compliance delays. You have been contracted to build the frontend HTML structure for their Vendor Onboarding Application (`onboarding.html`). When submitted, the form must securely transmit all text data and attached compliance documents to `/api/vendors/register`.

## Functional Requirements

### Accessibility & Semantics

Every visible field must have a properly linked label so clicking the label focuses or toggles the control, and every submittable field must carry a clear, descriptive key name for backend processing.

### Company & Contact Identification

Collect the legal business name (mandatory), a primary account contact's work email (mandatory), a direct dispatch phone number, and the company's public website address.

### Portal Account Setup

Prospective vendors must create a temporary portal passcode (mandatory, masked from shoulder-surfing) during registration.

### Operational Capacity

- Capture the year the company was founded (must be between 1900 and the current year).
- Capture their fleet size (must be at least 1, incrementing in steps of 5).
- Allow the vendor to specify their earliest available contract start date (cannot be in the past).

### Service Classification

- Vendors operate under exactly one primary business structure: Sole Proprietorship, LLC, or Corporation.
- Vendors can select one or more service regions they cover: North America, Europe, Asia-Pacific, or Latin America.
- Provide a compact list to choose their primary equipment tier (Standard Dry Van, Refrigerated / Cold Chain, Flatbed & Heavy Haul, or Hazardous Materials).

### Compliance & Internal Tracking

- Vendors must attach a copy of their active liability insurance certificate.
- Provide a multi-line area for safety certifications, special equipment notes, or fleet details.
- Include a non-visible tracking value (`referral_source` set to `"web_portal_v2"`) that submits automatically with the application.

### Form Controls

Include a primary action to submit the application and a secondary action that clears all user entries back to their initial defaults.
