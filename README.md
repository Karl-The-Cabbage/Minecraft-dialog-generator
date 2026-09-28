# Minecraft Dialog GUI Generator

A visual builder for Minecraft's `/dialog show` command (Java Edition 1.21.6+).
Design a dialog with a live preview, then copy the generated command. It's a single
static web page: no server, no build step, no dependencies, and it works offline.

_Not affiliated with Mojang or Microsoft._

## Features

- Title, body text, button grid columns, pause and after-action settings
- Player inputs: text, checkbox, dropdown, number slider
- Buttons with color (including custom hex), bold/italic/underline/strikethrough, tooltips
- Button actions: run command, suggest command, open URL, copy to clipboard, open another dialog
- Optional exit button, and choice of who sees the dialog (`@p`, `@a`, `@s`, or custom)
- Live preview, command length counter, and a "Things to check" linter
- Templates, save/load configs (browser storage), JSON export/import, import an existing command
- Share by link, auto-saved draft, collapsible sections, compact/comfortable layout

## Run it

- **Just open it:** double-click `index.html`. Everything works except offline caching.
- **Host it on GitHub Pages:** push this folder to a repo, then go to
  *Settings → Pages → Deploy from a branch → `main` / root*. Your app will be at
  `https://<you>.github.io/<repo>/`.
- **Install it as an app:** open the hosted (https) page in Chrome or Edge and use
  *Install app* in the address bar. It then opens in its own window and works offline.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app (HTML, CSS, JS in one file) |
| `manifest.webmanifest` | Makes the page installable |
| `sw.js` | Service worker for offline use |
| `icons/` | App icons |

## Notes

- Saved configs and drafts live in your browser's local storage, so they are per-browser.
- Share links contain your whole GUI in the URL after the `#`.
- The field names for newer dialog features were written from documentation, so if
  Minecraft rejects a generated command, please open an issue with the error message.

## License

MIT. See `LICENSE` (replace `YOUR NAME` with your own).
