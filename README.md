# scorza-wiki
Personal wiki and study notes I wrote and made public

[![Lighthouse Performance](https://img.shields.io/badge/Lighthouse-100%2F100-success?style=flat-square&logo=lighthouse)](https://pagespeed.web.dev/analysis?url=https%3A%2F%2Fscorza9999.github.io%2Fscorza-wiki%2F)
[![CI Build](https://github.com/Scorza9999/scorza-wiki/actions/workflows/ci.yml/badge.svg)](https://github.com/Scorza9999/scorza-wiki/actions/workflows/ci.yml)

## Contents
Currently archiving my study notes and lab documentation for:
* **Cisco NetAcad** 

## Infrastructure & Performance
I hate how bloated and slow the modern web has become, so I tried to make my corner as fast as possible. 
Built with a zero-bloat, docs-as-code architecture to ensure maximum rendering speed and minimal browser overhead.

* **Static Generation:** Pre-compiled via MkDocs Material. Zero server-side rendering or database queries.
* **CI/CD Pipeline:** Automated HTML minification (`mkdocs-minify-plugin`) running on GitHub Actions. CSS/JS minification when I'll add them.
* **Delivery:** Hosted on Github Pages, which use Fastly CDN with Brotli/GZip compression.
* **Performance Metrics (Throttled Mobile):**
  * **LCP & FCP:** `0.4s` (lowest: `0.3s`)
  * **Total Blocking Time (TBT):** `0ms`
  * **Cumulative Layout Shift (CLS):** `0`

<details>
<summary><b>📊 View Lighthouse Baseline Metrics</b></summary>
<br>
Performance baseline captured on initial deployment:
<img src="website_performance.png" alt="Lighthouse 100/100 Report showing 0.3s LCP and 0ms TBT" width="600">
</details>
 
_Note: My wiki is still WIP, so these numbers are subject to change_

