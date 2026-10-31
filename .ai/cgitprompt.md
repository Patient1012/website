# Task: Extract and Recreate the Standard cgit Web Interface

## Objective

Use the official cgit source code as the reference implementation to recreate its standard web interface as a standalone website.

Official source repository:
https://git.zx2c4.com/cgit/

I want to reuse the standard cgit interface on my own website, without any of its Git functionality.

This is an interface extraction and recreation task, NOT an attempt to build another Git frontend.

## 1. Initial inspection

Before making changes:

1. Inspect the entire existing project.
2. Examine the official cgit source code, particularly:
   - `ui.c`
   - `ui-shared.c`
   - `ui-repolist.c`
   - `ui-summary.c`
   - `ui-log.c`
   - `ui-tree.c`
   - `ui-commit.c`
   - `cgit.css`
   - `cgit.js`
3. Identify how cgit generates its HTML.
4. Identify the common layout components, page structure, styling, typography, spacing, colours and navigation.
5. Determine which parts of the interface are shared between pages and which are page-specific.

Do not assume that the C source contains traditional HTML templates. Follow the actual rendering functions and understand how the output is assembled.

## 2. Interface to recreate

Recreate the standard cgit appearance as closely as possible.

Preserve:

- Overall page layout.
- Header and site title.
- Navigation bar.
- Repository listing appearance.
- Page content positioning.
- Typography.
- Colours.
- Borders and separators.
- Spacing and padding.
- Tables and their styling.
- Links and hover states.
- Footer.
- General proportions and alignment.

The result should look recognisably like the original cgit interface.

Do not redesign it, modernise it, or introduce unnecessary visual changes.

## 3. Remove Git functionality

The website must not implement Git functionality.

Remove or replace:

- Git repository access.
- Git command execution.
- Commit history retrieval.
- Branch management.
- Repository browsing.
- Git diff generation.
- Git-specific backend operations.
- Any server-side functionality that depends on libgit or Git itself.

Where cgit normally displays Git-derived information, use static example data or simple placeholder content.

The purpose is to retain the interface, not its underlying functionality.

## 4. Pages and components

Recreate the standard interface components, including:

- Main page.
- Repository listing.
- Repository information/header.
- Navigation.
- Generic content area.
- Tables.
- Footer.

Where useful, create reusable components rather than duplicating markup.

Do not implement pages or functionality that are unnecessary for reproducing the standard interface.

## 5. Technical requirements

- Use semantic HTML.
- Keep CSS separate from HTML.
- Keep JavaScript separate from HTML.
- Avoid unnecessary JavaScript.
- Do not introduce a backend unless absolutely necessary.
- Make the interface work as a static website.
- Ensure the layout works on desktop and mobile.
- Preserve the original cgit styling wherever possible.

Prefer a simple implementation over introducing a large frontend framework.

If the existing project already has a framework or established structure, follow it unless there is a compelling reason not to.

## 6. Licensing and attribution

cgit is open-source software.

Before copying or adapting any source code, inspect the repository's actual licence and copyright notices.

- Preserve applicable copyright notices.
- Follow the licence's redistribution and attribution requirements.
- Include the required licence text in the project.
- Document which files or components were derived from cgit.
- Do not remove existing licence notices.

If a component is better recreated from observing its HTML and CSS rather than copying its source, that is perfectly acceptable.

## 7. Quality requirements

The finished result should:

- Closely match the original standard cgit interface.
- Have clean, understandable HTML and CSS.
- Avoid unnecessary dependencies.
- Contain no Git backend functionality.
- Be easy to customise later.
- Be usable as a standalone website.

Do not sacrifice visual accuracy for simplicity.

## 8. Testing and verification

Once implemented:

1. Run the website locally.
2. Compare the result against the original cgit website.
3. Check the layout at different screen sizes.
4. Check navigation and hover states.
5. Verify that no Git commands or backend functionality are required.
6. Fix any visual inconsistencies.

## 9. Final report

When finished, provide:

- Files created.
- Files modified.
- Components recreated.
- Any functionality intentionally omitted.
- Licensing information and attribution included.
- Instructions for running the standalone website.

## Important instruction

Work autonomously. Inspect first, plan the implementation, and then complete it.

Do not stop after producing a plan or a basic mockup. The objective is a finished, working recreation of the standard cgit interface.
