# Slidev Copilot Template

A production-ready template for creating beautiful, developer-friendly presentations with [Slidev](https://sli.dev) and AI-assisted content creation.

## ✨ Features

- 📝 **Markdown-based** - Write presentations in markdown with full MDC support
- 🎨 **Modern theming** - Customizable themes and transitions
- 🤖 **AI-ready** - Structured for GitHub Copilot assistance with custom instructions
- 🎯 **Consistent formatting** - Biome for code quality and formatting
- 📊 **Visual diagrams** - Built-in Mermaid support for flowcharts and diagrams
- 📤 **Multi-format export** - Build to SPA or export to PDF
- 🔄 **Hot reload** - Live preview with instant updates

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ and npm

### Installation

```bash
# Clone the repository
git clone https://github.com/rkondratowicz/slidev-copilot-template.git
cd slidev-copilot-template

# Install dependencies
npm install
```

### Create Your First Presentation

1. **Create a new folder** under `slides/`:
   ```bash
   mkdir slides/my-presentation
   ```

2. **Create a markdown file** with the same name:
   ```bash
   touch slides/my-presentation/my-presentation.md
   ```

3. **Add npm scripts** to `package.json`:
   ```json
   {
     "scripts": {
       "dev:my-presentation": "slidev slides/my-presentation/my-presentation.md --open",
       "build:my-presentation": "slidev build slides/my-presentation/my-presentation.md --base /my-presentation/ --out dist/my-presentation",
       "export:my-presentation-pdf": "slidev export slides/my-presentation/my-presentation.md --output slides/my-presentation/my-presentation.pdf"
     }
   }
   ```

4. **Start developing**:
   ```bash
   npm run dev:my-presentation
   ```

## 📁 Project Structure

```
├── .github/
│   └── instructions/
│       └── slides.instructions.md    # GitHub Copilot instructions
├── slides/
│   └── example/
│       └── example.md                # Example presentation
├── biome.json                        # Biome configuration
└── package.json                      # Project dependencies and scripts
```

## 📚 Available Presentations

### 📁 slides/
- **example/** - A demonstration presentation showcasing Slidev features (`example.md`)

## 🛠️ Development

### Run a presentation in dev mode
```bash
npm run dev:example          # Run example presentation
```

### Build presentations
```bash
npm run build:example        # Build single presentation
npm run build:all            # Build all presentations
```

### Export to PDF
```bash
npm run export:example-pdf   # Export single presentation
npm run export:all           # Export all presentations
```

## 🤖 AI-Assisted Development

This template includes GitHub Copilot instructions to help you:
- Create new presentations following best practices
- Use up-to-date library documentation via Context7 MCP
- Maintain consistent formatting and structure
- Generate visual diagrams and code examples

## 🤝 Contributing

Contributions are welcome! Please follow the coding guidelines and run formatters before submitting PRs.

---

Made with ❤️ using Slidev and GitHub Copilot