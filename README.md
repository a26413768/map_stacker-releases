# MapStacker

**行星／月面影像疊合工具** — 免安裝 Python，下載對應平台的壓縮檔，解壓後即可執行。
支援 Windows、macOS、Linux。

**Lunar &amp; planetary image stacking tool** for lucky imaging — a free,
lightweight, cross-platform alternative to AutoStakkert!3, RegiStax and
PlanetarySystemStacker. No Python required: download the archive for your
platform, unzip, and run. Windows, macOS and Linux.

> Keywords: astrophotography · planetary imaging · lunar imaging · lucky
> imaging · SER stacking · AutoStakkert / RegiStax / PlanetarySystemStacker
> alternative · Moon · Mars · Jupiter · Saturn.

---

## 功能特色 / Features

- **多對齊點局部對齊 / Multi-alignment-point (AP) local alignment** — 以網格扭曲
  修正大氣視寧度造成的局部形變，而非只做整體位移。 / Mesh-warp local
  registration that corrects seeing-induced local distortion, not just a
  global shift.
- **SER 影片直接讀取 / Reads SER capture files** — 支援 FireCapture、SharpCap 等
  常用擷取軟體輸出的 `.ser` 檔（含 debayer）。 / Opens `.ser` files from
  FireCapture, SharpCap and other capture tools (with debayering).
- **自動品質排名與挑幀 / Automatic quality ranking &amp; frame selection** — 依銳利度
  排名，取最佳的 top-% 疊合；可手動指定參考幀、手動排除壞幀。 / Ranks frames by
  sharpness and stacks the best top-%; manual reference-frame pick and manual
  frame rejection are also supported.
- **彩色與單色 / Colour &amp; mono** — 支援 RGB 通道對齊與 drizzle。 / RGB channel
  alignment and drizzle upscaling.
- **批次處理 / Batch processing** — 一次處理多個 SER 檔。 / Process many SER files
  in one run.
- **繁體中文 / English 介面 / Bilingual UI**。

---

## 繁體中文

### 下載

請至 [**Releases**](../../releases/latest) 頁面下載最新版本：

| 平台 | 檔案 |
| --- | --- |
| Windows (x64) | `MapStacker-windows-x64.zip` |
| Linux (x64) | `MapStacker-linux-x64.zip` |
| macOS (Apple Silicon) | `MapStacker-macos-arm64.zip` |

### 系統需求與注意事項

**Windows**
- Windows 10 / 11 (64-bit)。
- 解壓後執行資料夾內的 `MapStacker.exe`，不需另外安裝 Python。
- 若提示缺少 VC++ 執行庫，請安裝 Microsoft Visual C++ Redistributable（近代 Windows 多半已內建）。

**Linux**
- 需 **glibc ≥ 2.31**（Ubuntu 20.04+、Debian 11+ 或同等發行版）。
- 解壓後執行資料夾內的 `MapStacker`。
- 圖形介面使用 Qt xcb，在純文字環境或缺少 X11 的情況下無法啟動。

**macOS**
- 僅提供 **Apple Silicon (arm64)** 版；Intel Mac 不支援。
- 因 app 未簽章，首次開啟若被 Gatekeeper 阻擋，請右鍵 →「打開」，或到「系統設定 → 隱私權與安全性」放行。

### 多國語言

內建英文與繁體中文介面。

### 問題回報

發現問題或有需求？請至 [**Issues**](../../issues) 頁面開票。回報時請附上作業
系統、應用程式版本（見「說明 → 關於 MapStacker」）以及重現步驟。

---

## English

### What is MapStacker?

MapStacker is a free desktop tool for **lucky-imaging planetary and lunar
astrophotography**. Feed it a SER capture of the Moon, Mars, Jupiter or Saturn
and it ranks the frames by sharpness, aligns the best ones with a
**multi-alignment-point mesh warp** (correcting local seeing distortion), and
stacks them into a sharp result you can then wavelet-sharpen elsewhere. It is a
lightweight, cross-platform alternative to **AutoStakkert!3**, **RegiStax** and
**PlanetarySystemStacker (PSS)**.

### Download

Get the latest build from the [**Releases**](../../releases/latest) page:

| Platform | File |
| --- | --- |
| Windows (x64) | `MapStacker-windows-x64.zip` |
| Linux (x64) | `MapStacker-linux-x64.zip` |
| macOS (Apple Silicon) | `MapStacker-macos-arm64.zip` |

### Requirements &amp; notes

**Windows**
- Windows 10 / 11 (64-bit).
- Unzip and run `MapStacker.exe` from the folder; no separate Python install needed.
- If a missing VC++ runtime is reported, install the Microsoft Visual C++ Redistributable (usually already present on recent Windows).

**Linux**
- Requires **glibc ≥ 2.31** (Ubuntu 20.04+, Debian 11+, or equivalent).
- Unzip and run `MapStacker` from the folder.
- The GUI uses the Qt xcb platform plugin; it will not start in a headless or X11-less environment.

**macOS**
- **Apple Silicon (arm64) only**; Intel Macs are not supported.
- The app is unsigned. If Gatekeeper blocks the first launch, right-click → "Open", or allow it under System Settings → Privacy &amp; Security.

### Languages

English and Traditional Chinese UI are bundled.

### Support

Found a bug or have a request? Open an issue on the
[**Issues**](../../issues) page. Please include your OS, the app version
(shown under *Help → About MapStacker*), and the steps to reproduce.
