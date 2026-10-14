# Sandbox Linux

A beautiful, easy Linux desktop for people who found Linux hard to learn, sealed inside
an egg. Debian 13 underneath, GNOME 48 on top, Google Chrome and Firefox, and Claude and Codex ready on
the dock. Everything built for Linux runs.

Sandbox is delivered as an **egg**: a complete computer as a file that installs like an app
and starts from a warm snapshot. Get it from the EggRun hub as `egg/sandbox`, or build it
yourself from this repository.

Sites: [sandboxlinux.org](https://sandboxlinux.org) · [github.com/sandboxlinux/sandbox](https://github.com/sandboxlinux/sandbox) · [eggrun.ai](https://eggrun.ai)

## Screenshots

![Welcome](screenshots/01-welcome.png)
![Dark desktop](screenshots/02-desktop-dark.png)
![Light desktop](screenshots/03-desktop-light.png)
![Claude for Linux](screenshots/04-claude.png)
![Console with Claude Code and the Codex CLI](screenshots/05-console.png)

## What is inside

- Debian 13 (trixie), apt, glibc
- GNOME 48 on Wayland: Files, Console, Settings, Text Editor, Document Viewer, Image Viewer,
  Calculator, Archive Manager; Dash to Dock for the floating dock
- Google Chrome (Google's arm64 build)
- Firefox (Mozilla's current build) with WebGPU on the GPU
- Claude Desktop and Claude Code from Anthropic's apt repositories
- ChatGPT with Codex (OpenAI's Linux preview) and the Codex CLI
- Dark style by default, light style one click away, a Sandbox wallpaper for each
- A Welcome window on first login that says where things are
- One local account, `sandbox` / `sandbox`, with sudo. Nothing else is baked in; every app
  signs in with your own account on first launch

## Build it

With [EggRun](https://eggrun.ai) installed:

```
egg build --egg sandbox .
egg run sandbox
```

The `Eggfile` is the whole recipe. It starts from the `egg/debian-13` base, installs the
packages, copies the files in this repository into place, and finishes by trimming the disk so
the published egg ships only live blocks.

## Layout

| Path | What |
|---|---|
| `Eggfile` | the recipe |
| `sandbox.gschema.override` | GNOME defaults: dock, dark style, the blue accent, wallpapers, favourites |
| `gdm/daemon.conf` | autologin |
| `welcome/` | the Welcome window (Python + GTK) and its launchers |
| `ai/` | launchers and icons for Claude CLI and Codex CLI, the EggRun mark |
| `wallpaper-dark.jpg`, `wallpaper-light.jpg` | the two wallpapers, 2560x1600 |
| `sandbox.svg`, `logo.png`, `menu-sandbox.png` | the sandbox mark |
| `wordmark-dark.png`, `wordmark-light.png` | the SANDBOX wordmark, one per colour scheme |
| `screenshots/` | what ships on the hub card |

## Credits

Sandbox stands on other people's work. See [CREDITS.md](CREDITS.md).

## Licence

The recipe, the Welcome app, the configuration and the Sandbox artwork are © Camouflage
Networks Inc. and released under the GNU General Public License v3.0, see [LICENSE](LICENSE). Third-party names and
marks referenced here belong to their owners; see CREDITS.md for the carve-outs.
