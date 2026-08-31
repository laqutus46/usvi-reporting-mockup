# USVI SPFx Outcome Reporting Concept

This package is a standalone, interactive demonstration of the proposed USVI reporting experience. It separates detailed project reporting from outcome-based functional-support reporting.

## What the demonstration includes

- **Weekly Project Report** with four guided sections:
  1. Project and status
  2. Results and outcomes
  3. Risks and decisions
  4. Outlook and submission
- PM reporting modes for one project, several selected projects, or a centrally maintained saved project bundle.
- Bundle membership is displayed automatically, while ad hoc multi-project reports support removable project tags.
- **Functional Work & Outcomes** for Program Controls, Supply Chain, Quality, Grants, Document Control, Commercial, GIS/Environmental, Resource Management, Administration, and other support functions.
- Per-work-item affected-scope selection for All 54 projects, Healthcare, Infrastructure, PMO, Education, or one or more individual projects.
- Compact multi-select project and sector tags within every work item; production SPFx would search all 54 records from the Master Project List.
- Direct-submission functional work records with no functional-lead approval step.
- A plain-language choice between “I completed or supported work” and “The work produced a material result or change,” with examples and guidance for users who are unsure.
- Work performed, reason/request, work product, supporting record, direction received, follow-up, outcome, impact, evidence, commitments, dependencies, and leadership-support fields.
- Repeatable work items so one weekly functional submission can contain multiple work categories, project-specific issues, and distinct pieces of work while reusing only the function, period, and submitter.
- No meeting-attendance or meeting-count reporting.
- Healthcare-sector demonstration data.
- Two working top-level tabs, conditional outcome fields, direct functional submission, and sample submission histories.

## Publish with GitHub Pages

1. Create a new GitHub repository, for example `usvi-outcome-reporting-concept`.
2. Upload `index.html` and `.nojekyll` to the root of the repository. `README.md` is recommended. The QA files are supporting documentation and do not need to be published.
3. Commit the files to the `main` branch.
4. In the repository, select **Settings**.
5. Select **Pages** under **Code and automation**.
6. Under **Build and deployment**, select **Deploy from a branch**.
7. Select the `main` branch and the `/(root)` folder, then select **Save**.
8. Wait for GitHub Pages to display the published address.

The typical address will be:

`https://YOUR-GITHUB-USERNAME.github.io/usvi-outcome-reporting-concept/`

## Important sharing note

Treat the GitHub Pages site as publicly accessible unless your organization's GitHub plan and repository settings explicitly provide restricted Pages access. This demonstration contains sample Healthcare-sector information only. Do not add live project, employee, client, financial, security, or protected healthcare information.

## Demonstration scope

This is a front-end concept. It does not connect to SharePoint lists, Power Automate, Power BI, authentication, or production data. A production SPFx implementation would replace the sample content with approved SharePoint records and apply the organization's access, retention, and governance requirements.
