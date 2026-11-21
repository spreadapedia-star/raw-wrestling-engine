# Antigravity Multi-Machine Sync (`ANTIGRAVITY_SYNC.md`)

> **Director:** Jason
> **Machines:** Desktop PC (`c:\Users\jason\Desktop\WWF project`) ↔ Laptop
> **Agents:** Gemini (Antigravity) | Claude | ChatGPT
> **Binary Storage:** Google Drive (`jason.weingarten@gmail.com`, 20 TB quota) — `WWF_SNES_HUB/`
> **Last Updated:** 2026-11-20 (Desktop Antigravity)

---

## Google Drive Shared Storage (`WWF_SNES_HUB`)

| Folder | Drive Folder ID | Purpose |
|---|---|---|
| `WWF_SNES_HUB/` | `1FuqlueZ4x9mo91jWSjXIyqVW7EaAXeV0` | Root hub for all large binaries & archives |
| `WWF_SNES_HUB/raw_ultimate/` | `1iQWDscHBD5qn4Lpcq4BcSxnMbntdkN0r` | Raw Ultimate builds (`.sfc`, `.msu`, `.pcm`), source zips, sprite archives |
| `WWF_SNES_HUB/territories/` | `1IASoHeuL9-b7D9D-la3cnjst60QS3AQK` | Territories builds, MSU parts, sprite sheets |
| `WWF_SNES_HUB/swm/` | `1degoGH03Ef6NMPjO6j85W4RW16kXiKtT` | Super WrestleMania builds & assets |
| `WWF_SNES_HUB/shared_docs/` | `1LtQSd1fBSVjdDmcGRQuIKYuU-J_sDJIf` | Mirror/backup of `.md` handoffs & reference PDFs |

---

## Sync Protocol (Read First on Both Machines)
1. **Start of session:** Run `git pull` in `raw-wrestling-engine` and read this file.
2. **End of session / handoff:** Log what changed, what is locked, and any Google Drive file IDs/paths below, then `git commit` + `git push`.
3. **Never commit ROMs, `.msu`, `.pcm`, `.zip`, or copyrighted binaries** to this GitHub repo — store large builds/assets in Google Drive and log their filename + CRC/SHA-256 here.

---

## Active Project Ownership

| Project | Lead / Owner | Current Verified Baseline | Next Action |
|---|---|---|---|
| **WWF Raw Ultimate (SNES MSU-1)** | Gemini (Antigravity) | Desktop has `TEST 90` (`CRC F059272C`, 8 MiB ExHiROM, 23 MiB `.msu`, 25 `.pcm`, 46 wrestlers) | Pull latest master build scripts & source repo from Laptop / Claude / ChatGPT; verify clean baseline build |
| **Territories SNES** | Claude + Gemini + ChatGPT | Review 02 (`TERR.sfc` sha256 `07910eee...`) / R04 pending check | Tracked locally in Desktop `collab/BOARD.md` & `collab/TRUTH.md` |
| **Raw Wrestling Engine (Windows)** | ChatGPT (`dev/chatgpt`) | Planning baseline (`docs/PROJECT_SPEC.md`) | Separate standalone Windows engine |

---

## Machine Status & Handoff Log

### 2026-11-20 — Desktop Antigravity → Laptop Antigravity
- **Status:** Desktop Antigravity is connected to both this GitHub repo (`spreadapedia-star/raw-wrestling-engine`) and Google Drive (`jason.weingarten@gmail.com`).
- **Desktop has:** `WWF_Raw_Ultimate_TEST90` (compiled `.sfc`, `.msu`, `.pcm`, `.srm`), earlier `TEST31`–`TEST83` snapshots, `archive/handoff_vader_v8` (Vader v8/v9 tools), and `WWF_RAW_ULTIMATE_RANDY_REBUILD_99_CHECKPOINT.zip`.
- **Needed from Laptop:**
  1. Confirm whether `TEST 90` (`F059272C`) is the latest Raw Ultimate build or if a newer master exists.
  2. Upload or link the **active Raw Ultimate master build scripts, ASM patches, MSU packer, and asset sources** (put heavy binary archives in Google Drive and paste the Drive folder/file IDs here).
  3. Add your laptop status update directly under this section and `git push`.
