# Landing launch verification · 2026-10-07

Actual native0.3.0 snapshots; built-in image_gen banner with saved prompt/provenance. Local page checked at1440×1000 and390×844: no horizontal overflow, assets loaded and internal links resolve. Screenshot tabs switch and support arrow keys; fullscreen dialog opens, Escape closes and restores focus. Browser console has zero errors/warnings. Static asset/ID/anchor check and JavaScript syntax pass. No iframe, autoplay audio, external font request or analytics.

Mac release contains installed/validated0.3.0 AU/VST3/standalone; ad-hoc signed and not notarized. Public corresponding-source package has full dependency and license/provenance. A clean extraction initially exposed missing empty Git refs directories; corrected archive retains directories, Git verifies pinned JUCE revision, source manifest matches every file. External pluginval binary is excluded from the corresponding source. Public0.3.0 package checksums are attached to the release and recorded in public-package-receipt.json.

Windows native build is separate from Pages deployment and not advertised as available until build, DSP/native tests, pluginval and packaging succeed. Mac/local DAW listening and Windows DAW compatibility are not inferred from CI.

Publication uses the dedicated public FRACTAL-RECALL repository; original audio product and outer workspace remain unversioned. Previous local0.2 packages and installed backups remain intact. Store, author website and sibling product links are included; store source is not modified by this task.
