# MapStacker

行星／月面影像疊合工具。免安裝 Python，下載對應平台的壓縮檔，解壓後即可執行。

Planetary &amp; lunar image stacking tool. No Python required — download the
archive for your platform, unzip, and run.

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

---

## English

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
