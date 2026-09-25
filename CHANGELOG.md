# MOTO-HUB Studio — release notes

MOTO-HUB Studio is in private beta: these are notes only, with no packages. Ask for the beta on [Discord](https://discord.gg/FzhXZtPhC8).

## 1.12.0

_Released 23 September 2026._

### Maps
- Studio's maps are now **MapLibre**, the same engine the phone draws with, in MOTO-HUB's own day style. Follow and heading-up now look right, and a replay shows a real map between a dashboard's two layers.
- The map has a camera: zoom follows the pointer and keeps the pan, the track can be clicked to move the shared cursor and hovered to read the moment under it, and the replay can chase the rider with the way ahead up.

### Replay
- **A ride plays on a real dashboard:** pick one of your dashboards from a gallery of pictures and watch it run on the ride's own data.
- The phone's three 3D views are offered with the phone's own numbers.
- The panel says when the OBD adapter was not delivering, and jumps to where the data resumes.

### Trips
- Overview gets the map room it was missing, months are named under their bars, corners say when they are still being detected, and times use one clock format everywhere.

### Windows
- The Windows package now bundles a newer Java.

## 1.9.0

_Released 22 September 2026 · thirty new features in one release._

### The editor explains itself
- Every element, property, signal and action has an **info card**: what it is, when to use it, a concrete example and the pitfall to avoid. Read it on hover, in the **Info** tab, or in **What's this?** mode.
- A **command palette** (`Cmd+K`) reaches every command by name.
- **What's new** appears after an update.

### Dashboards
- A colour picker wherever a colour is set, multiple selection with align, spacing and move together, moving elements in and out of containers, locking, an image manager and colour replace.
- **States:** the whole dashboard drawn in every state at once (day and night, with and without engine data, navigating or not, values at their extremes) in every layout.
- **Parts:** save a selection as a named component, place it anywhere, and update every copy when you improve it.
- **Keep the layouts in step:** carry colour, font, signal and condition changes from the base layout to the variants, while position and size stay where each variant put them.
- **Play a ride:** a real ride can drive the editor's preview instead of made-up values.

### Trips
- Sync now runs **both ways**, field by field, with deletions through a trash.
- **Edit** rides: remove points, split and join rides, trim the sensor log with them. The changes travel back to the phone.
- **Roads:** corners found in every ride and matched across your library, and timed segments.
- Export tracks as GPX and KML, a **heat map** of your library, and **your dashboard drawn over your own video footage**.

### Simulator: a test bench
- Motorcycle profiles set the screen and the T-Box together and describe what is known to go wrong on each model.
- **Break it on purpose:** dropped packets, latency, a link that goes down, injected on demand.
- **Do it again:** sessions of touches and handlebar gestures recorded and replayed with checks.
- One button records the phone's screen, the simulated TFT, the phone's log and Studio's log into one file, on one timeline.

### Phone
- Once paired, the Phone workspace shows the phone: its dashboards (**Open here** pulls one into the editor), its modules, the computers allowed to read its rides, a **backup** of the whole app, and the health of the link.

## 1.3.4

_Released 21 September 2026._

### AI assistant
- **Save and connect** asks the endpoint which models it can run and fills a list to choose from. No more typing a model name from memory.
- The API key field keeps only the key, even when a whole code snippet from a provider's page is pasted into it, and a key is never shown back on screen.

## 1.3.3

_Released 21 September 2026._

### Android, a new workspace
- Your phone on the desk, through `adb` and `scrcpy`: the attached devices appear and disappear as you plug and unplug them.
- **Mirroring** opens scrcpy's own windows, one per device and mode, listed so a window hidden behind Studio can be brought back; settings per device and reusable profiles.
- **Wireless pairing** from a QR code, without reading addresses off the phone.
- **A remote control:** click, drag and type on the phone's snapshot, plus buttons for power, wake, home, back, recents, volume and more. It works even with the phone's screen off.

## 1.3.2

_Released 20 September 2026._

### Phone, a workspace of its own
- Finding and pairing the phone moves out of the inspector into a page of its own, **first in the rail**: the phones on this Wi-Fi on one side, the pairing code, the address and what the phone reports on the other.
- The address is always visible, an empty state explains in three steps how to turn the link on, and a phone can be forgotten.
- The inspector keeps what belongs to the dashboard: the tab is now called **Send**, with sending and the live preview.
- A first launch with no phone paired opens on the Phone workspace.

### Trips
- The first-sync guide is shorter: its first step now simply opens the Phone workspace and ticks itself off when the phone answers.

## 1.3.1

_Released 20 September 2026._

### A window for every workspace
- Any workspace can be pulled out into a window of its own, from the button in the corner of its rail entry or from the new **Window** menu, and put back by closing that window.
- Nothing is drawn twice: the rail raises the detached window instead, and a workspace that changes window keeps its view: zoom, conversation, open ride, simulator drawers.
- Handy with two screens: the dashboard on one, the simulator playing it on the other.

## 1.3.0

_Released 20 September 2026._

### Studio updates itself
- Studio now checks for new versions, shows what changed, and installs the update with one button, on macOS and on Windows. Every download is checked (size and SHA-256) before anything is replaced.
- Where Studio is not allowed to replace itself (a machine-wide install, a folder that is not yours), it says so and opens the download page instead.
- The version is shown in the **Help** menu.

### A workspace rail
- The workspaces move to a rail down the left edge, one entry each, with `Cmd+1`, `Cmd+2`, `Cmd+3`.

### The T-Box simulator, inside the window
- A simulated motorcycle TFT that MOTO-HUB pairs with like a real bike. Studio draws the TFT itself; clicks on it are touches, and the handlebar sits underneath (arrow keys and Enter work too).
- The pairing QR carries your Wi-Fi password, so it now starts covered and can be revealed when needed, handy for screen recordings.
- The simulator also runs from the installed app, not only from a development build.

## 1.2.0

_Released 18 September 2026 · the first version named **MOTO-HUB Studio**._

### Trips, a new workspace
- **Sync finished rides from the phone** and study them on the computer. The phone asks you to allow the computer first; allowed computers are listed in the app's settings.
- A first-sync guide, then five pages over your ride library: **Ride**, **Overview**, **Engine**, **Replay** and **Compare**.
- Map tiles, channel charts, and panels you can resize and close.

## 1.0.0

_Released 17 September 2026 · the first version, then called **Dashboard Editor**._

The first desktop editor for MOTO-HUB dashboards, for macOS and Windows.

### Dashboards
- A canvas with selection, move and resize handles, a grid, edge snapping with guides, pan and zoom.
- The full element catalogue in a palette, layers in drawing order, and an inspector built from each element's own properties.
- Dashboard settings: TFT presets and fit, layouts for other screens, requirements, handlebar bindings and theme colours.
- Test values to see warning colours and conditions without a ride.
- Undo and redo, copy and paste through the system clipboard, alignment tools, recent files.
- Templates: the classic MOTO-HUB dashboards, broken into elements you can edit, and **Break into elements** for any classic block.
- Image elements show their picture on the canvas and in the saved preview, exactly as the phone draws them.

### Phone
- Finds phones with the editor link turned on, remembers the pairing code of each one, sends the dashboard and shows a live preview drawn by the phone itself.

### AI assistant
- An OpenAI-compatible endpoint can build and change the dashboard with the editor's own tools, as one undo step per request.
