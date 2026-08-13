[README.md](https://github.com/user-attachments/files/31046069/README.md)
# Kill Counter Overlay

A stream overlay (wins / losses counter) for OBS, controllable from a Stream Deck.

## Host on GitHub Pages
1. Create a new repository and upload the contents of this folder (`index.html`).
2. Go to **Settings -> Pages**, set Source to the `main` branch, folder `/ (root)`, Save.
3. Your overlay will be live at `https://<username>.github.io/<repo>/`.

## Add to OBS
- Add a **Browser** source, paste your GitHub Pages URL (or use Local File with `index.html`).
- Size: 520 x 360. Uncheck "Shutdown source when not visible".

## Controls (Stream Deck -> System -> Hotkey)
| Action | Keys |
| --- | --- |
| Win +1 | F13, 1, K, Up, + |
| Win -1 | F14, 2, J, Down, - |
| Loss +1 | F15, 3, D, Right, ] |
| Loss -1 | F16, 4, F, Left, [ |
| Reset | F17, 0, R |

You can also click a number to add and right-click to subtract.

## Change the look (in your browser)
Open the overlay in a normal browser tab and press the **` (backtick)** key to open the
settings panel. Adjust background, pill colour/gradient, lava lamp, and text colours —
changes apply live and are saved in that browser (localStorage). Press ` again to hide it.

The panel never shows in OBS (OBS doesn't send key presses to the source), so your overlay
stays clean. Set the look once in your browser; OBS picks up the same saved style.

Note: a Browser Source only receives key presses while focused - click **Interact** on the
source once, or capture a real browser window instead.

Counts and style are saved per-browser and survive restarts.
