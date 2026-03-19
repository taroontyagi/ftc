# figma-to-code-with-claude

**by Taroon Tyagi · Principal Designer · March 2026**

A field guide for designers and developers navigating the Figma → Claude → Code workflow. Two editions, same content focus — pick the one that fits how you think.

---

## Files

| File | Description |
|---|---|
| `index.html` | Landing page — choose your edition |
| `designer.html` | Figma-style UI · 19 slides · Design-focused |
| `developer.html` | GitHub-style UI · 13 slides · Terminal-focused |

## Live URL (after GitHub Pages deploy)

```
https://taroontyagi.github.io/figma-to-code-deck/
```

---

## Designer Edition — 19 slides

Figma-core aesthetic (toolbar, layers panel, properties panel, canvas grid). Keyboard navigation, zoom controls, focus mode.

| Section | Slides |
|---|---|
| Intro | Hero · Agenda · Toolkit |
| Foundations | Design Tokens · Figma Prep · Code Connect |
| Workflow | Workflow · Prompting · Visual Thinking · Code→Canvas · Components |
| Limits | Can Do · Can't Do · Pro Tips |
| Skills | What & Why · Build Your Own · Skill Library |
| Tools | figma-console-mcp |
| Close | Close |

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

### Focus mode behaviour
- **Short slides** — content is optically centered (~45% from top), grid hidden, chrome hidden
- **Tall slides** — top-aligned at natural scale, scrollable, no zoom applied

---

## Developer Edition — 13 slides

GitHub dark UI (gray-900). Left sidebar = file tree navigation. All code blocks are copy-paste ready.

| Section | Files |
|---|---|
| *(root)* | `README.md` · `CHANGELOG.md` |
| `setup/` | `install.sh` · `mcp-config.md` · `figma-prep.md` |
| `workflow/` | `loop.md` · `prompts.md` · `limits.md` · `code-to-figma.md` |
| `skills/` | `intro.md` · `build.md` · `registry.md` |
| `tools/` | `console-mcp.md` |

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
