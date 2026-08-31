# Design QA

## Comparison target

- Source visual truth: `C:\Users\MCGARIAL\AppData\Local\Temp\codex-clipboard-96830f71-906e-47bc-b6dc-661af3d7c098.png`
- Browser-rendered implementation: `C:\Users\MCGARIAL\Documents\Codex\2026-08-27\referenced-chatgpt-conversation-this-is-an\outputs\USVI_SPFX_Outcome_Reporting_Concept_GitHub_Pages\qa-functional-portfolio-top.png`
- Browser viewport and implementation pixels: 1280 × 720 CSS pixels at 1× density.
- Source pixels: 1261 × 925.
- State: Functional Work & Outcomes; “I completed or supported work” selected; Selected project(s); Healthcare and Education selected; three projects selected.
- Theme normalization: source is light and implementation capture is dark. The implementation uses theme-aware equivalents; comparison focuses on structure, hierarchy, density, spacing, and semantic color mapping.

## Full-view comparison evidence

The implementation preserves the reference SPFx pattern: two compact top tabs, Segoe UI typography, square native controls, restrained borders, a dense form layout, a direct-submission workflow, and submission history. The portfolio picker and audit-oriented work fields extend the form without changing the established visual language.

## Focused comparison evidence

The scope region was inspected at full desktop scale. All 54 projects, selected sectors, and selected projects are mutually exclusive scope choices. The four-sector checkbox row and searchable project checklist remain readable, and selected projects are represented as tags below the list.

## Required fidelity surfaces

- Fonts and typography: Passed. Segoe UI hierarchy, compact labels, normal and medium weights, wrapping, and helper text remain consistent.
- Spacing and layout rhythm: Passed. The scope selector, sector row, search action row, and two-column project list align with the SPFx grid.
- Colors and visual tokens: Passed. Navy chrome, blue selected states, neutral controls, and semantic colors preserve the reference in light and dark appearances.
- Image quality and asset fidelity: Passed. No required raster imagery, illustration, or custom icon assets are present.
- Copy and content: Passed. The form asks what happened in plain language, explains both choices with concrete examples, gives unsure users a safe default, states that functional-lead approval is not required, and explains when information can feed weekly and monthly reporting.

## Primary interactions tested

- All 54 projects hides sector and project selectors.
- Selected sector(s) displays Healthcare, Infrastructure, PMO, and Education while hiding the project picker.
- Selected project(s) displays both sector filters and the project picker.
- Search filters the representative project list.
- Select all shown selects visible matches.
- Clear selection removes all project selections.
- Selected count and project tags update with checkbox changes.
- “I completed or supported work” keeps the factual work-record fields visible and hides the outcome/reporting sections.
- “The work produced a material result or change” reveals outcome, impact, evidence, commitments, dependencies, and leadership-support fields.
- Submit Work Record displays a direct-submission confirmation with timestamp, version-history, and reporting-curation language.
- Add Another Work Item creates a separately labeled work item with its own category and details; Remove deletes it and renumbers the remaining items.
- Multiple work items share the submission's function, reporting week, and submitter while retaining separate work dates and affected project/sector selections.
- Each work item supports multiple affected projects or sectors as removable tags; choosing All 54 projects replaces narrower selections for that item.
- No Functional Lead review or approval status remains in the functional flow or sample history.
- Two top-level reporting tabs continue to work.
- Weekly PM reporting switches correctly among one project, several selected projects, and a saved bundle.
- Saved bundle selection updates the member-project tags and project count; ad hoc project selection supports adding and removing individual projects.
- Browser console checked: no errors.

## Comparison history

### Iteration 1

- Finding: [P2] Project items marked hidden by search remained visible because the checkbox-row display rule overrode the browser's hidden attribute.
- Fix: Added an explicit hidden-state rule for project items.
- Post-fix evidence: Searching “Hospital” shows two matching projects; clearing the search restores all eight representative projects.

## Findings

No actionable P0, P1, or P2 issues remain.

## Follow-up polish

- [P3] Production SPFx should show the complete project count by sector and virtualize the 54-project list if portfolio size increases significantly.

final result: passed
