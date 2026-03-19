# figma-to-code-with-claude

**by Taroon Tyagi · Principal Designer · March 2026**

A field guide for designers and developers navigating the Figma → Claude → Code workflow. Two full deck editions plus a quick reference — pick what fits.

## 🔗 Live

**[https://taroontyagi.github.io/figma-to-code-deck/](https://taroontyagi.github.io/figma-to-code-deck/)**

| Page | URL |
|---|---|
| Landing | `/` |
| Designer Edition | `/designer.html` |
| Developer Edition | `/developer.html` |
| Quick Reference | `/quickref.html` |

---

## Files

| File | Description |
|---|---|
| `index.html` | Landing page — choose your edition |
| `designer.html` | Figma-style UI · 23 slides · Design-focused |
| `developer.html` | GitHub-style UI · 17 slides · Terminal-focused |
| `quickref.html` | One-page summary with deep links into both decks |
| `README.md` | This file |
| `.nojekyll` | Disables Jekyll on GitHub Pages |

---

## Designer Edition — 23 slides

Figma-core aesthetic: toolbar, layers panel, properties panel, canvas grid. Full keyboard navigation, zoom, and focus mode.

| Section | Slides |
|---|---|
| Intro | Hero · Agenda · Toolkit |
| Foundations | Design Tokens · Figma Prep · Code Connect |
| Workflow | The Loop · Visual Thinking · Code→Canvas · Components |
| Prompting | Anatomy · Weak vs Strong · Templates |
| Limits | Can Do · Can't Do · Figma→Web Gap · Pro Tips |
| Skills | What & Why · Build Your Own · Skill Library |
| Tools | figma-console-mcp |
| Close | Ways of Working · Close |

### Keyboard shortcuts

| Key | Action |
|---|---|
| `← →` or `↑ ↓` | Navigate slides |
| `1–9` | Jump to slide |
| `\` | Toggle all panels |
| `P` | Focus mode — hides chrome, centers short content, scrolls tall content |
| `Esc` | Exit focus mode or panel-hide |
| `⌘=` / `⌘-` | Zoom in / out |
| `⌘0` | Reset zoom to 100% |
| `F` | Fullscreen |
| `Ctrl/⌘ + scroll` | Zoom with trackpad/mouse |

### Focus mode
- **Short slides** — content optically centered (~45% from top), grid hidden, chrome hidden
- **Tall slides** — top-aligned at natural scale, scrollable, no zoom applied

---

## Developer Edition — 17 slides

GitHub dark UI (gray-900). Left sidebar = file tree navigation. All code blocks are copy-paste ready.

| Section | Files |
|---|---|
| *(root)* | `README.md` · `CHANGELOG.md` |
| `setup/` | `install.sh` · `mcp-config.md` · `figma-prep.md` |
| `workflow/` | `loop.md` · `figma-web-gap.md` · `limits.md` · `code-to-figma.md` |
| `prompting/` | `anatomy.md` · `examples.md` · `templates.md` |
| `skills/` | `intro.md` · `build.md` · `registry.md` |
| `tools/` | `console-mcp.md` |
| `team/` | `ways-of-working.md` |

### Keyboard shortcuts

| Key | Action |
|---|---|
| `← →` or `↑ ↓` | Navigate slides |
| `1–9` | Jump to slide |
| `\` | Toggle sidebar |
| `P` | Focus mode |
| `Esc` | Exit focus / close sidebar |
| `⌘=` / `⌘-` | Zoom in / out |
| `⌘0` | Reset zoom |
| `F` | Fullscreen |
| `Ctrl/⌘ + scroll` | Zoom with trackpad/mouse |

---

## Deploy to GitHub Pages

```bash
# From inside the unzipped folder:
gh repo create figma-to-code-deck --public --source=. --push
gh api repos/:owner/figma-to-code-deck/pages \
  --method POST \
  --field source='{"branch":"main","path":"/"}'
```

Live at: `https://taroontyagi.github.io/figma-to-code-deck/`

---

## Key resources

| Resource | URL |
|---|---|
| Figma MCP Guide | https://help.figma.com/hc/en-us/articles/32132100833559 |
| Remote MCP Setup | https://developers.figma.com/docs/figma-mcp-server/remote-server-installation/ |
| Claude Code Install | https://code.claude.com/docs/en/setup |
| Agent Skills Docs | https://code.claude.com/docs/en/skills |
| skills.sh directory | https://skills.sh |
| anthropics/skills | https://github.com/anthropics/skills |
| vercel-labs/agent-skills | https://github.com/vercel-labs/agent-skills |
| figma-console-mcp | https://github.com/southleft/figma-console-mcp |
| claude-to-figma skill | https://github.com/designagentlab/skills/tree/main/claude-to-figma |
| Code→Figma blog | https://www.figma.com/blog/introducing-claude-code-to-figma/ |
