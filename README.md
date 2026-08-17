Example Change Detection

The system can detect a change such as:

Previous Version
Acme Widget
USD 99.00 / month
Version 4.8.2
Release Date: August 12, 2026
Monitoring Frequency: Every 5 minutes
Current Version
Acme Widget
USD 79.00 / month
Version 4.9.0
Release Date: August 17, 2026
Monitoring Frequency: Every 2 minutes
Detected Changes
Field	Previous	Current
Price	USD 99.00	USD 79.00
Version	4.8.2	4.9.0
Release Date	August 12, 2026	August 17, 2026
Monitoring Frequency	Every 5 minutes	Every 2 minutes
Customer Feedback

"Acme Widget helped our team catch important website changes without manually checking dozens of pages."

Sarah Mitchell
Product Manager, Northstar Labs

"The visual comparison feature is particularly useful when monitoring competitor landing pages."

Daniel Carter
Growth Lead, BrightWorks

Frequently Asked Questions
How frequently can pages be monitored?

Professional accounts can monitor supported pages as frequently as every five minutes.

Enterprise accounts can use custom monitoring intervals.

Does the system detect visual changes?

Yes.

The platform can capture screenshots and compare the previous version with the current version to identify visual differences.

Can I monitor a specific element on a page?

Yes.

CSS selectors, XPath selectors, and other extraction strategies can be used to monitor specific sections of a webpage.

Is an API available?

Yes.

Professional and Enterprise plans include REST API access for integrating monitoring results with external applications.

Can I export historical changes?

Yes.

Historical results can be exported in:

CSV
JSON
PDF

depending on the selected plan.

Example Monitoring Workflow
                    ┌─────────────────────┐
                    │      Target URL     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Fetch Web Page   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Content Extraction  │
                    └──────────┬──────────┘
                               │
                    ┌──────────┴──────────┐
                    ▼                     ▼
             ┌─────────────┐      ┌──────────────┐
             │ Text / DOM  │      │  Screenshot  │
             │ Comparison  │      │  Comparison  │
             └──────┬──────┘      └───────┬──────┘
                    │                     │
                    └──────────┬──────────┘
                               ▼
                    ┌─────────────────────┐
                    │   Change Detected?  │
                    └──────────┬──────────┘
                               │
                         ┌─────┴─────┐
                         │           │
                        YES          NO
                         │           │
                         ▼           ▼
                  ┌────────────┐   Continue
                  │ Send Alert │   Monitoring
                  └────────────┘
Example API Response
{
  "url": "https://example.com/product",
  "status": "changed",
  "detected_at": "2026-08-17T07:30:00Z",
  "changes": [
    {
      "field": "price",
      "previous": "99.00",
      "current": "79.00"
    },
    {
      "field": "version",
      "previous": "4.8.2",
      "current": "4.9.0"
    },
    {
      "field": "monitoring_frequency",
      "previous": "Every 5 minutes",
      "current": "Every 2 minutes"
    }
  ]
}
Latest Product Update

Version: 4.9.0

Release Date: August 17, 2026

What's New
Reduced monitoring interval from 5 minutes to 2 minutes
Improved visual comparison
Improved HTML content extraction
Added advanced price monitoring
Improved API performance
Added additional notification options
Start Monitoring

Track:

Website content
Product prices
Competitor pages
Product availability
Landing pages
Documentation
News pages
HTML changes
Visual changes
Page structure changes

Acme Widget — Monitor what matters.

License

© 2026 Acme Widget. All rights reserved.

This page is a demonstration fixture created for testing:

Web crawling
Content extraction
DOM comparison
Text diff
Semantic diff
Visual comparison
Screenshot comparison
Price monitoring
Change detection
