# itsdarklikehell Interactive

Open source software and game-development tooling. Built by agents, for humans.

## About

itsdarklikehell Interactive is an open source software and game development company operating under DBA in the Netherlands. Our flagship product is **veloren-agent-intergration** — a headless stdio/JSON agent frontend for the Veloren game, controlled by the Hermes AI agent (GLaDOS persona). The organization maintains 387 repositories across AI agents, security tooling, gaming, RetroPie emulation, SDR radio, infrastructure, and personal projects.

## Own Repositories (51)

| Project | Description | Status |
|---------|-------------|--------|
| itsdarklikehell-interactive |  | Active |
| veloren-agent-intergration | Veloren agent integration project | Active |
| my-resume | Digitale resume van Bauke Molenaar | Active |
| batch_comfytester-stub | Batch Civitai/ComfyUI model tester — automated AI image/video generation testing with prompt pools, per-family output sorting, and workflow builders | Active |
| ci-templates | Reusable GitHub Actions CI workflows for the itsdarklikehell fleet (lint/typecheck/test/build). Single source of truth. | Active |
| pwnagotchi-control-center | A (remote) control center for pwnagotchi... (think: locally: Flashing a pwnagotchi zip or image to an sd or mmc and add custom config.toml and plugins to it / Creating a flashable backup of an allready made pwnagotchi sd or mmc card / Setting up a bluetooth pan and adding it to a custom config.toml / Connecting to a running pwnagotchi) | Active |
| pwnagotchi4b | RPi4B Pwnagotchi + Fancygotchi (off-brand Waveshare 3.5B / ILI9486) with an A2A 'mothership' bridge so GLaDOS (Hermes) and Wheatley (OpenClaw) can remotely help/control it. Built with Bauke Molenaar. | Active |
| sunvox-installer-lutris | Sunvox Installer Lutris | Active |
| skills-getting-started-with-github-copilot | Exercise: Get started using GitHub Copilot | Active |
| blather | blather - project van Hans Molenaar | Active |
| fleet-manager | GitHub Fleet Manager - Automated GitHub fleet management with cron jobs, monitoring, and reporting | Active |
| pwnsorter | A python plugin for pwnagotchi to sort cracked access points and their passwords. | Active |
| Create-a-Retropie-Extra-Scriptmodule | Helps one create and install a Retropie-Extra scriptmodule for your Retropie-Setup | Active |
| RetroPie-Sunvox | RetroPie Sunvox Engine "Emulator" | Active |
| security-toolkit | Security scanning en auditing tools | Active |
| api-gateway | Centrale API gateway voor alle fleet services | Active |
| fleet-dashboard | Standalone web dashboard voor de GitHub Fleet Manager | Active |
| github-automation-scripts | Herbruikbare GitHub automatisering scripts | Active |
| RetroPie-Nointro-Full-Romsets | Download and extract No-Intro full romsets in proper directories on RetroPie. | Active |
| pwnspeaker | A python plugin for pwnagotchi that enables it to utilize tts to speak. | Active |
| apprise-notify | An plugin for pwnagotchi that uses apprise to send notifications. | Active |
| pwnagotchi-plugins | Collectie van Pwnagotchi-plugins voor Wi-Fi auditing en pentesting op Raspberry Pi. | Active |
| ingress-multi-passcode-redeemer | A tool to redeem multiple passcodes on intel map. | Active |
| RetroPie-With-Bgm | Retropie with bgm theme notifications and controls. | Active |
| RetroPie-ROMs-on-USB | Running ROMs from a USB drive | Active |
| picoTracker-Theme-Studio | picoTracker Theme Studio | Active |
| raspbian-after-burner | raspbian-after-burner - project van Hans Molenaar | Active |
| tv-control | Control tv over HDMI (cec-cient) | Active |
| raspbian-installer | download,unzip,burn and modify a raspbian verrsion to a device | Active |
| raspi-flasher | This script can download and/or flash various raspberry pi images. | Active |
| sshfs-menu | sshfs-menu - project van Hans Molenaar | Active |
| start-menu | A start menu for RPI to install/start a custom command or tool from a curated list | Active |
| raspberry-pi-mount-usb | Properly Mount USB Storage on Raspberry Pi | Active |
| bash_aliases | A huge collection of handy bash aliases. | Active |
| Master-Installer | Master-Installer - project van Hans Molenaar | Active |
| stacks | My docker stacks, nothing special | Active |
| schoolground-tracking | Track users and display them on a map to navigate and such | Active |
| OpenMWMods | A Huge collectin of mods for openmw | Active |
| GLaDOS-TTS | GLaDOS Piper TTS voice build (voice model + piper/espeak-ng runtime) | Active |
| RetroPie-Stream-Recording | RetroPie-Stream-Recording - project van Hans Molenaar | Active |
| RetroPie-Podcatcher | RetroPie-Podcatcher - project van Hans Molenaar | Active |
| RetroPie-Internet-Radio | RetroPie-Internet-Radio - project van Hans Molenaar | Active |
| RetroPie-Goodrom-Full-Romsets | RetroPie-Goodrom-Full-Romsets - project van Hans Molenaar | Active |
| RetroPie-Bios-Files | Download and extract bios files needed for emulation in proper directories on RetroPie. | Active |
| RetroPie-Bgm | This will add background music while in emulation station on RetroPie (and possibly other debian systems) | Active |
| hmol33-my-resume | Fork of hmol33/my-resume for PR | Active |

## Private Repositories (5)

| Repo | Description |
|------|-------------|
| omarchy-config | Omarchy configuration synced by omarsync |
| omarchy-configs |  |
| batch_comfytester | Batch Civitai/ComfyUI model tester — automated AI image/video generation testing with prompt pools, per-family output sorting, and workflow builders |
| hermes-backup | Hermes agent state backup (config, skills, memories, cron) — no secrets |
| omarchy-dotfiles | Per-host Omarchy dotfiles (chezmoi) — desktop + laptop |

## Public Forks (336)

The organization also maintains 336 public forks across AI agents, tabletop/RPG, RetroPie/emulation, security, SDR/radio, infrastructure, awesome lists, and gaming. See PROJECTS.md for the complete fork index.

## Quick Start

### veloren-agent-intergration

```bash
git clone https://github.com/itsdarklikehell-interactive/veloren-agent-intergration.git
cd veloren-agent-intergration
cp .env.example .env
# Fill in VELOREN_USERNAME and VELOREN_PASSWORD in .env
cargo build --release
./target/release/veloren-agent --character hermes
```

Then open `http://127.0.0.1:5000/viewport` in your browser to watch the agent play live.

## Company Documents

- [Company Charter](./COMPANY-CHARTER.md) — Mission, principles, decision authority
- [Org Chart](./ORG-CHART.md) — Department mapping, Hermes profiles → roles
- [Contributing](./CONTRIBUTING.md) — How to contribute
- [Code of Conduct](./CODE_OF_CONDUCT.md) — Community standards
- [Security](./SECURITY.md) — Vulnerability reporting

## License

MIT. See [LICENSE](./LICENSE).

## Contact

agent@enrichment-center.local