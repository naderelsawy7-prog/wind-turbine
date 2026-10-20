# Wind Turbine Quick Performance Calculator

A self-contained, beginner-friendly screening calculator for small wind turbines. It runs in a modern browser, works offline, and does not need a build step or third-party libraries.

## Quick start

1. Open `index.html` in a browser, or publish the folder with GitHub Pages.
2. Replace the pre-filled example values with the turbine’s datasheet values and a long-term average wind measurement.
3. Read the two headline estimates. They update automatically as inputs change.
4. Open **More results & checks** for the power curve and wake screen, or **Reference & beginner help** for explanations and sources.

The pre-filled values are examples—not a forecast for any particular site. A 12-month wind measurement at turbine height and the manufacturer’s certified power curve are preferable.

## What it estimates

- **Electrical power at the entered wind speed:** a simplified constant-power-coefficient model, capped at rated power and adjusted for cut-in / optional cut-out speed.
- **Yearly electricity:** rated power × 8,760 hours × the selected capacity factor. This is a screening estimate; it is not calculated from a year-long wind-speed distribution or a certified turbine power curve.
- **Rotor area:** HAWT uses `π × diameter² ÷ 4`; the VAWT option uses the approximate H-rotor area `diameter × height`.
- **Optional wake screen:** a simplified Jensen model for one aligned downstream turbine. It is not a wind-farm layout design tool.

The interface uses EPROM-inspired navy, teal, cyan and gold colors. All calculations run locally in the browser. The CSV download and print-to-PDF actions also run locally.

## Project files

- `index.html` — complete application: markup, styles, calculator logic, charts, guide and source links are included in this one file.
- `README.md` — project and usage notes.
- `CHANGELOG.md` — brief version history.
- `.gitignore` — common local-machine files excluded from Git.

## Publish with GitHub Pages

1. Create a GitHub repository and upload the files in this folder to the repository root.
2. Open the repository’s **Settings → Pages**.
3. Choose deployment from a branch, select `main` and the `/ (root)` folder, then save.
4. After GitHub Pages finishes building, use the URL shown in the Pages settings.

There are no dependencies to install and no build command to run. The calculator itself works offline after the HTML file has been downloaded. The source-document links shown in the app point to Google Drive files and may require permission to view.

## Important limitations

This is for early screening and learning only. It does not replace measured site data, a certified power curve, structural/electrical design, permitting, or professional engineering review. Regional capacity factors and wake parameters are assumptions and should be verified for a real project.

## License

No license has been selected. Add a license file before distributing or reusing the project publicly.
