# 🎬 320 Video Downloader by shahin0774@

A **portable YouTube video downloader** (320x240 resolution) in a single EXE file.

---

## ✨ Features

- 320x240 resolution, MPEG-4
- Auto split videos: 
  - ≤30 minutes → single file
  - >30 minutes → Part 1 & Part 2
- Fullscreen stretch output
- Date-based download folder
- Portable: No installation required
- Desktop-friendly: EXE downloaded into `Desktop\Video Downloader` folder
- Auto-run EXE and open folder after download

---

## 🚀 How to Install / Run

### Option 1: PowerShell One-Liner (Recommended)

Open **PowerShell** and copy-paste:

```powershell
$folder=Join-Path $env:USERPROFILE "Desktop\Video Downloader";if(!(Test-Path $folder)){New-Item -ItemType Directory -Path $folder | Out-Null};$exe=Join-Path $folder "320VideoDownloader.exe";iwr "https://raw.githubusercontent.com/shahinalam0774/320videodownloader/main/320VideoDownloader.exe" -OutFile $exe;Start-Process $exe;Start-Process $folder
