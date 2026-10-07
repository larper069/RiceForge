# RiceForge

**Offline visual theme and config builder for Waybar and Wofi.**

RiceForge lets you design Waybar and Wofi themes visually, preview changes live, customize modules, generate real config files, and export everything without npm, Rust, a build step, accounts, telemetry, or internet access.

> One file. Open it. Start ricing.

---

## Features

### Waybar

- Live visual preview
- Left / center / right module zones
- Drag-and-drop module reordering
- Move modules between zones
- Module library
- Per-module styling overrides
- Top / bottom bar position
- Generated `config.jsonc`
- Generated `style.css`

Supported modules currently include:

- Hyprland workspaces
- Hyprland window title
- Clock
- Network
- Pulseaudio
- Battery
- CPU
- Memory
- Temperature
- Tray

### Wofi

- Live launcher preview
- Generated `config`
- Generated `style.css`
- Entry style controls
- Search field style controls
- Shared palette and geometry controls
- Multiple shape and visual modes

### Theme controls

- Background color
- Surface color
- Text color
- Accent color
- Border width
- Radius
- Gap
- Opacity
- Shadow styles
- Random palettes
- Local theme saving
- JSON theme export

### Style system

RiceForge includes multiple design families and lets you mix styles instead of being locked to a single preset.

Current styles include:

- Neo Brutal
- Floating
- Pill
- Sharp
- Notched
- Segmented
- Underline
- Frame

The style composer also lets you independently control:

- Outer bar style
- Module shape
- Active workspace style
- Clock style
- Shadow style
- Wofi entry style
- Wofi search style

### Per-module inspector

Waybar modules can override the global theme individually.

You can customize:

- Shape
- Background
- Text color
- Border color
- Border width
- Radius
- Horizontal padding
- Label / format text

Click a module in the layout editor to edit it.

`Shift + Click` removes it.

---

## Run

Clone the repository:

```bash
git clone https://github.com/larper069/RiceForge.git
cd RiceForge
```

You can open the file directly:

```bash
firefox index.html
```

For the most reliable browser behavior, run a tiny local server:

```bash
python3 -m http.server 8080
```

Then open:

```text
http://localhost:8080
```

---

## Export

### Waybar

Select **WAYBAR**, design your theme, and press **EXPORT**.

RiceForge generates:

```text
config.jsonc
style.css
```

Typical destination:

```text
~/.config/waybar/config.jsonc
~/.config/waybar/style.css
```

Restart Waybar after replacing your files.

Example:

```bash
pkill waybar
waybar &
```

### Wofi

Select **WOFI** and press **EXPORT**.

RiceForge generates:

```text
config
style.css
```

Typical destination:

```text
~/.config/wofi/config
~/.config/wofi/style.css
```

---

## Contributing

Contributions are welcome.

Good areas to contribute:

- presets
- Waybar modules
- Wofi layouts
- config generation
- accessibility
- UI improvements
- bug fixes
- additional compositor support

Keep the core lightweight and offline-first.

If a feature can work without adding a dependency, prefer that approach.

---

---

## Screenshots

![screenshot](ss/1.png)
![screenshot](ss/2.png)
![screenshot](ss/3.png)

```

