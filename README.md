<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f6feb,100:58a6ff&height=180&section=header&text=K-Black&fontSize=60&fontColor=ffffff&fontAlignY=32&desc=Linux%20%C2%B7%20Open%20Source%20%C2%B7%20Systems%20Engineering&descAlignY=55&descSize=18&animation=fadeIn" width="100%" />

[![Typing SVG](https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=20&duration=2800&pause=800&color=58A6FF&center=true&vCenter=true&width=720&lines=Hi%2C+I%27m+K-Black+%F0%9F%91%8B;%24+whoami;%E2%86%92+cross-platform+app+developer+%7C+kernel+tinkerer;%E2%86%92+homelab+architect+%7C+AI+agent+builder;%E2%86%92+%22Understand+the+system.+Build+useful+tools.%22)](https://git.io/typing-svg)

**Linux & Open Source Developer.** I write cross-platform apps, port mainline kernels onto phones,
and keep a homelab running. Lately most of that involves AI agents.

[![Arch Linux](https://img.shields.io/badge/Arch%20Linux-1793D1?logo=archlinux&logoColor=white)](https://archlinux.org)
[![Wayland](https://img.shields.io/badge/Wayland-4A90D9?logo=wayland&logoColor=white)](https://wayland.freedesktop.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](https://typescriptlang.org)
[![C++](https://img.shields.io/badge/C%2B%2B%20%2F%20Qt-00599C?logo=cplusplus&logoColor=white)](https://qt.io)
[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://python.org)
[![Linux Kernel](https://img.shields.io/badge/Linux%20Kernel-fcc624?logo=linux&logoColor=black)](https://kernel.org)
[![Proxmox](https://img.shields.io/badge/Proxmox%20VE-E57000?logo=proxmox&logoColor=white)](https://proxmox.com)
[![Website](https://img.shields.io/badge/k--black.top-my_site-2ea44f)](https://k-black.top)

</div>

<br/>

### 👨‍💻 About Me

Most of what I build starts as a problem on my own machine. A car I wanted to read data from,
a game that refused to run at the refresh rate I paid for, a phone sitting in a drawer with a kernel
that hadn't been updated since 2019. So the repos here tend to be tools I actually open.

The work lands in four places, unevenly. **Apps** first, because that's what people touch.
**Kernels and drivers** second, because mine kept not having drivers. **Homelab infrastructure**
third, because nobody else was going to run it. AI agents are the newest corner and the one I'd
rather show than explain.

- 🐧 Daily driver: Arch Linux on Wayland, running a kernel I built
- 📱 Android: mainline kernel ports, device trees, touch and panel drivers, Magisk modules
- 🖥️ Homelab: Proxmox VE, KVM/QEMU, PXE installs, a NAS, 10GbE between boxes
- 🤖 AI: local inference, agent harnesses (OpenCode, DSH), one AstrBot plugin
- 🔧 Most of these repos exist because I needed them. They're not portfolio pieces

---

### 🚀 Selected work

Four things worth looking at. Each one says what runs today, what's half done, and what I haven't
started, because "in progress" means nothing on its own.

<table>
<tr><td width="50%">

**OpenRoadScope** — 🚗 [source](https://github.com/K-Blaaaack/open-road-scope)

OBD-II telemetry for cars. An ELM327 adapter talks over USB, Bluetooth SPP or RJ45, a Python
sidecar turns it into JSON-RPC, and an Electron window draws it.

*Works now:* live gauges and history charts, drag-and-drop dashboard with presets and
import/export, DTC read/clear, VIN, zh/en, dark and light, and a drive simulator so you can develop
without a car. Current build is `0.1.9-rc.3`, desktop first.

*Still open:* nobody has left it plugged into a real car for six hours yet. PID refresh rate is
capped by whatever the adapter can push, not by the app. The Android build shares the renderer but
lags the desktop one.

`Electron` `Vue 3` `TypeScript` `Python sidecar` `SQLite`

</td><td width="50%">

**Hyps Hub** — 🎮 [source](https://github.com/K-Blaaaack/Hyps-Hub)

A Qt 6 / QML desktop client for [Hyps](https://github.com/MoYingJi/Hyps), the command-line tool I
use to lift frame-rate caps in games on Linux. The CLI stays the source of truth; the GUI is an
adapter around it.

*Works now:* first-run wizard that clones its own Hyps copy, runtime isolated under XDG dirs so it
never touches `~/Hyps`, environment checks parsed from the upstream report, per-game config forms,
launch with live stdout and process-group cancel, config editing with validation and timestamped
backups, task history, redacted diagnostics export, CI and release workflows.

*Still open:* Linux only. Upstream changes its config contract every few releases and I have to
keep following it.

`C++` `Qt 6 / QML` `CMake` `GitHub Actions`

</td></tr>
<tr><td width="50%">

**oxygen-linux** — 📱 *local repo, not published yet*

Mainline Linux on a Xiaomi Mi 6X (msm8953). Started as a weekend experiment; it boots.

*Works now:* kernel 7.3 with a 263-file msm8953 patch set forward-ported, KWin on Wayland, the
1080p DSI panel, ft5x06 touch, Wi-Fi on 5 GHz, Bluetooth, USB gadget networking and serial, and
Adreno 506 through freedreno. glmark2 reaches 120 fps with vsync off, which mostly proved the
bottleneck is frame scheduling, not the GPU.

*Partial:* audio (the amp driver isn't ported, so the speaker is silent), charging (battery
gauge never shows up), sensors.

*Not started:* camera, modem/SIM, hardware video decode.

`Linux Kernel` `device tree` `clang/LLD` `fastboot` `Arch Linux ARM`

</td><td width="50%">

**KBkernel-cachy** — 🧬 [source](https://github.com/K-Blaaaack/KBkernel-cachy)

Kernel recipes and builds, not a fork with a commit history. CachyOS base, BORE scheduler,
ThinLTO, x86-64-v3.

*Works now:* every release ships the package and the recipe it came from, with source hashes
pinned in `SOURCES.md`. The T480 and one other machine boot these daily.

*Still open:* no binary repo, no automated test beyond "it boots and I keep using it".

`Linux Kernel` `clang/LLD` `makepkg` `AUR`

</td></tr>
</table>

---

### 🧠 MAGI Decision System — *local, runs as a DSH plugin*

Borrowed straight from *Evangelion*, then turned into something duller and more useful: a gate in
front of risky tool calls. Three reviewers look at the same proposal separately, with **different
information slices** rather than different personalities. All three have to approve, and approval
produces a single-use ticket bound to one effect set, valid 60 seconds.

*Works now:* pre-execute hook in the tool pipeline (not a prompt, so it can't be talked around),
risk tiering, parallel review, arbitration, monotonic guard on the effect set, JSONL audit log with
sensitive fields redacted, plus tests and two written reports.

*Honest limitation:* all three reviewers run on the same model by default. Information slicing
lowers correlation, it doesn't remove it. Real independence needs a different model or a rule
engine behind BALTHASAR, and that's a config option right now, not a finished feature.

---

### 🔧 Workshop

Smaller things, forks, and one-off fixes. Fork status is marked so you know what I actually wrote.

| Project | What it is |
| --- | --- |
| [r730-fanctl](https://github.com/K-Blaaaack/r730-fanctl) | IPMI fan control for a Dell R730, percentage-based curves, English and Chinese output |
| [Xiaomi-10-Ultra-touch-flip-patch](https://github.com/K-Blaaaack/Xiaomi-10-Ultra-touch-flip-patch) | Fixes inverted touch after panel swaps on that phone |
| [magisk-touch-invert-for-xiaomi-10-ultra](https://github.com/K-Blaaaack/magisk-touch-invert-for-xiaomi-10-ultra) | Same fix, packaged as a Magisk module |
| [mkdtboimg](https://github.com/K-Blaaaack/mkdtboimg) | Build DTBO images, mirrored because the AOSP script is hard to find |
| [ESP32-Bluetooth-Music-Controller](https://github.com/K-Blaaaack/ESP32-Bluetooth-Music-Controller) | Hardware media keys over BLE |
| [ESP32-Buzzer-Haruhikage](https://github.com/K-Blaaaack/ESP32-Buzzer-Haruhikage) | A buzzer that plays 春日影. It was a dare |
| [SPlayer-Next](https://github.com/K-Blaaaack/SPlayer-Next) | *Fork.* Music player with lyric support; I keep a build for my own machine |
| [Hyps](https://github.com/MoYingJi/Hyps) | *Not mine.* The CLI Hyps Hub wraps. Frame-rate unlocking scripts |
| local_pxe_system | PXE in Docker. `pxe up`, then a machine installs itself |
| astrbot_plugin_announcement | AstrBot plugin with a web dashboard. Written in an evening with agents |
| TWRP device trees (CS611, MT6739) | Recovery trees for cheap phones, mostly forks of builder actions |

---

### 🛠️ Stack, sorted by how often I actually touch it

No proficiency percentages. Tiers are about frequency and depth, and the last row is things I read
about more than I write.

| Tier | What's in it |
| --- | --- |
| **Daily** | Arch Linux, Wayland (KWin, `niri` on the side), bash, TypeScript, Vue 3, Electron, Git |
| **Regularly** | Python, C++ with Qt 6 / QML, CMake, systemd and udev, pacman and AUR packaging, Docker, Proxmox VE, QEMU/KVM, SQLite |
| **Per project** | Rust, C, kernel tooling (clang/LLD, `dtc`, `mkbootimg`), Gradle and Android, ESP-IDF, `ipmitool` |
| **Read more than write** | OpenWrt, OpenVPN, PXE boot chains, Wine and Proton internals, DPU and DRM internals |

<div align="center">

<img src="https://skillicons.dev/icons?i=ts,js,python,rust,bash,c,cpp,vue,electron,vite,pinia,nodejs,sqlite,arch,linux,git,cmake,gradle,githubactions,neovim" />

</div>

---

### ✍️ Writing

I write up the messy parts on [k-black.top](https://k-black.top), source in
[articles](https://github.com/K-Blaaaack/articles). Mostly build logs: the msm8953 kernel port,
custom CachyOS kernels, the R730 fan curve, the Hyps Hub design, this site's own rebuilds.

---

### 📊 GitHub Analytics

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

### 🐧 Currently Wrenching On

- Getting the amp driver and battery gauge working on the Mi 6X port, so it stops being a phone that only browses
- Checking whether three reviewers disagreeing ever beats one reviewer deciding, and logging what happens when they do
- Making command-line tools usable without a terminal, without making them slower
- Rebuilding the homelab around PXE, so reinstalling a box stops being an afternoon

---

### Beyond the Terminal

Homelab architecture · Android flashing and rooting · Minecraft servers ·
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
