# Drug Discovery Sciences Personal Curriculum Planner

Version 1.2.8 — 11 October 2026.

Published with GitHub Pages from the main branch root. All planning and saving happens in your browser; no backend is used.

Choose your specialisation, path where applicable, and previous education. Required courses are preselected. Add courses or projects to either academic year and review the scheduling warnings.

- Planning uses recurring Year 1 and Year 2, September to August, rather than an absolute calendar year. Flexible blocks start on month boundaries and end at the nearest month end after duration calculation. Study-guide links remain annual references.
- A short introduction can be skipped or reopened with Help. Undo and Redo restore recent changes. Autosave stores your plan in this browser; Save my curriculum planning downloads a portable draft.
- On mobile, switch between a course list and a calendar. Add courses and edit blocks through drawers.
- Export PDF becomes available at 120 EC. The A3 landscape PDF contains only the selected timeline, workload overview, year totals and applicable warnings. It fits both years onto one landscape page when the rows fit legibly; dense timelines and detailed warnings use additional pages.
- Export for PEP approval downloads a schema 2 draft that can be opened directly with **Open draft** in the [DDS PEP generator](https://dannyscholten.github.io/dds-pep/2026/). Complete the personal and research details there, then follow the coordinator and examination board approval process. An exported plan is not an approval.
- A Year 1 major start maps to Part I + Part II registration; a Year 2 start maps to the single 48 EC variant. PEP export requires the compulsory courses because the PEP generator always includes them.

The curriculum planner is maintained separately from the PEP tool. The PDF libraries are bundled locally under `vendor/`; their licenses and the embedded Noto Sans font license are included there.

Readable development sources and the standalone offline build are kept in the local planner workspace. Run `python3 src/build.py` there to rebuild the standalone HTML and this Pages package.

The major research project can start in Year 1 P5–P6 or Year 2 P1–P3. Older Year 2 P4 plans are retained with a warning so the start can be corrected.

The top toolbar groups Save/Open, the two exports, and Undo/Redo/Reset. Help reopens the introduction. PDF export is visibly disabled below 120 EC.

Help uses the exact action labels. Status messages are shown in red directly below the action buttons. The PDF credit threshold is explained in the button tooltip.

Routine status messages disappear after 4.5 seconds and the status panel collapses when empty. Errors and unresolved warnings persist. The calendar reuses available rows across categories; category affinity is preferred among free rows. RAS stays in its own top row. PDF export uses the same row arrangement.

Block details now open on demand, category guidance is behind information buttons, and literature thesis additions prefer available periods without research overlap. Plans above 120 EC show diploma-supplement guidance.

Version 1.2.2 simplifies course details, uses research days per week and a single 0–8-week leave/pause field, adds explicit course metadata and period summaries, and presents curriculum checks as a checklist.

Version 1.2.2 groups RAS under compulsory courses, combines major/minor legend entries, applies a coordinated pastel palette to the canvas and PDF, and refines the course details timing and action layout.

Reset form now clears all settings and selections after confirmation, with Undo available for recovery.

Version 1.2.2 applies Clear & distinct with muted teal research projects; separates red overlap guidance from red high course workload; exposes study-guide links directly; and uses green checkmarks/red crosses in curriculum checks.

Version 1.2.2 adopts the Clear & distinct palette with muted teal research projects. Workload uses red overlap guidance and red high-workload guidance; checklist boxes use a white check on dark green or white X on red. Study-guide links are directly visible. Course categories start collapsed when settings load or a saved plan opens, with compact added-count badges and selected-course Edit buttons.

Version 1.2.3 makes overlap warnings red in the canvas, detailed warning overview and PDF, while preserving their separate explanations.

Version 1.2.4 places end dates directly below start dates, displays duration summaries, moves research days and leave into More options, simplifies explanatory text, and spells out Alpha/gamma electives in the legend. PEP export targets the verified current form 0.9.0 / schema 2 and includes target version metadata.

Version 1.2.5 places warning explanations below the final timeline wherever space remains, creating continuation pages only when needed.

Version 1.2.6 clarifies the Theory part and Practical part period selectors for Didactics of Science Supervision, with months shown for each period. Both parts may share a period.

Version 1.2.7 requires deliberate selection of both Didactics periods. Confirm, file saving and exports are disabled until both are selected; browser autosave preserves unfinished edits. Each part has an information button with teaching guidance. Existing saved period choices are preserved.

Version 1.2.8 keeps the missing-Didactics-period warning in the main overview without duplicating it in course details. Workload sections are titled Workload or overlap issues and omit the legend in the planner and PDF.
