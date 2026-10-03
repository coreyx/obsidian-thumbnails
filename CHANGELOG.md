# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.4.0] - 2026-10-02

### Added
- Insert Thumbnail on Paste: pasting a YouTube or Vimeo link into a note automatically wraps it in a `vid` code block, like the "Insert thumbnail from URL in clipboard" command.
  - Only triggers when the clipboard holds a single video link.
  - Normal pasting is kept when text is selected or the cursor is inside a code block.
  - When pasting mid-line, the code block is placed on its own lines so it renders.
  - Falls back to pasting the plain link if the video ID can't be resolved.
- "Insert Thumbnail on Paste" setting (enabled by default) to turn the paste behavior off.
- BRAT installation instructions in the README.

For releases before 1.4.0, see the [upstream releases](https://github.com/Meikul/obsidian-thumbnails/releases).

[1.4.0]: https://github.com/coreyx/obsidian-thumbnails/releases/tag/1.4.0
