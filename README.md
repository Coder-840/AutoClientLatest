# AutoClientPATCH

This repo contains runtime patches for the bundled `AutoClient.html` build without rebuilding/decompiling the huge embedded payload.

## Included patch

- `AutoClient.injector.html` loads the original `AutoClient.html`, injects a small script at runtime, and applies two fixes:
  - Prevents the Right Shift GUI hotkey from triggering while you are focused in text inputs/chat-like editable fields.
  - Mirrors lowercase single-key `keydown` events to uppercase equivalents (outside editable fields) so module keybinds like `X` reliably trigger.

## Usage

Open `AutoClient.injector.html` instead of `AutoClient.html`.
