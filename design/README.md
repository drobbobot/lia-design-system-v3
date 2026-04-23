# Lia Design System — Design Source

Figma file: [Lia shadcn studio](https://www.figma.com/design/I6XZUsUEu44R1gQSGLNQXx/Lia-shadcn-studio)

## `lia-tokens.tokens.json`

Tokens Studio-compatible export of the Lia theme (light + dark). Use this to apply the theme to the shadcn/ui Figma kit when the shadcn/studio Figma plugin or MCP write path is unavailable.

### Import into Figma (via Tokens Studio plugin)

1. In Figma, open the Lia-shadcn-studio file
2. Run the **Tokens Studio for Figma** plugin (install from Community if needed)
3. Tools → Load existing tokens → JSON file → select `design/lia-tokens.tokens.json`
4. In the Tokens Studio panel, apply the `Lia Light` theme (then `Lia Dark` for the dark mode)
5. Tools → Sync → Figma Variables → this writes the tokens into the `☀️ Mode` variable collection

### Import into Figma (manual, no plugin)

If Tokens Studio isn't available, you can paste the hex values directly into the `☀️ Mode` collection's Light and Dark mode columns. The JSON keys match the `theme/*` variable names.

### Source of truth

The canonical theme source is `src/app/globals.css` — these JSON files are regenerated from that.
