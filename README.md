# UI Design Bundle

A comprehensive suite of UI/UX design intelligence tools, tailored to accelerate frontend development, design systems, and brand consistency.

Based on **UI/UX Pro Max Skill v2.5.0**, this bundle acts as the ultimate design intelligence "brain" spanning from brand identity and system tokens to deep UI component styling and presentations.

## 🌟 What's Included

This bundle packages the following core specialized design skills:

1. **`ui-ux-pro-max`**: Deep UI/UX design intelligence for web and mobile. Includes dozens of styles and guidelines covering accessibility, interactions, and layouts.
2. **`ui-styling`**: Style UIs with shadcn/ui, Tailwind CSS, and canvas-based visual design to create beautiful, accessible user interfaces.
3. **`design-system`**: Generate token architecture (primitive → semantic → component), component specs, and strategic slides.
4. **`design`**: Comprehensive design skill for brand identity, logo generation (55 styles), and CIP (Corporate Identity Program) mockups.
5. **`brand`**: Establish brand voice, visual identity, messaging frameworks, and asset management to maintain brand consistency.
6. **`banner-design`**: Design banners for social media, ads, website heroes, and print across multiple art direction styles.
7. **`slides`**: Create strategic HTML presentations using Chart.js and design tokens.

## 📊 Data Insights & Coverage

The design intelligence relies on a massive underlying database expanded in v2.5.0:

- **161 Product Types** with dedicated reasoning rules.
- **161 Color Palettes** meticulously mapped to different product domains.
- **99 UX Guidelines** with priority-based actionable recommendations.
- **1,923 Google Fonts** in a fully searchable database for expert font pairing.
- **25 Chart Types** and data visualization library recommendations.

## 🛠 Improvements & Sync

- Full english localization across all SKILL documentation.
- CLI robust synchronization making sure the single-source-of-truth aligns with script output.
- Extensive quick-references for checking code on the fly. 

## 🚀 Integration & Connectivity with AI Agents

This bundle is natively designed for agentic AI architectures (such as Gemini Advanced, Antigravity, Cursor, or CLI Agents) that support file-based tool retrieval or `.agents` rulesets.

### How It Works

1. **Rule-Based Retrieval**: Each sub-folder contains a `SKILL.md` file wrapped in metadata. When the AI scans directories for contextual rules, it automatically ingests these `SKILL.md` files as a "context payload" to absorb specific design disciplines.
2. **Dynamic Script Execution**: Inside the `ui-ux-pro-max` folder, Python scripts (like `search.py`) act as a local database engine. The AI Agent runs these scripts under the hood to generate optimal color palettes (Hex codes), interaction patterns, and CSS properties based on the User's product category (SaaS, Ecommerce, Healthcare, etc.).
3. **The Execution Pipeline**:
   - 🗣️ **User Prompt**: "Build a fintech dashboard."
   - 🤖 **AI Ingestion**: The Agent matches "fintech" and "dashboard" with the bundle's capabilities, reading the `ui-ux-pro-max/SKILL.md` instructions.
   - ⚙️ **AI Script Call**: The Agent silently calls the Python data scripts to query the best UX practices and color palettes specifically tuned for "fintech" products.
   - 💻 **Code Output**: The Agent writes your React/HTML code strictly conforming to the returned design system without requiring any human manual styling.

### How to Connect to Your Local Workflow

**1. Connecting to Local Projects (Project-level Context)**
For IDE-level AI Assistants (like Cursor, GitHub Copilot, or Aider), simply clone this repository into an `.agents/skills` sub-directory at the root of your target project:

```bash
cd your-project
mkdir -p .agents/skills
git clone https://github.com/sinhnguyen1411/ui-design-bundle.git .agents/skills/ui-design-bundle
```
Your agent will inherently "see" the `SKILL.md` files during codebase indexing. 

**2. Integrating as a Global Skill (Agent Scratch Folder)**
For system-wide agents (like Antigravity or dedicated local AI engines), place the `ui-design-bundle` folder inside the AI's internal app data or skill scratch directory so it can permanently utilize these tools across any project.
*Standard Local Path Example: `~/.gemini/antigravity/scratch/.agents/skills/ui-design-bundle`*

**3. Direct Integration via Prompting**
If using a standard web chat interface, you can manually attach the specific `SKILL.md` as context before issuing your instruction:
> "Please learn the rules from `@ui-ux-pro-max/SKILL.md` and generate a React UI according to its constraints."

---
*Created automatically to aggregate Design standards across development scopes.*
