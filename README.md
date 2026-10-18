# Personal Education Plan Builder (Cohort 2026)

Version 1.4.1 — 19 October 2026.

[Open the PEP Builder](https://dannyscholten.github.io/PEP-builder/)

A student-facing, browser-based builder for a 120 EC Drug Discovery Sciences programme. It supports research specialisations and Education in Drug Discovery, with relative Year 1/Year 2 planning. A build supports preparation; it does not grant institutional approval.

## Build and review

Select specialisation, path where applicable, and previous education to preload required courses. The **Course Catalog** groups **Compulsory components** and **Elective space**. Use **+** and choose the academic year, or drag courses and projects onto the **PEP Builder Canvas**. **+ Add unlisted course** is at the bottom of **Elective space** in the catalog. Category guidance is behind **i** buttons. Clicking a colored canvas legend label opens the matching catalog category; **Research project(s)** opens both major and minor groups.

Added courses have consistent edit and remove controls in the catalog and canvas. Compulsory Education components retain their removal restriction. Required research-specialisation courses can be removed for review, with unmet curriculum checks and export restrictions where applicable.

Click a placed course or project to open **Course details**. Regular courses show their teaching periods. Research projects and the literature thesis expose permitted start months; dates use month boundaries. For research projects, **Days per week & leave** contains optional adjustments. A hatched project segment opens leave settings directly. Education's 30 EC major is full-time without leave/part-time controls, in Year 1, starting February–April.

**Confirm** keeps course edits. Clicking outside or pressing Escape discards unconfirmed course edits. Required-input additions are cancelled in full when their details are dismissed. Unconfirmed edits are not written to autosave or Undo history.

The EC total and warning count stay visible at the top. Curriculum checks identify met and unmet requirements. Workload/overlap warning cells link to detailed explanations; high-workload explanations identify the academic year and teaching period. New warnings appear briefly in orange at the top and remain in the detailed overview until resolved. Confirmations are green; errors are red. Routine confirmations disappear after 4.5 seconds and warning notices after 7 seconds.

## Save and export

- **Save build** downloads a portable build JSON file. **Open build** restores it.
- Autosave keeps the confirmed build and recent Undo/Redo history in this browser. Browser storage is specific to the browser and site; use a build file when moving between devices or from the standalone file to the published website.
- **Undo**, **Redo** and **Reset** are grouped beside save/open. Reset requires confirmation.
- **Export PDF** is enabled from 120 EC once required placement choices are complete. It produces an A3 landscape visual overview, workload/overlap status, applicable scheduling warnings, curriculum checks with their actual status, and course tables grouped into Compulsory components and Elective space. Both years share an overview page when readable; further pages are added as necessary.
- **Export for approval** creates a schema 2 PEP draft for **Import draft PEP** in the [DDS PEP approval tool](https://dannyscholten.github.io/dds-pep/2026/). Complete personal/project details and exception requests in that tool. The transfer targets PEP 0.10.6, rule DDS-2026-2027.13. Planning dates remain in `plannerTransfer`; they are not inserted into Additional explanation.
- A Year 1 research-specialisation major uses Part I + Part II registration; a Year 2 major uses the single 48 EC variant. Education has its own 30 EC major.

## Mobile

The default phone view is a year-specific course list; Calendar offers a horizontally scrollable visual overview. **+ Add courses & projects** stays visible in the sticky header while scrolling and opens the catalog. A legend shortcut opens that catalog at the chosen category. Newly added courses switch the list to their assigned year.

The sticky phone header keeps EC and warnings visible. **Build actions** opens save/open, history/reset, help and export controls without requiring sideways toolbar scrolling. Touch targets, full-height catalog scrolling, bottom course actions and safe-area spacing are adapted for phones. Desktop retains the visible toolbar and side catalog.

The optional six-step interactive tour uses temporary fictional data and restores the user's own build when finished or skipped. The help icon restarts it; the introduction can be dismissed or hidden for future visits.

## Sources, privacy and maintenance

The footer links to the DDS Teaching and Examination Regulations 2026–2027 and the programme feedback form. Annual Study Guide references remain linked for each course. All calculations and files run locally in the browser; there is no application backend. PDF libraries and font assets are bundled under `vendor/`, with licenses included.

GitHub Pages serves the `main` branch root. Readable development sources live in the separate planner workspace; `python3 src/build.py` rebuilds the standalone file and this Pages package. Storage keys, saved-build kinds and schema remain compatible with existing builds.

## Verification

Verified with the actual application code in DOM emulation: all legend routes, catalog/canvas removal, Education restrictions, popup cancellation and Confirm/Undo, save/open payload round-trips, PEP schema 2 import, new-warning notices, and tour restoration. Responsive interaction branches were checked at 320, 390, 700, 768 and 1456 px. Research and Education PDF outputs were rendered and visually inspected, including checklist continuation and missing-requirement states.

These checks do not substitute for physical-device Safari/Chrome testing. Native on-screen keyboard, touch scrolling, browser download/share behaviour and screen-reader use remain recommended device checks.
