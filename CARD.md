# Diamond Linux

Hard like a diamond. A beautiful, easy Linux desktop for people who found Linux
hard to learn: GNOME with a floating dock, search from the top, Google Chrome,
Claude and Codex on the dock, and a Welcome window that says where things are. Debian 13 underneath, so
everything built for Linux runs.

## What's inside

- Debian 13 (trixie), apt, glibc
- GNOME 48 on Wayland: Files, Console, Settings, Text Editor, Document Viewer,
  Image Viewer, Calculator, Archive Manager
- Google Chrome (Google's own arm64 build)
- Claude Desktop (Anthropic's Linux beta) and Claude Code, from Anthropic's apt repositories
- ChatGPT with Codex (OpenAI's Linux preview) and the Codex CLI
- All four on the dock; each signs in on first launch with your own account
- Dark style by default with a light style one click away; a Diamond wallpaper
  for each
- Welcome: Chrome, Files, Terminal, Settings, Look & feel, eggrun.ai, Docs, Learn
- Signs you in as `diamond` (password `diamond`) with sudo
- **No credentials baked in** beyond that local desktop account

## Resources

| | |
|---|---|
| Class | M |
| CPUs | 4 |
| RAM | 8G |
| Disk | 32G |
| GPU | virgl, 2G |
| Display | 1280x800 at 2x |
| Network | restricted |
| Licence | EggRun EULA |

## First run

Double-click the icon. From a terminal: `egg run egg/diamond`.
The desktop appears with the Welcome window; press Let's go and it will not
return. Chrome shows Google's terms on its first launch.

## Sites

diamondlinux.org · eggrun.ai
