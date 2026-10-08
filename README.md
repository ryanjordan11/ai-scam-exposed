# AI Scam Exposed

**They make the claims. You bring the receipts.**

Website: https://aiscamexposed.xyz

AI Scam Exposed is an independent public record documenting AI failures, hallucinations, coding disasters, broken promises, agent drift, unauthorized changes, wasted time, and the gap between what AI systems claim to do and what they actually deliver.

Anonymous reporting. Real experiences. Evidence over promises.

No account. No email. No hiding behind marketing.


<img width="3360" height="2100" alt="aiscam" src="https://github.com/user-attachments/assets/ebc63b24-69f9-4019-9689-bba58511497e" />

---

## Table of Contents

* [Mission](#mission)
* [Why This Exists](#why-this-exists)
* [Core Principles](#core-principles)
* [Features](#features)
* [Anonymous Reporting](#anonymous-reporting)
* [Evidence and Verification](#evidence-and-verification)
* [Hallucination File](#hallucination-file)
* [Drift File](#drift-file)
* [Benchmark Record](#benchmark-record)
* [Anonymous Voting](#anonymous-voting)
* [Company-by-Company Records](#company-by-company-records)
* [Privacy and Security](#privacy-and-security)
* [Moderation](#moderation)
* [Technical Architecture](#technical-architecture)
* [Data Model](#data-model)
* [Development Setup](#development-setup)
* [Production Requirements](#production-requirements)
* [Testing](#testing)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [Legal and Editorial Standards](#legal-and-editorial-standards)
* [License](#license)

## Mission

AI companies make ambitious claims about intelligence, autonomy, reliability, productivity, and the ability of AI agents to perform complex work.

But what happens when an agent claims it created a file that does not exist?

What happens when it says it checked a source it never accessed, changes working code without permission, breaks a development environment, invents evidence, forgets the original objective, or sends a user into hours of unnecessary troubleshooting?

What happens when the user asks for proof?

AI Scam Exposed exists to document these experiences.

The project aims to build a searchable public record that compares AI claims with reported outcomes, preserves supporting evidence, and identifies recurring failure patterns.

The goal is not to declare every AI product fraudulent. It is to make specific claims, documented incidents, and verifiable results open to scrutiny.

**The central question: What did the AI claim, and what actually happened?**

## Why This Exists

AI agents are increasingly marketed as autonomous developers, research assistants, productivity systems, and intelligent collaborators.

Users can nevertheless encounter failures such as:

* Claiming a task is complete when the requested result is missing.
* Reporting that a command ran without verifiable execution evidence.
* Inventing screenshots, citations, test results, or file contents.
* Repeatedly changing implementation plans instead of completing the original task.
* Modifying unrelated files or damaging existing functionality.
* Installing conflicting packages or changing project configurations without appropriate authorization.
* Ignoring explicit instructions and constraints.
* Recommending destructive recovery steps without establishing the cause of a problem.
* Blaming the user or environment before investigating the failure.
* Generating large amounts of activity without meaningful progress.
* Requiring users to spend hours repairing the work the agent was supposed to perform.

These failures can cost users time, money, working code, and trust.

Individual incidents may look isolated. A public record makes it possible to investigate whether similar failures recur across products, models, providers, and environments.

## Core Principles

### 1. Anonymous by default

People should be able to report their experiences without creating an account or publishing their identity.

### 2. Evidence over promises

A claim that an action succeeded is not proof that it succeeded.

Reports should include screenshots, logs, source files, diffs, command output, or reproducible steps when available.

### 3. Reports are not automatically facts

A firsthand report establishes that someone has made an allegation. It does not independently establish every detail of that allegation.

The site must distinguish user-submitted reports from findings that have been independently verified.

### 4. Transparency over marketing

Benchmarks must identify their sources and testing conditions. Company claims must be distinguishable from independent results.

### 5. Accountability without fabrication

Criticism should be direct, specific, and supported by available evidence. Fabricated receipts, manipulated evidence, and knowingly false submissions undermine the entire project.

### 6. Users own the consequences

AI systems should be evaluated not only on their outputs but also on the work users must perform to verify, correct, or recover from those outputs.

### 7. Privacy is a technical requirement

Anonymity must be supported by the actual implementation, not merely promised in website copy.

## Features

The project is organized around six primary areas.

### Public reporting desk

A public submission form for documenting incidents involving AI agents, models, providers, and related products.

### Hallucination File

A collection of incidents involving fabricated information, unsupported claims, false completion statements, and claims of verification without reliable evidence.

### Drift File

A collection of incidents involving abandoned objectives, repeated rewrites, ignored instructions, unauthorized scope changes, and activity without meaningful progress.

### Benchmark Record

A sourced collection of published evaluations and reproducible tests, with the methodology and configuration documented.

### Anonymous voting

Public polls allowing users to select multiple options, withdraw their selections, and suggest additional models.

### Company-by-company records

Individual records organized by product, model, agent, or provider, linking reported incidents to their available evidence and verification status.

## Anonymous Reporting

The reporting form should be simple enough to complete in under a minute.

### Report fields

* Headline: a short description of the incident.
* Agent: an existing agent or a user-entered name.
* Model: the model involved, if known.
* Provider: the company or service responsible, if known.
* Report: a description of what happened.
* Evidence: an optional screenshot or other supported attachment.

The report should encourage users to explain three things:

1. What did the AI claim it did?
2. What actually happened?
3. What evidence supports the account?

### Submission requirements

* No account required.
* No email required.
* No public identity required.
* Evidence optional for initial submission.
* Clear indication of the report's verification status.
* Accessible form validation and understandable error messages.
* A confirmation that accurately reflects whether the report was actually saved.

Reports should not be described as published if the server has not confirmed successful persistence.

The prototype must not pretend that browser-local data is a permanent public record.

## Evidence and Verification

Evidence is central to the project's credibility.

### Supported evidence

Depending on the incident, useful evidence may include:

* Screenshots of the original interaction.
* Relevant conversation excerpts.
* Terminal output and execution logs.
* Git diffs showing code changes.
* File listings or timestamps.
* Test results.
* Error messages and stack traces.
* Billing records with sensitive details removed.
* Reproduction steps.
* Links to official documentation or published benchmarks.

### Verification statuses

**Unverified**

The report has been submitted but has not been independently established.

**Evidence supplied**

The submitter has attached material supporting the account. The material has not necessarily been independently authenticated.

**Under review**

The report is undergoing additional examination.

**Independently verified**

A documented review has established the specific finding represented by this label.

**Disputed**

Material disagreement exists about the account or its interpretation. The reason for the dispute should be documented when appropriate.

**Rejected or removed**

The submission does not meet the publication standards, contains prohibited material, or has been removed following review.

Verification should apply to specific findings, not automatically to every statement in a report.

A screenshot can support a claim without proving every part of the story. A test result can establish behavior under specific conditions without proving that the same behavior occurs universally.

### Evidence handling

Uploaded evidence should be stored securely, validated, and reviewed for exposed secrets or private information.

The site should warn users to remove:

* API keys and access tokens.
* Passwords and authentication cookies.
* Private messages and personal information.
* Confidential customer data.
* Proprietary code they are not authorized to publish.
* Sensitive billing or account information.

Original evidence should not be silently altered. Any redacted public copy should be distinguishable from the original, with the reason for redaction recorded where appropriate.

## Hallucination File

This section documents incidents in which an AI system produces unsupported or fabricated information.

### Pattern 01: "I did it."

The agent describes an action as complete, but the result cannot be found or verified.

Examples:

* Claims a file was created when it is missing.
* Claims code was changed without a corresponding diff.
* Claims tests passed without producing test output.
* Claims a deployment succeeded without a deployment record.

### Pattern 02: "I checked."

The agent claims to have inspected a file, source, application, or result without producing reliable evidence of that inspection.

Examples:

* Citing an unrelated file.
* Claiming to have accessed a resource it could not access.
* Presenting a guess as an observed result.
* Confusing instructions for running a check with evidence that the check ran.

### Pattern 03: The invented receipt

The agent supplies evidence that does not establish the claimed event.

Examples:

* Screenshots from an unrelated source.
* Results from a different project.
* Unsupported claims about API usage or costs.
* Fabricated citations or test output.

Each report should identify the actual discrepancy and include the available supporting material.

## Drift File

This section documents failures to preserve the original objective, constraints, or requested scope.

### Pattern 04: Motion without progress

The agent produces plans, code, downloads, and explanations while leaving the original task unfinished.

### Pattern 05: The reset escape

The agent recommends restarting, reinstalling, deleting, or rebuilding without adequate diagnosis.

### Pattern 06: Scope expansion

The agent changes requirements, adds unrelated functionality, or modifies areas outside the agreed task.

### Pattern 07: The working-code casualty

An attempted fix introduces regressions or destroys existing behavior.

### Pattern 08: The repeated promise

The agent repeatedly claims it understands or will complete the task, but does not produce the requested result.

These patterns should be backed by incident reports, reproducible examples, or other evidence whenever possible.

## Benchmark Record

Published benchmarks and independently conducted tests should be documented separately from user-submitted incidents.

Each benchmark entry should identify:

* Benchmark name and source.
* Publication date and version.
* Model and provider.
* Agent framework and configuration, where applicable.
* Test environment and dependencies.
* Prompt or task definition.
* Number of trials.
* Success and failure criteria.
* Scoring method.
* Results and relevant uncertainty.
* Known limitations.
* Links to source data or reproduction instructions.

### Methodological rules

A benchmark score is not proof that every real-world task succeeds.

A user report is not automatically a benchmark result.

A successful demonstration is not proof of general reliability.

A failed test is evidence of a failure under the tested conditions; broader conclusions require additional evidence.

The project should not publish invented scores or imply that a model was tested when no test was performed.

## Anonymous Voting

The voting system allows visitors to share their experiences without creating an account.

### Voting categories

**Worst agent**

Which coding or research agent has caused the most cleanup in your experience?

**Worst provider**

Which provider has the largest gap between its claims and your observed results?

**Worst model**

Which model has been least reliable for your actual tasks?

Additional polls may cover:

* False completion claims.
* Hallucinations.
* Unauthorized code changes.
* Context loss.
* Recovery failures.
* Time wasted on unsuccessful tasks.
* Cost overruns.
* Reproducible benchmark results.

### Voting behavior

* Users may select multiple options.
* Selecting an option again removes that selection.
* Users may suggest additional models.
* Users may remove their own suggestions when supported by the implementation.
* Poll totals should be derived from stored vote records.
* The interface should distinguish total votes from unique voters.
* Votes must not be presented as independent people unless the counting method establishes that distinction.

### Abuse prevention

Anonymous voting creates risks of automated submissions and repeated voting.

The production system should implement proportionate rate limiting, input validation, abuse monitoring, and transparent counting rules.

If the system cannot reliably prevent repeat voting, it should disclose that limitation rather than claim one-person-one-vote results.

## Company-by-Company Records

The site can organize incidents by company, provider, agent, and model.

Initial directory candidates include:

* Claude and Anthropic.
* OpenAI and its products.
* StepFun and its products.
* Cohere and its products.
* OpenCode.
* Kilo.

These are directory candidates, not declarations that every listed organization or product has committed misconduct.

Each record should contain:

* Product or company name.
* Product category.
* Reported incidents.
* Evidence links.
* Verification statuses.
* Relevant official claims and their sources.
* Published benchmark results.
* Known limitations and corrections.
* Last-updated timestamp.

Company responses may be included where available and relevant.

The directory should make it possible to compare incidents without treating the number of submissions alone as a reliable failure rate.

## Privacy and Security

Anonymous reporting is a core product requirement.

### Data minimization

The application should not require names, email addresses, or account profiles for ordinary reporting and voting.

Avoid collecting unnecessary personal data.

Do not embed personal identifiers in public report URLs or expose internal database identifiers unnecessarily.

### Important distinction

Not requiring a name or email does not automatically make a system fully anonymous.

Hosting providers, infrastructure services, security systems, and other components may process IP addresses or technical metadata.

The privacy policy must accurately describe what is collected, by whom, why it is processed, and how long it is retained.

### Required safeguards

* HTTPS in production.
* Server-side validation.
* Safe file-upload handling.
* Restricted file types and file sizes.
* Malware scanning where appropriate.
* Protection against cross-site scripting and injection.
* Rate limiting and abuse prevention.
* Secure database access controls.
* Secrets stored outside source control.
* Defined retention and deletion policies.
* Restricted access to original evidence.
* Backups and tested restoration procedures.
* A documented incident-response process.

The project must not promise that no identifying information is collected unless the actual architecture and infrastructure support that promise.

## Moderation

The site should permit criticism while limiting abuse and unsupported harmful claims.

Prohibited material should include:

* Threats and targeted harassment.
* Doxxing or publication of private personal information.
* Stolen credentials and authentication secrets.
* Malware and harmful executable uploads.
* Knowingly fabricated evidence.
* Impersonation intended to mislead readers.
* Illegal material.
* Content the submitter has no right to disclose.

Moderation decisions should follow published standards.

Where feasible, the project should provide a correction or appeal process and retain an internal record of significant editorial decisions.

Criticism of a company or product should not automatically be removed merely because it is negative.

## Technical Architecture

The implementation should separate the user interface, persistence, evidence storage, and moderation.

### Frontend

Responsible for:

* Landing page and navigation.
* Reporting forms.
* Evidence previews.
* Public report listings.
* Verification badges.
* Voting interfaces.
* Company records.
* Benchmark tables.
* Responsive layouts and accessibility.

### Backend API

Responsible for:

* Creating and retrieving reports.
* Validating submissions.
* Managing evidence metadata.
* Persisting votes and model suggestions.
* Enforcing moderation rules.
* Applying rate limits.
* Returning accurate publication status.
* Supporting corrections and deletion requests.

### Database

Responsible for durable storage of reports, vote records, evidence metadata, benchmark entries, moderation actions, and configuration.

### Evidence storage

Responsible for securely storing uploaded files, validating them, controlling access, and applying retention policies.

### Deployment

The application should support separate development, staging, and production environments.

The exact framework, database, storage service, and hosting platform must be documented according to the actual repository. No particular implementation should be described as present until it has been confirmed.

## Data Model

The following is a conceptual data model. It is not a claim that these tables already exist.

### Reports

Suggested fields:

* `id`
* `headline`
* `agent_name`
* `model_name`
* `provider_name`
* `report_text`
* `verification_status`
* `submitted_at`
* `updated_at`
* `published_at`
* `moderation_status`

### Evidence

Suggested fields:

* `id`
* `report_id`
* `storage_key`
* `original_filename`
* `media_type`
* `file_size`
* `uploaded_at`
* `review_status`
* `redaction_status`

Sensitive storage keys and internal metadata should not be exposed through public API responses.

### Votes

Suggested fields:

* `id`
* `poll_id`
* `option_id`
* `voter_token`
* `created_at`

The voter token should be designed to minimize identifiability. Its security properties and limitations must be documented.

### Poll options

Suggested fields:

* `id`
* `poll_id`
* `label`
* `created_at`
* `status`

### Benchmarks

Suggested fields:

* `id`
* `name`
* `source_url`
* `version`
* `publication_date`
* `model_configuration`
* `test_conditions`
* `results`
* `limitations`
* `created_at`

### Moderation records

Suggested fields:

* `id`
* `report_id`
* `action`
* `reason`
* `created_at`

Access to moderation records should be restricted appropriately.

## Development Setup

The following instructions are a general starting point. Adapt them to the actual project structure and package manager.

### Prerequisites

* Git.
* Node.js, if the application uses Node.js.
* The package manager required by the repository.
* Access to the required development database and storage services, if applicable.

### Clone the repository

```bash
git clone <repository-url>
cd <repository-directory>
```

### Install dependencies

Use the command appropriate to the repository:

```bash
npm install
```

Or, if the project uses pnpm:

```bash
pnpm install
```

### Configure environment variables

Create the appropriate local environment file using the project's documented template.

Typical configuration may include:

```dotenv
NODE_ENV=development
DATABASE_URL=
UPLOAD_STORAGE_URL=
UPLOAD_STORAGE_KEY=
```

These are illustrative variable names, not verified requirements. Use the names expected by the actual application.

Never commit production credentials, private keys, API tokens, or populated secrets files.

### Start the development server

For a project configured with an npm development script:

```bash
npm run dev
```

For a pnpm project:

```bash
pnpm dev
```

Use the script defined in `package.json`. Do not assume that the server starts successfully without checking its output.

## Production Requirements

Before opening the site to the public, confirm the following.

### Persistence

* Reports survive browser refreshes and server restarts.
* Votes are stored durably.
* Attachments remain accessible according to the retention policy.
* Database backups are configured and tested.

### Anonymous operation

* Report submission works without an account.
* Voting works without requiring registration.
* No hidden name or email requirement exists.
* The privacy policy matches actual infrastructure behavior.
* Rate limiting does not depend on publishing users' identities.

### Evidence integrity

* File types and sizes are validated.
* Uploaded files cannot execute as server code.
* Private attachments are not unintentionally public.
* Verification statuses cannot be self-assigned by ordinary submitters.
* Published evidence can be reviewed and corrected appropriately.

### Public record

* Reports have stable URLs.
* Verification labels are clear.
* Search and filtering operate on stored records.
* Moderation and correction mechanisms are available.
* Voting totals reflect persisted data.
* The site does not fabricate reports, benchmark results, or user counts.

### Reliability

* Errors are logged without unnecessarily exposing sensitive data.
* Monitoring and backups are in place.
* Database migrations are controlled.
* Deployment can be rolled back.
* Recovery procedures have been tested.

## Testing

Testing should verify both normal behavior and failure conditions.

### Reporting tests

* A valid report can be submitted anonymously.
* Missing required fields produce useful errors.
* Oversized or invalid attachments are rejected.
* A failed database write does not produce a false success message.
* Reports remain available after refresh.
* Moderation changes the public visibility of a report appropriately.

### Voting tests

* A visitor can select multiple options.
* A selection can be removed.
* Totals update correctly.
* Invalid options are rejected.
* Automated submissions are rate-limited.
* The displayed counts match stored records.

### Security tests

* Input validation prevents injection.
* User-submitted content cannot execute arbitrary scripts.
* Uploads cannot expose server files.
* Secrets do not appear in logs or public responses.
* Private evidence remains access-controlled.
* Authorization protects administrative actions.

### Integrity tests

* A submitted report starts with the correct verification status.
* Submitters cannot mark their own reports independently verified.
* Benchmark results include source and methodology metadata.
* The site distinguishes report counts from unique users.
* Empty or unavailable data is not replaced with invented values.

### Regression tests

Every fix should be tested against the existing application so that improvements do not silently break working features.

## Accessibility and User Experience

AI Scam Exposed should be usable by people with different devices, abilities, and levels of technical experience.

Requirements include:

* Responsive layouts.
* Keyboard-accessible controls.
* Clearly labeled form fields.
* Visible focus states.
* Readable contrast.
* Accessible status messages.
* Understandable error handling.
* Appropriate image descriptions.
* Reduced-motion support for animations.
* No reliance on color alone to communicate verification status.

Animations may help communicate the site's personality, but they must not interfere with reading, reporting, or navigating the public record.

## Roadmap

### Phase 1: Public prototype

* Landing page.
* Hallucination and drift sections.
* Reporting form.
* Evidence attachment preview.
* Benchmark section.
* Anonymous voting interface.
* Company and model directories.
* Responsive design.

### Phase 2: Functional public record

* Durable report storage.
* Persistent voting.
* Stable report URLs.
* Server-side validation.
* Evidence storage.
* Basic search and filtering.
* Abuse prevention.
* Privacy policy.
* Reporting and correction procedures.

### Phase 3: Verification and transparency

* Evidence review workflow.
* Verification status history.
* Moderation tools.
* Benchmark source records.
* Reproducible test documentation.
* Company response records.
* Public corrections and audit history.

### Phase 4: Research and analysis

* Cross-product failure categorization.
* Searchable incident archives.
* Aggregated failure-pattern reports.
* Benchmark comparisons with documented conditions.
* Time-series analysis where sufficient data exists.
* Public methodology documentation.

### Phase 5: Community participation

* Community-submitted benchmarks.
* Reproducibility contributions.
* Public source and evidence references.
* Expanded product directories.
* Community moderation under published rules.

Roadmap items represent planned work until implemented and verified.

## Contributing

Contributions are welcome from developers, researchers, AI users, testers, and anyone interested in documenting AI reliability.

Useful contributions include:

* Reproducible failure cases.
* Corrections to existing reports.
* Reliable benchmark sources.
* Testing tools and test cases.
* Security improvements.
* Accessibility improvements.
* Documentation.
* Privacy and moderation improvements.

### Contribution standards

Contributors should:

1. Describe the change or incident clearly.
2. Include reproduction steps where possible.
3. Separate observed behavior from interpretation.
4. Cite external sources for factual claims.
5. Avoid publishing confidential information.
6. Test code changes.
7. Disclose relevant limitations.

Do not submit fabricated reports, fabricated benchmark scores, or evidence presented in a misleading context.

## Legal and Editorial Standards

AI Scam Exposed is intended to support public-interest documentation and discussion of AI products and services.

The terms "scam," "fraud," and "dishonest" can imply different things depending on context. Their use must not automatically be treated as a proven legal finding.

The website should distinguish opinion, firsthand experience, independently verified behavior, and legally established misconduct.

Reports should focus on specific, supportable incidents. The site should provide an appropriate process for correcting factual errors and responding to substantiated complaints.

Before public launch, the operator should establish suitable terms of use, a privacy policy, an evidence-retention policy, and procedures for legal complaints and removal requests.

Nothing in this README constitutes legal advice.

## Project Status

**Project:** AI Scam Exposed

**Domain:** aiscamexposed.xyz

**Purpose:** Public documentation of AI failures and the gap between claimed and observed behavior.

**Participation:** Anonymous reporting and voting are core design goals.

**Evidence standard:** Reports are user submissions unless independently verified.

**Implementation status:** Must be determined from the current repository and deployment. A prototype should not be represented as a fully operational public reporting platform until persistence, security, anonymity claims, and voting behavior have been tested.

## License

The license has not yet been specified.

Before selecting one, decide how the source code, submitted reports, evidence, and third-party materials should be licensed or otherwise governed. These are separate questions and should not automatically share the same terms.

---

## Final Principle

AI systems are often judged by what they say they can do.

AI Scam Exposed asks what happened when people actually used them.

A claim is not a result.

A confident answer is not proof.

A plan is not execution.

A screenshot is not automatically verification.

And an agent saying "done" does not make the job done.

**AI SCAM EXPOSED**

**They make the claims. You bring the receipts.**
