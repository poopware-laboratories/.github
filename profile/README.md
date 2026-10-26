<div align="center">

<img src="https://avatars.githubusercontent.com/u/342596611?s=200" width="120" alt="Poopware Laboratories logo">

# Poopware Laboratories

**LABORATORIES.**

*Serious software. Unserious names.*

Brazil &nbsp;·&nbsp; Est. October 2026 &nbsp;·&nbsp; 4 personnel &nbsp;·&nbsp; 0 lawsuits to date

</div>

---

## About the institution

Poopware Laboratories is an independent research facility founded on a single
hypothesis: a project can have a terrible name and still be good software.

We build terminal emulators, text editors and hardware tools for the kind of
person who reads benchmark tables for fun. Then we name them after poop, because
the board of directors was not consulted.

Every product leaving the Laboratories is held to the same internal standard. It
must be fast. It must be careful with your files and your terminal. And it must
be mildly embarrassing to recommend to a coworker.

## Product portfolio

| Product | Division | In one sentence | Built with | License |
|---|---|---|---|---|
| [**Poopterm**](https://github.com/poopware-laboratories/poopterm) | Terminal Emulation | A terminal that is anything but crap. | Rust | AGPL-3.0 |
| [**neocaca**](https://github.com/poopware-laboratories/neocaca) | Text Editing | A modal editor that types at 10,000 cursors without breaking a sweat. | Zig | AGPL-3.0 |
| [**SoC Genius**](https://github.com/poopware-laboratories/SoC-Genius) | Legacy Apple Archaeology | Tells your jailbroken iPhone what it's made of. | Objective-C | MIT |
| [**pooplabs-apt-repo**](https://github.com/poopware-laboratories/pooplabs-apt-repo) | Plumbing & Logistics | Where all of the above ends up. | Shell | |

### 💩 Poopterm

Our flagship. A fast, software-rendered terminal emulator for Linux, macOS and
FreeBSD, with its own escape-sequence parser, its own font engine and its own
image decoders, because borrowing someone else's felt unsanitary.

- Handles real-world output at **108 MB/s overall** on a low-power laptop CPU, images included
- Sixel and kitty graphics (animation too), the kitty keyboard protocol, SIMD parsing
- Tabs, 13 themes plus a custom one, wallpapers, shell integration for zsh, fish and bash
- On Linux, every tab's shell lives in its own cgroup, so one runaway program
  can't clog the rest of the system

Available via Homebrew, APT, RPM, a PKGBUILD, or a source build.
[Latest release →](https://github.com/poopware-laboratories/poopterm/releases/latest)

### 🧻 neocaca

*"Caca" is Portuguese for exactly what you think it is.*

A modern terminal code editor in Zig with Kakoune-style keys: select first, then
act. Multiple selections, regex search, undo, and atomic saves, so a crash never
eats your file.

- Draws its first frame in **3.4 ms** (the competition: 13.3 ms)
- Answers a keypress in **0.66 ms**
- Ships in ReleaseSafe with bounds checks on, and is still fast
- Pull requests must carry **three lines of tests for every line of code**. This
  is enforced by CI. HR has received complaints.

Early days: one file at a time, no syntax highlighting yet. The roadmap lives in
[`TODO.md`](https://github.com/poopware-laboratories/neocaca/blob/main/TODO.md),
and so do the benchmarks it loses.

### 🔬 SoC Genius

A hardware information app for jailbroken iPhone, iPad and iPod touch. Model, SoC,
core layout, GPU, process node, RAM, battery, thermals, live accelerometer.

- **Classic** build: ARMv7, iOS 6, for the 32-bit devices in your drawer
- **SoC Genius 64**: ARM64, profiled from the A7 up to the A17 Pro and the M2
- Comes with a CPU-Z Classic theme, for the nostalgic

Not affiliated with Apple. Apple has not been informed.

### 🚽 pooplabs-apt-repo

The Laboratories' distribution pipeline. A flat APT feed serving both Debian
packages and Cydia packages, rebuilt hourly and published to GitHub Pages.
It pulls the latest Poopterm release automatically.

```sh
# Debian / Ubuntu, or paste the URL into Cydia, Sileo or Zebra
https://poopware-laboratories.github.io/pooplabs-apt-repo/
```

## Corporate values

1. **Your files are safe.** Atomic saves, undo for everything, no truncation on crash.
2. **Untrusted input stays untrusted.** Opening a file should never be able to attack your terminal.
3. **Benchmarks or it didn't happen.** We publish our numbers, including the ones we lose.
4. **Tests first.** The test suite is the only employee who has never been late.
5. **The name stays.** This has been raised in several meetings. The name stays.

## Personnel

<p>
  <a href="https://github.com/vx9k"><img src="https://github.com/vx9k.png?size=96" width="48" alt="vx9k"></a>
  <a href="https://github.com/vgs499p"><img src="https://github.com/vgs499p.png?size=96" width="48" alt="vgs499p"></a>
  <a href="https://github.com/meowzerskittycat"><img src="https://github.com/meowzerskittycat.png?size=96" width="48" alt="meowzerskittycat"></a>
  <a href="https://github.com/flowatach"><img src="https://github.com/flowatach.png?size=96" width="48" alt="flowatach"></a>
</p>

Open positions: none. Unpaid internships: technically all of them.

## Doing business with us

- **Found a bug?** Open an issue on the relevant repository. We take crap reports seriously.
- **Want to help?** neocaca's [issues](https://github.com/poopware-laboratories/neocaca/issues) are open for pickup. Bring tests. Three times as many as you think.
- **Found a vulnerability?** Please don't open a public issue. Poopterm and neocaca each have a `SECURITY.md` explaining how to report it.

---

<div align="center">
<sub>
Poopware Laboratories is not affiliated with Apple, any plumbing company, or good taste.<br>
Some rights reserved; see each repository's LICENSE.
</sub>
</div>
