<div align="center">

<br />

<a href="https://drive.google.com/file/d/1WooqwhF5uSOR7lb7JnSX3meqbsAuSw5T/view?usp=drive_link">
  <strong>View Hero Preview</strong>
</a>

<br />

# ScreenSentinel

### Real-time deepfake awareness for Windows.

ScreenSentinel is a native Windows desktop app that watches visible video content on your screen, detects faces, analyzes authenticity signals locally, and shows a compact confidence overlay while you continue browsing normally.

<br />

<a href="https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0">
  <img src="https://img.shields.io/badge/Download-v2.0.0-2563EB?style=for-the-badge&logo=github&logoColor=white" alt="Download ScreenSentinel v2.0.0" />
</a>
<a href="https://screensentinel.me">
  <img src="https://img.shields.io/badge/Website-screensentinel.me-111827?style=for-the-badge&logo=googlechrome&logoColor=white" alt="ScreenSentinel website" />
</a>
<img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0078D4?style=for-the-badge&logo=windows&logoColor=white" alt="Windows 10 and Windows 11" />
<img src="https://img.shields.io/badge/Release-v2.0.0-22C55E?style=for-the-badge" alt="Release v2.0.0" />

<br />
<br />

**Trust what you watch. Detect uncertainty before it becomes belief.**

</div>

---

## Why ScreenSentinel Exists

Deepfakes are no longer rare, obvious, or slow to make. They appear in short-form videos, reposted clips, online debates, ads, scams, impersonation attempts, and social feeds where people make trust decisions in seconds.

Most verification tools ask you to stop what you are doing:

- download or copy the video,
- upload it somewhere else,
- wait for analysis,
- then return to the content after the moment has already passed.

ScreenSentinel takes a different approach. It acts like a lightweight authenticity layer on top of your screen, giving you a real-time signal while the content is still in front of you.

> ScreenSentinel is not a replacement for human judgment or forensic review. It is a decision-support tool designed to make suspicious media harder to ignore.

---

## Download

<div align="center">

### Latest Stable Release

<a href="https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0">
  <img src="https://img.shields.io/badge/Download%20ScreenSentinel-v2.0.0-2563EB?style=for-the-badge&logo=windows&logoColor=white" alt="Download ScreenSentinel v2.0.0" />
</a>

<br />
<br />

Windows 10 and Windows 11 are supported.

</div>

| Release | Platform | Source Code |
|---|---:|---:|
| [v2.0.0](https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0) | Windows | Private |

This repository is intended as the public product page and release landing page. The Windows application source code is not included here.

---

## Product Preview

<div align="center">

<a href="https://drive.google.com/file/d/1WooqwhF5uSOR7lb7JnSX3meqbsAuSw5T/view?usp=drive_link">
  <strong>Open ScreenSentinel Hero Image</strong>
</a>

</div>

---

## What It Does

ScreenSentinel runs as a Windows desktop application with a small always-on-top overlay. As video content appears on screen, it captures frames, detects faces, analyzes them using a deepfake detection model, smooths the results over time, and displays a human-readable confidence state.

### Core Capabilities

| Capability | What it means |
|---|---|
| Real-time screen analysis | Watches visible content while you browse, scroll, or watch videos. |
| Floating Windows overlay | Shows authenticity status without needing a browser extension. |
| Face-focused detection | Detects faces from captured frames before running authenticity analysis. |
| 5-tier confidence system | Reports more than just real/fake, including uncertain states. |
| Temporal smoothing | Reduces flickering results by aggregating predictions across frames. |
| Rule-based explanations | Gives simple text explanations for detection states. |
| System tray controls | Runs quietly with quick access to pause, resume, and open settings. |
| Local-first processing | Video frames are analyzed on the device rather than uploaded for cloud analysis. |

---

## Detection States

ScreenSentinel does not force every result into a binary answer. It uses confidence levels so uncertain content can stay uncertain.

| State | Meaning | Typical UI Color |
|---|---|---|
| `REAL` | Strong signal that visible facial content appears authentic. | Green |
| `LIKELY REAL` | Mostly authentic-looking signal, but with slightly lower confidence. | Lime |
| `UNCERTAIN` | Not enough confidence to call the content real or manipulated. | Yellow |
| `LIKELY FAKE` | Suspicious manipulation indicators are present. | Orange |
| `DEEPFAKE` | Strong signal that visible facial content may be manipulated. | Red |

<br />

<table>
  <tr>
    <td align="center" width="50%">
      <a href="https://drive.google.com/file/d/1ezMdQKByjvLEk1Lqfu2GiBgOy_Ff34gI/view?usp=drive_link">
        View real-state preview
      </a>
      <br />
      <br />
      <strong>REAL / LIKELY REAL</strong>
    </td>
    <td align="center" width="50%">
      <a href="https://drive.google.com/file/d/1XxLq0ci76wF9aoeCxzATUXxRXThqljyl/view?usp=drive_link">
        View fake-state preview
      </a>
      <br />
      <br />
      <strong>LIKELY FAKE / DEEPFAKE</strong>
    </td>
  </tr>
</table>

---

## How It Works

```text
Visible video content
        |
        v
Screen capture
        |
        v
Face detection
        |
        v
Deepfake model inference
        |
        v
Temporal aggregation
        |
        v
Confidence level + overlay explanation
```

### Detection Pipeline

| Stage | Purpose |
|---|---|
| Screen Capture | Captures visible screen frames at a controlled rate. |
| Motion Filtering | Skips static frames to reduce unnecessary work. |
| Face Detection | Finds faces before analysis so the model focuses on relevant regions. |
| MesoNet Inference | Runs deepfake classification on detected face crops. |
| Temporal Aggregation | Combines recent frame results for a steadier confidence signal. |
| Confidence Engine | Converts raw scores into readable states like `UNCERTAIN` or `DEEPFAKE`. |
| Overlay UI | Displays the current result in a compact, always-on-top Windows widget. |

---

## Built For Real-World Viewing

ScreenSentinel is designed for the way people actually encounter suspicious media: quickly, casually, and often inside another app.

It can assist while watching:

- short-form social media videos,
- livestream clips,
- video reposts,
- online interviews,
- video calls,
- browser-based video content,
- locally played media.

No copy-pasting links. No re-uploading private videos. No switching to a separate scanner first.

---

## Privacy Model

ScreenSentinel is designed around local analysis.

- Video content is analyzed on your Windows machine.
- No user video needs to be uploaded for the core detection workflow.
- Settings are stored locally under the user's application data directory.
- Optional screenshot capture is controlled through app settings.

The app should still be treated as security-sensitive software because it can inspect visible screen content. Only download releases from the official release page linked above.

---

## Demo Video

A proper video demo is not available yet.

When it is ready, this section can be replaced with:

```markdown
<video demo link or GIF preview>
```

For now, the screenshots above show the current product direction and detection-state UI.

---

## Installation

### Recommended

Download the Windows build from the latest release:

[Download ScreenSentinel v2.0.0](https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0)

Then run the installer or packaged executable included in the release assets.

### Important

The public repository is a release/documentation page. The Windows app source code is private and is not required for normal installation.

---

## Requirements

| Requirement | Notes |
|---|---|
| Operating System | Windows 10 or Windows 11 |
| Display Content | Works on visible screen content where faces can be detected |
| Release | Use the official `v2.0.0` release |
| Internet | Not required for local detection after installation, but useful for downloading updates |

Performance depends on hardware, screen resolution, video quality, lighting, face size, compression, and the number of visible faces.

---

## Limitations

ScreenSentinel is an assistive detection layer, not a truth oracle.

It may produce false positives or false negatives when:

- faces are very small or partially hidden,
- the video is heavily compressed,
- lighting is poor,
- the face is turned away or blurred,
- the content contains filters, beauty effects, or stylized edits,
- the manipulation method is outside the model's learned distribution,
- no face is visible.

Use ScreenSentinel as one signal among many, especially for high-stakes content.

---

## Roadmap

| Status | Area | Notes |
|---|---|---|
| Done | Windows desktop app | Native overlay-first experience. |
| Done | 5-tier confidence states | More nuanced than a binary label. |
| Done | Local-first detection flow | Core analysis runs on device. |
| Planned | Video demo | A polished walkthrough will be added later. |
| Planned | Performance improvements | Faster inference and smoother UI. |
| Planned | Additional model support | Stronger detection backends and model ensembles. |
| Exploring | Browser extension | Lower-friction browser-specific workflow. |
| Exploring | Mobile support | Android/iOS feasibility. |

---

## Frequently Asked Questions

<details>
<summary><strong>Does ScreenSentinel upload my videos?</strong></summary>

The core detection workflow is designed to analyze visible screen content locally on your device rather than uploading user videos for remote analysis.

</details>

<details>
<summary><strong>Does it work only on websites?</strong></summary>

No. ScreenSentinel watches visible screen content, so it is not limited to a particular browser tab or website.

</details>

<details>
<summary><strong>Is the app source code public?</strong></summary>

No. The Windows application source code is private. This repository is used for product information and public releases.

</details>

<details>
<summary><strong>Can I rely on it as final proof that something is fake?</strong></summary>

No. Deepfake detection is probabilistic. ScreenSentinel should be treated as a warning and awareness tool, not a final forensic authority.

</details>

<details>
<summary><strong>Where should I download it from?</strong></summary>

Use the official release page:

https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0

</details>

---

## Links

| Destination | Link |
|---|---|
| Website | [screensentinel.me](https://screensentinel.me) |
| Latest Release | [v2.0.0](https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0) |
| GitHub Profile | [omtripathi52](https://github.com/omtripathi52) |

---

<div align="center">

## ScreenSentinel

Real-time deepfake awareness for Windows.

<br />

<a href="https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0"><strong>Download v2.0.0</strong></a>
&nbsp;&nbsp;•&nbsp;&nbsp;
<a href="https://screensentinel.me"><strong>Visit Website</strong></a>

<br />
<br />

Built by <a href="https://github.com/omtripathi52">Om Tripathi</a>.

</div>
