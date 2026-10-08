# Credits

Diamond Linux is a recipe on top of other people's work. Thank you to all of them.

## The system

- **Debian** and its maintainers: the base system, the kernel, apt. https://www.debian.org
- **GNOME** and the GNOME Foundation: GNOME Shell 48, Mutter, GDM, Files, Console, Settings,
  Text Editor and the libadwaita apps. https://www.gnome.org
- **Dash to Dock** by Michele Gaio (micxgx) and contributors, GPL-2.0: the floating dock.
  https://micheleg.github.io/dash-to-dock/
- **AppIndicator support** (ubuntu-appindicators) by Marco Trevisan and contributors, GPL-2.0.
- **NetworkManager**, **PipeWire**, **Mesa** (virgl, Vulkan): the plumbing that makes a
  desktop in an egg work.

## Look

- **Papirus icon theme** by the Papirus Development Team, GPL-3.0. https://github.com/PapirusDevelopmentTeam/papirus-icon-theme
- **Inter** by Rasmus Andersson, SIL Open Font License. https://rsms.me/inter/
- **Noto** fonts by Google, SIL Open Font License.
- **Terminus** console font (used by the console eggs in the same family), SIL Open Font License.
- **Garuda Linux**: the layout of the GNOME edition, a floating dock under a clean top bar with
  a Welcome window on first login, is what Diamond set out to match. No Garuda files are used.
  https://garudalinux.org
- **Tux** by Larry Ewing and The GIMP; the flat version by the Linux Foundation. Wallpaper art
  only in earlier builds; kept in the repository as `tux.svg`.
- **The gem** (`diamond.svg`) was downloaded from SVG Repo (https://www.svgrepo.com). Its
  collection licence is being confirmed; if you are its author, please open an issue so we
  can credit you properly or replace it.
- The DIAMOND wordmark is set in Phosphate, an Apple system font; only the rendered image
  ships here.

## Apps that install at build time (not redistributed here)

- **Google Chrome** by Google. Downloaded from dl.google.com during the build, under Google's
  terms, which Chrome shows on first launch.
- **Claude Desktop** and **Claude Code** by Anthropic. Installed from Anthropic's apt
  repositories under Anthropic's terms.
- **ChatGPT** with **Codex**, and the **Codex CLI**, by OpenAI. Installed from OpenAI's
  package and npm under OpenAI's terms.
- **Node.js** from NodeSource, MIT.

## Trademarks

Debian, GNOME, Google Chrome, Claude, Anthropic, ChatGPT, Codex and OpenAI are trademarks of
their respective owners. The Claude and OpenAI marks appear inside the `claude-cli` and
`codex-cli` launcher icons only to identify which terminal starts which tool; they are not
covered by this repository's licence and remain their owners' property.

## EggRun

Diamond is built, packaged and delivered with **EggRun** (https://eggrun.ai) by Camouflage
Networks Inc.: the egg format, the Yolk hypervisor, the hub and the desktop app.
