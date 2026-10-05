# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Fixed
- The package now ships its backoffice files as Razor Class Library static web assets instead of NuGet content files. The property editor is picked up when running locally (F5 / `dotnet run`), not only after `dotnet publish`, and nothing is copied into the consuming project.

## [1.1.0] - 2026-07-29

### Added
- SVG Sprite Path setting now uses a static-file picker (filtered to `.svg`) instead of a free-text input

### Fixed
- Sprite fetch and icon previews bypass the browser cache, so newly added icons show up without a hard refresh

## [1.0.1] - 2026-06-04

### Changed
- Added NuGet package icon and Umbraco Marketplace listing metadata

## [1.0.0] - 2026-06-03

### Added
- Initial release targeting Umbraco 17+ (net10.0)
- SVG symbol picker property editor with visual preview grid
- Configurable per data type: sprite path and picker title
- Searchable symbol grid fetched directly from the configured spritesheet
- `Html.SvgIcon()` Razor extension method for inline rendering
- Setup via Umbraco backoffice — no code changes needed
