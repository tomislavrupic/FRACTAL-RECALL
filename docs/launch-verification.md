# Landing launch verification · 2026-10-07

Actual native0.3.0 snapshots; built-in image_gen banner with saved prompt/provenance. Local page checked at1440×1000 and390×844: no horizontal overflow, assets loaded and internal links resolve. Screenshot tabs switch and support arrow keys; fullscreen dialog opens, Escape closes and restores focus. Browser console has zero errors/warnings. Static asset/ID/anchor check and JavaScript syntax pass. No iframe, autoplay audio, external font request or analytics.

Mac release contains installed/validated0.3.0 AU/VST3/standalone; ad-hoc signed and not notarized. Public corresponding-source package has full dependency and license/provenance. A clean extraction initially exposed missing empty Git refs directories; corrected archive retains directories, Git verifies pinned JUCE revision, source manifest matches every file. External pluginval binary is excluded from the corresponding source. Public0.3.0 package checksums are attached to the release and recorded in public-package-receipt.json.

Windows native build is separate from Pages deployment and not advertised as available until build, DSP/native tests, pluginval and packaging succeed. Mac/local DAW listening and Windows DAW compatibility are not inferred from CI.

Publication uses the dedicated public FRACTAL-RECALL repository; original audio product and outer workspace remain unversioned. Previous local0.2 packages and installed backups remain intact. Store, author website and sibling product links are included; store source is not modified by this task.

Windows run37685888167 compiled VST3, standalone and both test binaries, but the aggregate build failed at the internal screenshot helper (WinMain linker entry point). Shipping workflow now selects the four required targets explicitly; no DSP source change or test removal. Windows availability still requires the complete native test/validator/package gate.

Final Windows gate: run37687466428 succeeded on exact published source SHA25607628ab996040f437520887231ac5bf45b0eba0cd3b7d24a90c864773100f0e6. 83 DSP and13 processor tests passed; pluginval1.0.4 strictness5 returned SUCCESS. Downloaded artifact ZIP passes integrity check, both shipping binaries are PE AMD64, source/version/run/commit and package SHA256 match the receipt, and license/HRIR/install notices are present. Public GitHub release digest matches local ZIP e1b4a32e2d83c812c44510d2e3232083e5307736d6b1025b2762a5c7a5dfd6f5. Windows button enabled only after upload and digest verification.

Initial Pages deployment37686138264 passed at5288768; all10 live files matched local bytes. Actual live browser checked1440px and390px, image loading and screenshot switching; zero console errors/warnings. Public Mac ZIP downloaded again with checksum/integrity and AU/VST3/standalone contents confirmed. Final download-card update requires another Pages deployment and live check.
