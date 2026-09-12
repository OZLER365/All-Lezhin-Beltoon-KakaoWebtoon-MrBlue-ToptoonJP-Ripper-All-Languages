# Universal Webtoon Ripper (Lezhin, Beltoon, Kakao, Mr-Blue, Toptoon JP)

A highly efficient userscript designed to extract and download high-quality webtoon panels using advanced Blob Hook interception and DOM-based sequence splicing. This tool bypasses the need for Canvas descrambling and downloads panels directly as lossless PNG files into a neatly organized folder.

## ✨ Core Features

* **Blob Hook Engine:** Intercepts raw image data directly from the network stream, perfectly capturing protected images without relying on secondary Canvas rendering.
* **Global Sequence Splicer:** Uses a DOM scanner to anchor intercepted blob data to the physical top-to-bottom layout of the page, ensuring pages are numbered in the exact reading order.
* **Cryptographic Deduplication:** Calculates SHA-256 hashes for every incoming blob to prevent duplicate images from being saved to the final folder.
* **Professional Floating UI:** Features a dark-themed, draggable, and minimizable control panel with a custom scroll-delay slider and an auto-download toggle.
* **Lossless PNG Export:** Automatically converts all captured WebP/JPEG blobs into high-quality PNG files during the download phase (Note: ZIP generation is not supported; images download directly to a folder).

## 🌐 Supported Platforms & Language Variants

This script supports multiple regional variants (English, Japanese, Korean, Thailand, France, Germany, Spain, China/Taiwan) for the following platforms:

* **Lezhin** (`.com`, `.us`, `.es`, `.jp`, `.de`, `.fr`, `.th`)
* **Bomtoon / Beltoon** (`.com`, `.tw`, `.jp`)
* **Kakao Webtoon**
* **Mr. Blue**
* **Toptoon JP** (Note: Only the Japanese variant is supported)

## ⚠️ Platform-Specific Behaviors & Quirks

| Platform | Recommended Usage & Known Quirks |
| :--- | :--- |
| **Mr. Blue** | Auto-scroll is completely unnecessary; the script captures all images automatically in the background within seconds. |
| **Kakao Webtoon** | Do not use auto-scroll. Simply open the chapter and wait for the capture counter in the UI to stop increasing. |
| **Lezhin Thailand** | Auto-scroll is not required and does not function on this specific variant. Wait for the background capture to complete. |
| **Toptoon JP** | Auto-scrolling works but is notably slow. It is highly recommended to manually scroll to the bottom of the page to trigger image loads. |
| **Page Counters** | The UI's total page counter relies on the site's reading progress bar, which means it may occasionally display an inaccurate "total" number compared to the actual image count. |

## 🚀 Installation & Usage

1. **Prerequisite:** Install the **Tampermonkey** extension in your browser.
2. **Install Script:** Download the latest version (v3.6.8) from [Greasyfork][https://greasyfork.org/en/users/1553223-ozler365](https://greasyfork.org/en/scripts/563063-all-lezhin-beltoon-kakao-webtoon-mr-blue-toptoon-jp-ripper-all-languages])
3. **Usage:** Open a supported chapter. Use the floating UI to adjust the **Scroll Delay** (if auto-scrolling is needed) and click **Start Auto-Capture**.
4. **Download:** Once the capture counter stops, click **Download Captured** to save the panels to your device.

## 🔗 Links, Feedback & Support

**This script is strictly for educational purposes. Do not repost or distribute the downloaded images.**

* **Greasyfork Scripts:** [ozler365's Profile](https://greasyfork.org/en/users/1553223-ozler365)
* **GitHub Repositories:** [ozler-s-works-info](https://ozler365.github.io/ozler-s-works-info/#/repositories)
* **Support the Developer:** Keep this script updated by leaving a tip at [Buy Me a Coffee (ozler)](https://buymeacoffee.com/ozler)

For queries, bug reports, or feature requests, please leave a review on Greasyfork or email **devjk6918@gmail.com**.
