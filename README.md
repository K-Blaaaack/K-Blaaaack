<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f6feb,100:58a6ff&height=180&section=header&text=K-Black&fontSize=60&fontColor=ffffff&fontAlignY=32&desc=Linux%20%C2%B7%20Open%20Source%20%C2%B7%20Systems%20Engineering&descAlignY=55&descSize=18&animation=fadeIn" width="100%" />

[![Typing SVG](https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=20&duration=2800&pause=800&color=58A6FF&center=true&vCenter=true&width=720&lines=Hi%2C+I%27m+K-Black+%F0%9F%91%8B;%24+whoami;%E2%86%92+cross-platform+app+developer+%7C+kernel+tinkerer;%E2%86%92+homelab+architect+%7C+AI+agent+builder;%E2%86%92+%22Understand+the+system.+Build+useful+tools.%22)](https://git.io/typing-svg)

**Linux & Open Source Developer.** I write cross-platform apps, port mainline kernels onto phones,
and keep a homelab running. Lately most of that involves AI agents.

[![Arch Linux](https://img.shields.io/badge/Arch%20Linux-1793D1?logo=archlinux&logoColor=white)](https://archlinux.org)
[![Wayland](https://img.shields.io/badge/Wayland-4A90D9?logo=wayland&logoColor=white)](https://wayland.freedesktop.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](https://typescriptlang.org)
[![Vue](https://img.shields.io/badge/Vue%203-4FC08D?logo=vuedotjs&logoColor=white)](https://vuejs.org)
[![Rust](https://img.shields.io/badge/Rust-000000?logo=rust&logoColor=white)](https://rust-lang.org)
[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://python.org)
[![Qt](https://img.shields.io/badge/Qt%2FQML-41CD52?logo=qt&logoColor=white)](https://qt.io)
[![Proxmox](https://img.shields.io/badge/Proxmox%20VE-E57000?logo=proxmox&logoColor=white)](https://proxmox.com)
[![Website](https://img.shields.io/badge/k--black.top-my_site-2ea44f)](https://k-black.top)

</div>

<br/>

### 👨‍💻 About Me

Most of what I build starts as a problem on my own machine. A car I wanted to read data from,
a game that refused to run at the refresh rate I paid for, a server I wanted to reinstall without
walking to the basement. So the projects here tend to be tools I actually open.

The work lands in three places, unevenly. **Apps** first, because that's what people touch.
**Kernels and drivers** next, because mine keep not having drivers. **Infrastructure** last, because
nobody else was going to run it. AI agents are the newest corner and the one I'd rather show than
explain.

- 🐧 Daily driver: Arch Linux on Wayland (`niri`), running a kernel I built
- 📱 Android: mainline kernel ports, device trees, touch and display drivers, Magisk
- 🖥️ Homelab: Proxmox VE, KVM/QEMU, PXE installs, a NAS, 10GbE between boxes, some soft routing
- 🤖 AI: local inference, agent harnesses like OpenCode and DSH, a couple of AstrBot plugins
- 🔧 Several repos here exist only because I needed them. None of them are portfolio pieces

---

### 🚀 Projects

<table>
<tr><td width="60%">

**[OpenRoadScope](https://github.com/K-Blaaaack/open-road-scope)** — 🚗 *active development*

Reads OBD-II from the car, draws the numbers live, logs the trips.

`Electron` `Vue 3` `TypeScript` `PixiJS` `Rust/NAPI-RS` `SQLite`

</td><td width="40%">

**[SPlayer-Next](https://github.com/K-Blaaaack/SPlayer-Next)** — 🎵 *public project*

A music player I wanted on Linux, with more than one place to pull tracks from.

`Vue` `Electron` `TypeScript`

</td></tr>
<tr><td width="60%">

**[Hyps](https://github.com/MoYingJi/Hyps) / Hyps Hub** — 🎮 *daily driver*

A CLI that lifts frame-rate caps in games on Linux (Genshin, ZZZ). **Hyps Hub** is the GUI I wrote
around it later, in Qt6/QML. It talks to the CLI through an adapter layer so the two can move
independently, which has already saved me from rewriting things twice.

`C` `Bash` `Qt6/QML`

</td><td width="40%">

**[KBkernel-cachy](https://github.com/K-Blaaaack/KBkernel-cachy)** — 🧬 *system*

CachyOS-based kernels I build for my own laptops, tuned per machine. The T480 gets most of the attention.

`Linux Kernel` `GCC` `Pacman/AUR`

</td></tr>
<tr><td width="60%">

**MAGI Decision System** — 🤖 *experimental*

Stolen straight from *Evangelion*. Three agents look at a proposal separately and in parallel.
All three have to agree. If one refuses, the system is supposed to draft a compromise and send it
back around. Whether that actually converges is the open question I'm still poking at.

`Python` `LLM agents`

</td><td width="40%">

**[articles](https://github.com/K-Blaaaack/articles) + [my-homepage](https://github.com/K-Blaaaack/my-homepage)** — 📝 *live*

[k-black.top](https://k-black.top) and the content behind it. Own build pipeline, light and dark
themes, English and Chinese.

`Node.js` `Vite` `CI`

</td></tr>
</table>

<details>
<summary><b>🧰 Workshop shelf (smaller stuff)</b></summary>
<br/>

| Project | What it does |
| --- | --- |
| [oxygen-linux] | Getting mainline Linux to boot on an msm8953 phone. Kernel 7.x, device tree, touch and panel drivers |
| local_pxe_system | PXE in Docker. `pxe up`, then a machine installs itself |
| astrbot_plugin_announcement | AstrBot plugin with a web dashboard for managing announcements. I wrote it in one evening with agents |
| Monster-Siren downloader | Pulls the Arknights soundtrack down locally |
| bili tooling | Small scripts that automate bits of Bilibili |

</details>

<br/>

## 📊 GitHub Analytics

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=K-Blaaaack&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=1f6feb&text_color=c9d1d9&ring_color=1f6feb" />
  <img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=K-Blaaaack&theme=github-dark-blue&hide_border=true&background=0D1117&ring=1F6FEB&fire=58A6FF&currStreakLabel=58A6FF" />
  <br/>
  <img width="370" src="https://github-readme-stats.vercel.app/api/top-langs/?username=K-Blaaaack&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&langs_count=8" />
  <br/><br/>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/K-Blaaaack/K-Blaaaack/output/github-contribution-grid-snake-dark.svg" />
    <img width="95%" alt="snake animation" src="https://raw.githubusercontent.com/K-Blaaaack/K-Blaaaack/output/github-contribution-grid-snake.svg" />
  </picture>
</div>

<br/>

## 🛠️ Arsenal

<div align="center">

<img src="https://skillicons.dev/icons?i=ts,js,python,rust,bash,c,cpp,qml&theme=dark" /><br/>
<img src="https://skillicons.dev/icons?i=vue,electron,vite,pinia,nodejs,sqlite&theme=dark" /><br/>
<img src="https://skillicons.dev/icons?i=arch,linux,kubernetes,docker,nginx,git&theme=dark" /><br/>
<img src="https://skillicons.dev/icons?i=gradle,githubactions,vscode,neovim,idea,raspberrypi&theme=dark" />

</div>

<table>
<tr><th>Domain</th><th>Tooling</th></tr>
<tr><td><b>🐧 Systems</b></td><td>Arch Linux · Linux Kernel · Wayland / <code>niri</code> · systemd / udev · Android · Device Tree · Magisk · Wine / Proton / Waydroid</td></tr>
<tr><td><b>🌐 Infra</b></td><td>Proxmox VE · KVM/QEMU · Docker · PXE · OpenWrt · iKuai · OpenVPN · NAS · 10/40GbE fabric</td></tr>
<tr><td><b>🤖 AI</b></td><td>Local LLM inference · OpenCode / DSH agent harnesses · AstrBot · multi-agent orchestration</td></tr>
</table>

<br/>

### 🛠️ Tech Stack

<table>
<tr><th width="25%">Languages</th><th width="25%">App & Desktop</th><th width="25%">Systems</th><th width="25%">Infra & AI</th></tr>
<tr><td>

TypeScript · JavaScript
Python · Rust
Bash · C / C++
QML

</td><td>

Vue 3 · Pinia · UnoCSS
Electron · Vite · Capacitor
Qt6/QML · PixiJS
Node.js · Hono · WebSocket
SQLite · NAPI-RS

</td><td>

Arch Linux · Linux Kernel
Wayland · niri · systemd · udev
Android · Device Tree · Magisk
Wine · Proton · Waydroid

</td><td>

Proxmox VE · KVM/QEMU · Docker
OpenWrt · iKuai · OpenVPN
PXE · NAS · Self-hosting · 10/40GbE
OpenCode · AstrBot · Local LLMs
Multi-agent systems

</td></tr>
</table>

<br/>

## 🐧 Currently Wrenching On

- Getting the display and touch panel alive on an old Snapdragon 625 phone (oxygen-linux). Neither works yet
- Figuring out whether three agents disagreeing can ever produce a better answer than one agent deciding (MAGI)
- Making command-line tools usable without a terminal, without making them slower
- Rebuilding the homelab around PXE, so reinstalling a box stops being an afternoon

---

### 🐧 Beyond the Terminal

Homelab architecture · Android flashing & rooting · Minecraft servers ·
anime & 二次元 · performance tuning · hardware DIY

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2" width="70%"/>

### 💭 Philosophy

> **Understand the system. Build useful tools. Keep experimenting.**

*Half of what I know came from breaking something in a VM and putting it back.*

<br/>

![Anime](https://img.shields.io/badge/-anime-ff69b4?style=flat-square&logo=sailpoint&logoColor=white)
![Minecraft](https://img.shields.io/badge/-Minecraft-62B47A?style=flat-square&logo=minecraft&logoColor=white)
![Homelab](https://img.shields.io/badge/-Homelab-1f6feb?style=flat-square&logo=proxmox&logoColor=white)
![Tinkering](https://img.shields.io/badge/-%E6%8A%98%E8%85%BE-58a6ff?style=flat-square)

<br/>

*This page is maintained by hand. The snake is the only thing on a schedule.*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:58a6ff,50:1f6feb,100:0d1117&height=120&section=footer" width="100%" />

</div>
