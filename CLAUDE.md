# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a MARP (Markdown Presentation Ecosystem) template repository for creating academic presentations, primarily designed for Japanese language content. It provides a comprehensive design system and multiple slide layouts.

## Key Files

- `marp-template.md`: Main template file containing 9 different slide design patterns with custom CSS
- `marp-slide-creation-rules.md`: Comprehensive guidelines (in Japanese) for creating presentations
- `marp.config.js`: MARP configuration allowing local file access

## MARP Commands

Since this is a template repository without package.json, use the MARP CLI directly:

```bash
# Generate HTML presentation
marp marp-template.md

# Generate PDF presentation
marp marp-template.md --pdf

# Watch mode for development
marp marp-template.md --watch

# Serve presentation locally
marp marp-template.md --server
```

## Design System

The template uses a defined color palette:
- Primary: #2E86AB
- Secondary: #A23B72
- Accent: #F18F01
- Background variations: #f8f9fa, #e9ecef

## Content Guidelines

When editing or creating slides:
- Headings: 1-2 lines maximum
- Body text: 6-8 lines per slide
- Japanese text: 35-40 characters per line
- Bullet points: 3-5 items maximum (see bullet point guidelines below)
- Base font size: 1.15em for readability

### Important: Bullet Point Usage Guidelines

**Be cautious with bullet points** - they can obscure logical relationships between ideas:

- Use bullet points ONLY for truly parallel, independent items
- Avoid bullet points for cause-effect relationships, processes, or logical arguments
- Consider alternatives: flow diagrams, numbered lists, comparison tables, or narrative text
- If using bullet points, add introductory text explaining the relationship between items

See `marp-slide-creation-rules.md` for detailed guidelines on appropriate bullet point usage.

## Slide Patterns Available

1. **title**: Centered title slide
2. **grid**: Grid layout for multiple items
3. **card**: Card-style list presentation
4. **icon**: Icon-based visual blocks
5. **table**: Styled data tables
6. **image**: Centered image with caption
7. **problem-solution**: Side-by-side comparison
8. **budget**: Financial/numerical data table
9. **two-column**: Parallel information layout

## Working with Templates

To create a new presentation:
1. Copy `marp-template.md` to a new file
2. Modify the content while keeping the CSS styles in the front matter
3. Use the `<!-- _class: [pattern-name] -->` directive to apply different slide layouts
4. Follow guidelines in `marp-slide-creation-rules.md` for content organization

## ⚠️ CRITICAL WARNING: PDF Preview Commands

**絶対に実行してはいけないコマンド:**
```bash
# NEVER use these commands - they cause preview function to malfunction:
open *.pdf
open marp-template.pdf
open marp-template-enhanced.pdf
# Or any variation of the 'open' command with PDF files
```

**理由:** macOSのPDFプレビューが暴走し、システムリソースを大量に消費する問題が発生します。

**代替方法:**
- PlaywrightのMCPツールを使用してPDFを確認: `mcp__playwright__browser_navigate` with file:// URL
- HTMLファイルを生成して確認: `marp file.md --html`
- ユーザーが手動でPDFを開く

**重要:** この警告は絶対に遵守してください。プレビュー機能の暴走を防ぐため、PDFファイルを自動的に開くコマンドは一切使用しないでください。