# Thunderbird Mail Cleaner

**A fast, standalone spam cleanup tool for Mozilla Thunderbird.**

Thunderbird Mail Cleaner is an open-source project designed to detect, filter, quarantine, and remove large volumes of unwanted email across multiple Thunderbird accounts — without relying on Thunderbird's interface for bulk processing.

It aims to make managing years of accumulated email easier, faster, and more efficient, while helping reclaim valuable disk space.

> **Project status: Planning and design**
>
> Thunderbird Mail Cleaner is currently under development and is not yet available for general use. The features described below represent the project's goals.

## Why Thunderbird Mail Cleaner?

Thunderbird is a powerful email client, but managing spam across dozens of accounts and millions of stored messages can be challenging.

Searching, filtering, and deleting massive numbers of messages through a conventional mail client can become slow and resource-intensive.

Thunderbird Mail Cleaner is being designed specifically to solve this problem.

**Keep Thunderbird for email. Use Thunderbird Mail Cleaner for large-scale cleanup.**

## Planned Features

### High-Performance Email Processing

- Scan millions of stored messages efficiently.
- Process multiple Thunderbird accounts in a single operation.
- Analyze email directly from local Thunderbird data.
- Minimize memory consumption through efficient processing.
- Display scan progress and processing statistics.
- Perform incremental scans for ongoing maintenance.

### Advanced Spam Detection

Combine established spam detection technologies with customizable rules.

Planned capabilities include:

- Integration with proven spam detection engines.
- Spam scoring and classification.
- Sender and domain analysis.
- Email header and content inspection.
- Detection of suspicious links and common spam patterns.
- User-defined allowlists and blocklists.
- Clear explanations of spam classification results.

### Powerful Custom Filtering

Create sophisticated filtering rules through an intuitive visual editor.

Each filter group can contain multiple conditions combined with **AND**, while separate groups are combined with **OR**.

Example:

```text
Filter Group 1
  Sender contains "spam@example.com"
  AND
  Subject contains "promotion"

OR

Filter Group 2
  Sender contains "spam@example.com"
  AND
  Body contains "click here"
```

Supported condition types are planned to include:

- Sender and recipient addresses
- Email domains
- Subject and message body
- Email headers
- Attachment filenames
- Message dates and sizes
- Spam scores
- Accounts and folders

Matching options will include exact matches, partial matches, prefixes, suffixes, regular expressions, and exclusions.

### Bulk Cleanup and Quarantine

- Review detected spam before taking action.
- Select messages across multiple accounts.
- Quarantine potentially unwanted messages.
- Bulk-delete confirmed spam.
- Protect legitimate messages through exclusion rules.
- Track cleanup history and recovered disk space.
- Provide recovery options for supported operations.

### POP3 and IMAP Support

The project aims to support both POP3 and IMAP accounts.

For locally stored POP3 messages, cleanup will operate on Thunderbird's local mail data.

For IMAP accounts, server-side synchronization and deletion must be handled correctly to ensure that removed messages do not simply reappear during synchronization.

### Scheduled Maintenance

After the initial cleanup, Thunderbird Mail Cleaner aims to provide ongoing maintenance through:

- Scheduled spam scans
- Incremental processing of newly received messages
- Automatic quarantine based on configurable rules
- Optional automated cleanup
- Processing history and status reporting

### Modern User Interface

A responsive graphical interface is planned, including:

- Dashboard with account and storage statistics
- Unified account overview
- Visual filter rule builder
- Spam review and bulk selection
- Message preview
- Quarantine management
- Cleanup history
- Scheduled maintenance settings
- Light and dark modes

The interface will be designed to remain responsive even when processing millions of messages.

## Target Environment

| Component | Planned support |
|---|---|
| Operating system | macOS |
| Email client | Mozilla Thunderbird |
| Email protocols | POP3 and IMAP |
| Account management | Multiple accounts and profiles |
| Mail volume | Millions of messages |
| Processing | Local-first, standalone |
| Interface | Graphical user interface |

Support for other operating systems may be considered in the future.

## Privacy and Data Safety

Email often contains sensitive personal and business information.

Thunderbird Mail Cleaner will prioritize:

- Local processing whenever practical.
- No unnecessary transmission of email content to external services.
- Protection of existing Thunderbird data.
- Safe handling of bulk deletion operations.
- Clear visibility into what will be deleted.
- Recovery mechanisms where technically feasible.

Data integrity and predictable behavior are fundamental project requirements.

## Development Roadmap

- [ ] Requirements definition and architecture design
- [ ] Thunderbird profile and account discovery
- [ ] High-performance email scanning
- [ ] Spam detection engine integration
- [ ] Custom AND/OR filtering system
- [ ] Graphical dashboard and review interface
- [ ] POP3 local cleanup
- [ ] IMAP-aware quarantine and deletion
- [ ] Bulk cleanup and recovery mechanisms
- [ ] Scheduled and incremental processing
- [ ] Performance testing with millions of messages
- [ ] Public preview release

## Installation

Not yet available.

Installation instructions will be published when the first usable version is released.

## Documentation

Technical documentation, architecture decisions, and implementation plans will be maintained in the `docs/` directory as development progresses.

## Contributing

Contributions, suggestions, and bug reports will be welcome as the project develops.

Contribution guidelines will be published in a future update.

## License

An open-source license will be selected and published before the first public release.

## Disclaimer

Thunderbird Mail Cleaner is an independent, unofficial project.

It is not affiliated with, endorsed by, or sponsored by Mozilla or the Thunderbird project.

Mozilla and Thunderbird are trademarks of their respective owners.
