# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.0] - 2025-06-16

### Changed

- Major refactoring of the core conversion engine for improved performance and reliability
- Updated to use the latest version of docx library (v8.0.0)
- Improved error handling and reporting
- Enhanced type safety throughout the codebase

### Breaking Changes

- Removed support for legacy style options
- Changed default font family to 'Calibri'
- Modified table of contents generation API
- Updated configuration interface for better type safety

### Added

- Support for custom page margins
- Enhanced image handling with better size control
- New style options for list formatting
- Improved documentation with TypeScript examples

## [1.4.9] - 2025-06-6

### Changed

- added numbered list support
- Updated dependencies to latest versions
- Improved documentation and examples

## [1.4.8] - 2025-05-27

### Fixed

- Corrected an issue where markdown bold syntax (`**text**`) with internal spaces was not being rendered correctly as bold text in the output document.

## [1.4.7] - 2025-05-27

### Added

- Added feature to remove markdown separators (e.g., ---)

## [1.4.6] - 2025-04-28

### Changed

- Improved table detection and handling:
  - Enhanced regex checks for table separators
  - Better support for additional table format ting scenarios
  - More robust table structure validation

## [1.4.5] - 2025-04-28

### Added

- Level-specific styling for Table of Contents entries:
  - `tocHeading1FontSize` through `tocHeading5FontSize` for different font sizes
  - `tocHeading1Bold` through `tocHeading5Bold` for bold formatting
  - `tocHeading1Italic` through `tocHeading5Italic` for italic formatting

## [1.4.4] - 2025-04-28

### Added

- Custom font size for Table of Contents entries via `tocFontSize` style option.

## [1.4.3] - 2025-04-28

### Added

- Automatic page numbering (centered in the footer).

## [1.4.2] - 2025-04-28

### Added

- Table of Contents (TOC) generation via `[TOC]` marker.
- Clickable internal links from TOC entries to corresponding headings.
- Page break support via `\pagebreak` command on its own line.

## [1.4.1] - 2025-04-19

### Changed

- Reorganized test files into dedicated `tests` directory
- Improved test organization and structure
- Enhanced test coverage for list formatting features

## [1.4.0] - 2025-04-19

### Added

- Enhanced text alignment support with improved justification handling
- Better spacing control for justified text
- Improved paragraph formatting with dynamic spacing

### Changed

- Updated text alignment implementation for better compatibility
- Refined default alignment settings for better document consistency

## [1.3.1] - 2025-04-18

### Changed

- Updated default heading alignments to be consistently left-aligned
- Improved heading alignment configuration with individual level controls

## [1.3.0] - 2025-03-31

### Added

- Text alignment support for all document elements
  - Paragraph alignment (LEFT, RIGHT, CENTER, JUSTIFIED)
  - Blockquote alignment (LEFT, CENTER, RIGHT)
  - Default heading alignments (H1: CENTER, H2: RIGHT, others: LEFT)
  - Configurable alignment through style options
- Enhanced documentation with text alignment examples

## [1.2.2] - 2025-03-31

### Added

- Custom font size support for all document elements
  - Headings (H1-H5)
  - Paragraphs
  - List items
  - Code blocks
  - Blockquotes
- Enhanced documentation with examples of custom font sizes

## [1.1.1] - 2025-03-30

### Added

- GitHub Actions workflows for CI/CD
- Automated npm publishing on release
- Automated testing and type checking

### Changed

- Updated build process to be more robust
- Improved documentation

## [1.1.0] - 2025-03-30

### Added

- Support for code blocks (inline and multi-line)
- Support for strikethrough text
- Support for links
- Support for images (embedded, non-clickable)

## [1.0.0] - 2025-03-29

### Added

- Initial release
- Convert Markdown to DOCX format
- Support for headings (H1, H2, H3)
- Support for bullet points and numbered lists
- Support for tables
- Support for bold and italic text
- Support for blockquotes
- Support for comments
- Customizable styling
- Report and document modes
