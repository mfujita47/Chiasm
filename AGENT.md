# 🤖 AGENT.md - Chiasm Development Guide

## Project Overview

**Chiasm** is a modern, elegant Marp theme for creating information-dense presentation slides. It's a customized version of the [Canyon](https://github.com/Jzurde/canyon) theme, tailored for professional and technical presentations with a focus on readability and visual clarity.

### Key Characteristics
- **Language**: CSS (primary theme file)
- **License**: MIT
- **Repository**: https://github.com/mfujita47/Chiasm
- **Status**: Active development (v1.1.0)
- **Created**: 12 days ago
- **Last Updated**: 7 days ago

## Repository Structure

```
mfujita47/Chiasm/
├── chiasm.css                    # Main theme stylesheet
├── README.md                     # Project overview and quick start
├── CHANGELOG.md                  # Version history and updates
├── chiasm-usage-guide.md        # Detailed usage documentation
├── chiasm-usage-guide.pdf       # PDF version of usage guide
├── chiasm-generation-prompt.md  # AI prompt template for slide generation
├── LICENSE                       # MIT License
├── .gitignore                   # Git ignore rules
└── AGENT.md                     # This file - development guide
```

## Core Features

### 1. **Two-Column Layout**
- `twoColumns` CSS class enables side-by-side content
- Perfect for comparisons, parallel information, and dense content

### 2. **Visual Components**
- **Color Boxes**: Four-color system (blue, green, yellow, red) for emphasis and organization
- **Tags**: Labels for categorization, importance levels, and highlighting
- **Arrows**: Visual flow indicators for processes and reasoning chains

### 3. **Typography & Design**
- BIZ UDPGothic font base for professional readability
- Automatic pagination with page numbers in header/footer
- Modern, minimalist design principles
- Information-density focused layouts

## Installation & Setup

### For Marp Users
1. Add to VS Code `settings.json`:
```json
"markdown.marp.themes": [
  "https://raw.githubusercontent.com/mfujita47/Chiasm/main/chiasm.css"
]
```

2. Or use locally:
   - Download `chiasm.css`
   - Reference via relative path in your Marp project

### Basic Marp Configuration
```markdown
---
marp: true
theme: chiasm
paginate: true
---
```

## Development & Contribution

### Adding New Features
1. Modify `chiasm.css` with new CSS classes or style extensions
2. Document changes in `CHANGELOG.md`
3. Update `chiasm-usage-guide.md` with usage examples
4. Test thoroughly in Marp environment

### Enhancement Ideas
- Additional color box options
- New layout templates
- Custom component designs
- Theme variants (dark mode, minimal, etc.)
- Additional typography options

## AI-Assisted Development

### Slide Generation Workflow
Chiasm includes an AI prompt template (`chiasm-generation-prompt.md`) that enables LLMs like ChatGPT and Claude to generate Chiasm-formatted Markdown:

1. Copy `chiasm-generation-prompt.md` content
2. Paste into your LLM conversation
3. Describe desired slide content and structure
4. LLM outputs optimized Chiasm-formatted Markdown

### Suggested AI Uses
- Generating presentation structure from outline
- Creating component-rich slide layouts
- Formatting complex multi-column content
- Producing consistent theme-aligned slides
- Batch slide generation for large presentations

## File Purposes

| File | Purpose |
|------|---------|
| `chiasm.css` | Core theme styling - the heart of the project |
| `README.md` | Quick reference and getting started guide |
| `CHANGELOG.md` | Version history and notable changes |
| `chiasm-usage-guide.md` | Comprehensive documentation with examples |
| `chiasm-usage-guide.pdf` | Printable/portable version of guide |
| `chiasm-generation-prompt.md` | System prompt for AI-assisted slide creation |

## Customization Guidelines

### CSS Modifications
- Maintain the existing class structure for backward compatibility
- Use CSS variables for colors to enable theming
- Document new classes in the usage guide
- Test with various content types before releasing

### Best Practices
- Keep component naming intuitive and descriptive
- Provide visual examples for new features
- Ensure responsive design considerations
- Maintain the professional aesthetic

## Testing & Quality Assurance

- Test theme with various content types
- Verify pagination works correctly
- Check typography across different zoom levels
- Validate two-column layouts with different content lengths
- Test color box and tag combinations

## Attribution & Credits

- **Original Theme**: [Canyon](https://github.com/Jzurde/canyon) by Jzurde
- **Customization & Maintenance**: [mfujita47](https://github.com/mfujita47)
- **License**: MIT (see LICENSE file)

## Future Directions

- Theme variants and color schemes
- Additional layout templates
- Enhanced component library
- Theme documentation website
- Community contributions and improvements

## Related Resources

- [Marp Documentation](https://marp.app/)
- [Canyon Theme (Original)](https://github.com/Jzurde/canyon)
- [Chiasm Usage Guide](./chiasm-usage-guide.md)
- [Chiasm Generation Prompt](./chiasm-generation-prompt.md)

---

**Last Updated**: 2026-02-15
**Maintainer**: mfujita47