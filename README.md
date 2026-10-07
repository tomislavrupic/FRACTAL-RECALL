# FRACTAL RECALL — public landing and releases

[Visit the landing page and downloads](https://tomislavrupic.github.io/FRACTAL-RECALL/)

![FRACTAL RECALL — Every repeat has consequences.](site/assets/banner.jpg)

Pixel Records' evolving stereo delay. This repository owns the GitHub Pages landing page and release automation. The working audio product remains in the separate FRACTAL RECALL folder; its corresponding AGPLv3 source is attached to each binary release.

## Local preview

```sh
python3 -m http.server 4177 --directory site
```

Publish `site/` with `.github/workflows/pages.yml`. The page is a dependency-free static site. Test desktop/mobile, screenshot switching, dialog keyboard behavior, links and image loading before publishing. `output/playwright/` contains local verification evidence and is not committed.

## Release

Mac 0.3.0: Apple Silicon macOS12+, AU/VST3 and standalone. Development ad-hoc signature; no notarization. Local DSP/native tests, pluginval and strict auval passed. Corresponding source includes pinned JUCE8.0.14 and HRIR attribution.

Windows workflow consumes the release's corresponding-source ZIP, verifies its SHA256, builds and tests on a native Windows x64 runner, and uploads the resulting VST3/standalone package. Windows 0.3.0 x64 is now available: native 83 DSP / 13 processor tests and pluginval 1.0.4 strictness 5 passed in [run 37687466428](https://github.com/tomislavrupic/FRACTAL-RECALL/actions/runs/37687466428). Archive integrity and both AMD64 binaries were independently checked; see `docs/windows-release-verification.json`. A native CI build is not a DAW listening test.

Banner artwork uses built-in image generation, based on the native editor's material/color identity; generation prompt and provenance are in `docs/banner-provenance.json`. Screenshots show the actual native plugin, not generated UI. Page-source license: AGPLv3; third-party notices accompany the plugin downloads.

Windows CI builds the explicit `FractalRecall_VST3`, `FractalRecall_Standalone`, `FractalTests` and `FractalProcessorTests` targets. The local macOS screenshot helper (`FractalPreview`) has a console-style entry point and is intentionally outside the Windows shipping build.
