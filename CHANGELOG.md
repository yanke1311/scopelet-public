# Changelog

## 0.1.8

- Add independent interface and preview font sizes, a compact 12px interface default, and font-aware result rows and preview navigation.
- Bring default control heights, spacing, and secondary text closer to 0.1.7: a 39px search field, 36px pane headings, and 11px secondary text.

- Refine the search-first layout, result hierarchy, inline match highlighting, preview headers, and high-contrast handling.
- Add editable Scope chips for multiple directories and globs, grouped scope history, path completion, and an explicit relative-path base. Existing directory and search history remain compatible.
- Replace Include/Exclude text areas with multi-rule chips; keep filters collapsed by default and show applied/pending state. Preserve comma expressions and multiline paste.
- Preserve explicit ignored directories when combining scopes, deduplicate overlapping file paths, and establish a missing base when selecting a directory.
- Expand preview choices to all 65 bundled Shiki themes plus Auto, including Catppuccin's four flavors. Group the selector by appearance and provide searchable names in the Command Palette.
- Load theme files locally on demand, cache them, reject stale theme responses, and include third-party theme license notices.
- Improve empty-state actions, result-limit feedback, narrow-window layouts, and preview navigation for long lines and large files.
- Replace the README's main screenshot with a recorded search demonstration, add a theme-switching animation, and refresh the light-theme screenshot.

## 0.1.7

- Clarify the VS Code Marketplace distribution and pending approval status; identify the public repository as documentation and support materials, not implementation source.
- Add a bilingual privacy notice and replace source-development instructions in the public documentation with issue-reporting guidance.
- Keep public documentation/image URLs explicit without advertising the documentation repository as the extension's source repository.
- Point support and documentation links at the public `yanke1311/scopelet-public` materials repository.
- Rewrite README and changelog links to public HTTPS URLs for the Marketplace listing.
- Exclude the unused ripgrep type declaration and local copies of the wordmark, screenshots, and Chinese README. Documentation and screenshots remain available through public HTTPS links; the privacy notice is included in the VSIX.
- Retain the extension icon, panel logo, runtime code, platform-specific ripgrep binary, and license notices. This repack keeps version 0.1.7 and does not change search behavior or confirm Marketplace acceptance.

## 0.1.6

- Prepare the `ke-yan.scopelet` Marketplace identity, listing metadata, and English/Chinese presentation.
- Normalize Windows search paths for consistent filtering and result labels; update cross-platform tests.
- Keep performance diagnostics exclusive to automated Test mode.

**Migration:** earlier trial packages used `scopelet-local.scopelet`. Disable or uninstall that extension when switching to the new ID. Stored extension history and preferences are not automatically migrated.

This version is being prepared for its first Marketplace release; it is not a claim of publication.
