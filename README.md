# Elegant Theme for Zed

A Zed port of [Elegant Theme](https://github.com/yx208/intellij-elegant-theme) for JetBrains IDEs.

## Themes

| Theme | Description |
|---|---|
| Elegant Ink Light | An eye-friendly ink-wash (水墨) light theme: ink-tone text and low-saturation traditional Chinese colors on warm rice-paper (宣纸) backgrounds, with no pure black or white anywhere |

## Install

From source, while the extension is not yet published:

1. Clone this repository.
2. In Zed, run `zed: install dev extension` from the command palette and select the cloned folder.
3. Run `theme selector: toggle` and pick **Elegant Ink Light**.

## Palette

| Role | Color |
|---|---|
| Paper (editor, panels, terminal) | `#F6F0DF` |
| Window base (title bar, status bar, tab bar) | `#EAE2CC` |
| Ink text / secondary / disabled | `#3B3A36` / `#6B675E` / `#9B937B` |
| Accent (focus) | `#44546B` |
| List selection / editor selection | `#C8D5E3` / `#E2D8BC` |
| Keyword / string / number / function | `#33568C` / `#4A7A3D` / `#A85F2E` / `#2E7093` |
| Constant & field / type / attribute & macro / comment | `#8E4D82` / `#2E7D6E` / `#96781C` / `#8F8873` |

Every color comes from the final values of the JetBrains version (2.1.1). Terminal dim colors, collaborator cursors and rainbow-bracket accents are derived from those same hues.

## Differences from the JetBrains version

Zed themes only control colors, and Zed highlights code with tree-sitter rather than a full semantic model, so a few things do not carry over:

- The Islands layout (gaps between islands, rounded corners, menu and tree row heights). Panels sit directly next to the editor and are separated by a 1px border.
- The focused/unfocused editor-tab chips with outlines. Zed has one background for the active tab and one for the others; the active tab uses the paper color and joins the editor.
- Semantic distinctions such as static vs. instance fields, underlined reassigned or `mut` bindings, and wavy-underline markers.
- `attribute` covers Rust attributes, decorators and HTML attribute names alike, so HTML attribute names are ochre here instead of ink.

## License

[Apache-2.0](LICENSE)
