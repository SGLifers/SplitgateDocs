# SplitgateDocs

Community documentation for Splitgate, maintained by SGLifers. This repository is a home for references and guides covering settings, game modes, maps, and mechanics as documentation is added.

## Documentation

- [Advanced settings reference](docs/settings/advanced-settings.md) — 115 settings across nine categories, including descriptions, control types, demonstrated ranges, enum choices, and source video timestamps.
- [Advanced settings JSON](data/advanced-settings.json) — the same extraction in a structured format for tools and analysis.
- [Advanced settings frames](assets/advanced-settings/README.md) — all 553 original extracted screenshots, with a frame index and preview.

## Source and scope

The advanced settings extraction covers the **Standard Rules** tab in game build **3.1-643074**, transcribed from a recording named **all advanced settings.mp4**. The recording is not included in this repository; timestamps refer to positions in that recording.

The reference records what was shown in that build. Selected values are not assumed to be defaults. Slider endpoints were documented where demonstrated; exact step sizes and internal precision were not established. Unknown ranges and discrepancies between descriptions and controls are called out in both formats.

## Contributing

Corrections and additional documentation are welcome. Include the game build and supporting evidence where possible. Keep observed behavior separate from assumptions, preserve unknowns, and update both the reference and JSON when changing the advanced settings extraction. Remove personal information, account identifiers, local file paths, and credentials from contributions and supporting media.

This is an unofficial community project and is not affiliated with or endorsed by the game's developers or publishers.
