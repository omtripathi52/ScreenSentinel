<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=230&color=0:020617,42:0F172A,72:1D4ED8,100:06B6D4&text=ScreenSentinel&fontColor=FFFFFF&fontSize=62&fontAlignY=35&desc=Real-time%20deepfake%20awareness%20for%20Windows&descAlignY=55&descSize=18&animation=fadeIn" alt="ScreenSentinel banner" width="100%" />

<br />

<img src="https://drive.google.com/thumbnail?id=1Av-q9QhncanhAYEmxosdXb480shLcKJQ&sz=w320" alt="ScreenSentinel logo" width="118" />

<br />
<br />

<img src="https://readme-typing-svg.demolab.com?font=Inter&weight=700&size=24&duration=2800&pause=900&color=38BDF8&center=true&vCenter=true&width=900&lines=Watch+normally.+Verify+as+you+go.;A+floating+AI+safety+layer+for+video+authenticity.;Real-time+deepfake+detection+for+Windows." alt="ScreenSentinel typing headline" />

<br />
<br />

<a href="https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0">
  <img src="https://img.shields.io/badge/Download-v2.0.0-2563EB?style=for-the-badge&logo=windows&logoColor=white" alt="Download v2.0.0" />
</a>
<a href="https://screensentinel.me">
  <img src="https://img.shields.io/badge/Website-screensentinel.me-0F172A?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" />
</a>
<img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0078D4?style=for-the-badge&logo=windows11&logoColor=white" alt="Windows" />
<img src="https://img.shields.io/badge/Source-Private-111827?style=for-the-badge&logo=github&logoColor=white" alt="Private source" />

<br />
<br />

<strong>ScreenSentinel is a native Windows desktop app that watches visible video content, detects faces, analyzes authenticity signals locally, and displays a compact confidence overlay in real time.</strong>

<br />
<br />

<a href="#download"><strong>Download</strong></a>
&nbsp;&nbsp;|&nbsp;&nbsp;
<a href="#product-preview"><strong>Preview</strong></a>
&nbsp;&nbsp;|&nbsp;&nbsp;
<a href="#how-it-works"><strong>How It Works</strong></a>
&nbsp;&nbsp;|&nbsp;&nbsp;
<a href="#privacy-model"><strong>Privacy</strong></a>
&nbsp;&nbsp;|&nbsp;&nbsp;
<a href="#faq"><strong>FAQ</strong></a>

</div>

---

<div align="center">

## The Problem

</div>

The internet has entered the **synthetic media era**. Deepfakes no longer look like obvious edits. They appear inside short-form videos, livestream clips, reposted news footage, scam ads, impersonation attempts, and ordinary social feeds where trust decisions happen in seconds.

Traditional verification tools ask users to stop watching, download or copy the media, upload it somewhere else, wait for analysis, and then return to the content later.

That workflow is too slow for the way people actually consume video.

ScreenSentinel brings the authenticity signal directly to the moment of viewing.

<br />

<table>
  <tr>
    <td width="50%">
      <h3>Traditional Detection</h3>
      <ul>
        <li>Upload or paste media manually</li>
        <li>Leave the current app or website</li>
        <li>Wait for a separate scan</li>
        <li>Verify after the moment has passed</li>
      </ul>
    </td>
    <td width="50%">
      <h3>ScreenSentinel</h3>
      <ul>
        <li>Watch normally</li>
        <li>Keep the overlay on screen</li>
        <li>Analyze visible faces locally</li>
        <li>See confidence while content is playing</li>
      </ul>
    </td>
  </tr>
</table>

> ScreenSentinel is a decision-support tool. It is designed to raise awareness and surface suspicious signals, not to act as final forensic proof.

---

<div align="center">

## Product Preview

<img src="https://drive.google.com/thumbnail?id=1WooqwhF5uSOR7lb7JnSX3meqbsAuSw5T&sz=w1600" alt="ScreenSentinel hero preview" width="96%" />

<br />
<br />

<sub>If the image does not render on GitHub, make sure the Google Drive file is shared as <strong>Anyone with the link can view</strong>.</sub>

</div>

---

<div align="center">

## Detection States

ScreenSentinel uses confidence levels instead of pretending every result is perfectly binary.

</div>

<br />

<table>
  <tr>
    <td align="center" width="50%">
      <img src="https://drive.google.com/thumbnail?id=1ezMdQKByjvLEk1Lqfu2GiBgOy_Ff34gI&sz=w1000" alt="ScreenSentinel real detection state" width="100%" />
      <h3>REAL / LIKELY REAL</h3>
      <p>Visible facial content appears authentic with stronger confidence.</p>
    </td>
    <td align="center" width="50%">
      <img src="https://drive.google.com/thumbnail?id=1XxLq0ci76wF9aoeCxzATUXxRXThqljyl&sz=w1000" alt="ScreenSentinel fake detection state" width="100%" />
      <h3>LIKELY FAKE / DEEPFAKE</h3>
      <p>Suspicious facial manipulation indicators are detected.</p>
    </td>
  </tr>
</table>

<br />

| State | Meaning | UI Signal |
|---|---|---|
| `REAL` | Strong authentic-looking signal | Green |
| `LIKELY REAL` | Mostly authentic-looking signal | Lime |
| `UNCERTAIN` | Confidence is not high enough either way | Yellow |
| `LIKELY FAKE` | Manipulation indicators are present | Orange |
| `DEEPFAKE` | Strong manipulated-media signal | Red |

---

<div align="center">

## Product Experience

</div>

<table>
  <tr>
    <td width="33%">
      <h3>Always-On Awareness</h3>
      <p>A compact floating overlay stays visible while you browse, watch, scroll, or attend calls.</p>
    </td>
    <td width="33%">
      <h3>Local-First Analysis</h3>
      <p>The core workflow analyzes visible screen content on the device instead of requiring video uploads.</p>
    </td>
    <td width="33%">
      <h3>Confidence, Not Guesswork</h3>
      <p>Five detection states communicate uncertainty instead of forcing every result into real or fake.</p>
    </td>
  </tr>
  <tr>
    <td width="33%">
      <h3>Face-Focused Detection</h3>
      <p>ScreenSentinel detects faces first, then runs authenticity analysis on the relevant regions.</p>
    </td>
    <td width="33%">
      <h3>Temporal Smoothing</h3>
      <p>Predictions are aggregated across recent frames to reduce flicker and improve stability.</p>
    </td>
    <td width="33%">
      <h3>Windows-Native Controls</h3>
      <p>System tray access, pause/resume controls, notifications, settings, and overlay behavior are designed for desktop use.</p>
    </td>
  </tr>
</table>

---

<div align="center">

## Download

<a href="https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0">
  <img src="https://img.shields.io/badge/Download%20ScreenSentinel-v2.0.0-2563EB?style=for-the-badge&logo=github&logoColor=white" alt="Download ScreenSentinel v2.0.0" />
</a>

<br />
<br />

Latest stable release for Windows 10 and Windows 11.

</div>

<br />

| Release | Platform | Status | Source Code |
|---|---|---|---|
| [v2.0.0](https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0) | Windows | Stable release | Private |

This repository is the public product and release page. The Windows application source code is private and is not required for installation.

---

<div align="center">

## How It Works

</div>

```mermaid
flowchart LR
    A[Visible video content] --> B[Screen capture]
    B --> C[Motion filtering]
    C --> D[Face detection]
    D --> E[Deepfake model inference]
    E --> F[Temporal aggregation]
    F --> G[Confidence engine]
    G --> H[Floating Windows overlay]

    style A fill:#0f172a,stroke:#38bdf8,color:#ffffff
    style H fill:#1d4ed8,stroke:#67e8f9,color:#ffffff
    style E fill:#111827,stroke:#f97316,color:#ffffff
    style G fill:#111827,stroke:#22c55e,color:#ffffff
```

### Pipeline Overview

| Layer | Role |
|---|---|
| Screen Capture | Captures visible desktop frames at a controlled rate. |
| Motion Filtering | Skips static frames to reduce unnecessary processing. |
| Face Detection | Finds visible faces before running authenticity analysis. |
| Deepfake Inference | Evaluates detected face crops with a deepfake detection model. |
| Temporal Engine | Smooths predictions over a recent frame window. |
| Confidence Engine | Converts raw scores into readable detection states. |
| Overlay UI | Shows the result in a compact always-on-top interface. |

---

<div align="center">

## Built For Real-World Viewing

</div>

ScreenSentinel is designed for the places where suspicious video is actually encountered:

<table>
  <tr>
    <td>Short-form videos</td>
    <td>Livestream clips</td>
    <td>Browser video</td>
  </tr>
  <tr>
    <td>Video calls</td>
    <td>Reposted social media clips</td>
    <td>Local video playback</td>
  </tr>
  <tr>
    <td>News clips</td>
    <td>Scam ads</td>
    <td>Impersonation attempts</td>
  </tr>
</table>

No copy-pasting links. No manual uploads. No browser extension required.

---

<div align="center">

## Privacy Model

</div>

ScreenSentinel is designed around local analysis.

- Core detection runs on the Windows device.
- User videos do not need to be uploaded for the detection workflow.
- App settings are stored locally in the user's application data directory.
- Optional screenshot capture is controlled by app settings.
- Users should only download builds from the official release page.

Because ScreenSentinel can inspect visible screen content, it should be treated as security-sensitive desktop software.

---

<div align="center">

## Requirements

</div>

| Requirement | Details |
|---|---|
| Operating System | Windows 10 or Windows 11 |
| Release | v2.0.0 |
| Content Type | Visible screen content with detectable faces |
| Internet | Needed to download releases and updates; core local analysis does not require uploading videos |

Performance can vary based on hardware, display resolution, video quality, compression, lighting, face size, and number of visible faces.

---

<div align="center">

## Demo Video

</div>

A polished video demo is not available yet.

When the demo is ready, this section will be replaced with a walkthrough showing:

- installation,
- overlay startup,
- real-state detection,
- fake-state detection,
- pause/resume controls,
- settings and notification behavior.

---

<div align="center">

## Limitations

</div>

Deepfake detection is probabilistic. ScreenSentinel may produce false positives or false negatives, especially when:

- faces are tiny, blurred, hidden, or turned away,
- lighting is poor,
- the video is heavily compressed,
- beauty filters or stylized effects are applied,
- no face is visible,
- the manipulation method is outside the model's learned distribution,
- the clip is too short or unstable for confident temporal aggregation.

Use ScreenSentinel as a warning signal, not as final proof.

---

<div align="center">

## Roadmap

</div>

| Status | Area | Direction |
|---|---|---|
| Complete | Windows desktop overlay | Native always-on-top detection experience |
| Complete | v2.0.0 release | Public Windows release build |
| Complete | 5-tier confidence states | Real, likely real, uncertain, likely fake, deepfake |
| Planned | Video demo | Polished product walkthrough |
| Planned | Performance tuning | Faster analysis and smoother overlay updates |
| Planned | Stronger model support | Additional model backends and ensemble options |
| Exploring | Browser workflow | Browser-specific experience |
| Exploring | Mobile workflow | Android/iOS feasibility |

---

<div align="center">

## FAQ

</div>

<details>
<summary><strong>Why were normal Google Drive links not rendering as images?</strong></summary>

Google Drive's normal `/file/d/.../view` links open a preview page, not the raw image. GitHub README images need an actual image endpoint. This README uses Drive thumbnail URLs so the images can render directly.

</details>

<details>
<summary><strong>What if the images still do not show on GitHub?</strong></summary>

Set each Google Drive file to <strong>Anyone with the link can view</strong>. If the files are private or restricted, GitHub cannot fetch them.

</details>

<details>
<summary><strong>Does ScreenSentinel upload videos?</strong></summary>

The core detection workflow is designed around local analysis of visible screen content on the user's Windows device.

</details>

<details>
<summary><strong>Is the source code public?</strong></summary>

No. This repository is a public product and release page. The Windows application source code is private.

</details>

<details>
<summary><strong>Is ScreenSentinel final proof that something is fake?</strong></summary>

No. It is a decision-support and awareness tool. Deepfake detection is probabilistic and should be combined with human judgment and additional verification for high-stakes cases.

</details>

---

<div align="center">

## Links

<a href="https://screensentinel.me">
  <img src="https://img.shields.io/badge/Website-screensentinel.me-0F172A?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" />
</a>
<a href="https://github.com/omtripathi52/ScreenSentinel/releases/tag/v2.0.0">
  <img src="https://img.shields.io/badge/Latest%20Release-v2.0.0-2563EB?style=for-the-badge&logo=github&logoColor=white" alt="Release" />
</a>
<a href="https://github.com/omtripathi52">
  <img src="https://img.shields.io/badge/Creator-Om%20Tripathi-111827?style=for-the-badge&logo=github&logoColor=white" alt="Creator" />
</a>

<br />
<br />

<img src="https://capsule-render.vercel.app/api?type=waving&height=120&section=footer&color=0:06B6D4,50:1D4ED8,100:020617" alt="footer wave" width="100%" />

</div>

