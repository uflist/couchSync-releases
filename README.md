<p align="center">
  <img src="https://raw.githubusercontent.com/uflist/couchSync-releases/main/couchsync-banner.svg" alt="couchSync — synced watch parties for Stremio" width="100%">
</p>

<p align="center">
  <a href="https://github.com/uflist/couchSync-releases/releases/latest"><img alt="Latest version" src="https://img.shields.io/github/v/release/uflist/couchSync-releases?include_prereleases&sort=semver&style=for-the-badge&label=version&color=e9a85f&labelColor=2a221c&cacheSeconds=3600"></a>
  <a href="https://github.com/uflist/couchSync-releases/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/uflist/couchSync-releases/total?style=for-the-badge&label=downloads&color=d7774f&labelColor=2a221c"></a>
  <img alt="Windows" src="https://img.shields.io/badge/Windows-10%20%7C%2011-f2e6d8?style=for-the-badge&logo=windows&logoColor=f2e6d8&labelColor=2a221c">
</p>

<p align="center">
  <b>Watch movies and shows with your friends, in sync, everyone in original quality.</b><br>
  Discord is just for talking — no more blurry screenshare. 🍿
</p>

---

## 🛋️ How it works

One person is the **host** 👑: they pick what to watch and control play, pause and seeking. Everyone else plays the **same video on their own PC** through their own Stremio, and couchSync keeps everyone on the same second. If someone is still loading, the room waits for them.

**Everyone needs:** [Stremio](https://www.stremio.com/) desktop **open** · [Radmin VPN](https://www.radmin-vpn.com/) connected to the group's network.

## 👥 Joining a room

Nothing to download. Open the link the host sent you (`http://26.x.x.x:8000`) in Chrome or Edge and click **Join**. The first time, the browser warns that the connection isn't private (the room uses a homemade certificate): click **Advanced → Continue**. If it asks to access apps on this device or the local network, click **Allow** (that's your Stremio). Pick a name and you're in.

## 👑 Hosting a room

1. Download **`couchSync-vX.Y.Z.exe`** from the [latest release](https://github.com/uflist/couchSync-releases/releases/latest) and put it in its own folder.
2. Double-click it. The couchSync window opens, along with your browser at `http://localhost:8000`.
3. Copy the friends' link from the window and send it on Discord.
4. To shut down, close the window.

> [!IMPORTANT]
> **First run only:** if Windows says *"Windows protected your PC"*, click **More info → Run anyway** (the app just isn't code-signed). When the firewall asks, click **Allow** for private networks, otherwise your friends can't connect.

**Real-Debrid (optional):** click **Real-Debrid** in the window, paste your [API token](https://real-debrid.com/apitoken) and save. Without it, you watch via torrent like everyone else. The key stays in `couchSync.env` next to the `.exe` and is **never shared** with your friends.

**Updating:** when a new version is out, the entry screen tells you. Download the new `.exe` into the same folder and delete the old one — your settings stay. Only the host ever needs to update.

---

## ✨ Features

- 🎮 **Real sync** — the host's play, pause and seek reach everyone; automatic pause while anyone is buffering
- 🍿 **Browse & search** — Cinemeta catalogs, episodes, torrent list with quality and seeders
- 🗳️ **Suggestions with votes** — anyone can suggest, everyone votes, the host decides
- 💬 **Your own subtitles** — OpenSubtitles or embedded, with your own language, size, style and delay
- 📺 **Binge mode** — "Up next" and auto-advance between episodes
- 🐢 **Dead or slow torrent?** The host swaps it in one click
- 🔁 **Refresh-proof** — hit F5 and you're back at the same second
- 🛋️ **The couch** — see who's in the room, with avatars and loading progress; click someone to hand them the crown 👑

| Key | Action |
|:---:|---|
| <kbd>F</kbd> · <kbd>C</kbd> · <kbd>M</kbd> | Fullscreen · subtitles & audio · mute |
| <kbd>↑</kbd> <kbd>↓</kbd> | Volume |
| <kbd>Space</kbd> · <kbd>←</kbd> <kbd>→</kbd> | Play/pause · ±10 s *(host only)* |

---

## 🩺 Troubleshooting

<details>
<summary><b>Friends can't open the link</b></summary>

Make sure everyone is on the same Radmin VPN network, that you allowed couchSync through the firewall (*Windows Security → Firewall → Allow an app*), and that you sent the link from the window — not `localhost`.
</details>

<details>
<summary><b>Clicking Join downloads a <code>.htm</code> file</b></summary>

The host is on version 0.2.1 or older, which joined through Stremio's proxy — Stremio's latest update turned that off. The **host** needs to update to 0.3.0 or newer; guests don't need to do anything.
</details>

<details>
<summary><b>"Your connection isn't private" when joining</b></summary>

Expected: the room uses a homemade certificate (it only travels inside your Radmin network). Click **Advanced → Continue** (or **Proceed**). You only need to do it once per host.
</details>

<details>
<summary><b>"Stremio is not open" warning</b></summary>

Open the Stremio **desktop** app (the web version isn't enough) and keep it running. Everyone needs their own.
</details>

<details>
<summary><b>The video never finishes loading</b></summary>

The torrent is probably dead or slow — the loading card will say so. The host can swap it for another one (or a lighter one).
</details>

<details>
<summary><b>As the host, things look wrong when I open the 26.x.x.x link</b></summary>

On your own PC always use `http://localhost:8000`; through the Radmin IP you're treated as a guest.
</details>

<details>
<summary><b>My antivirus deleted the .exe</b></summary>

A common false positive for unsigned apps. Restore it and add the couchSync folder to your antivirus exclusions.
</details>

---

<p align="center"><sub>made with love for GDC™ · made by <b>flist</b> 🛋️🍿</sub></p>
