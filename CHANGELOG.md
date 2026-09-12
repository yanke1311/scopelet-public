# Changelog

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
