Changelog

All notable changes to this project will be documented in this file. This project adheres to Semantic Versioning.

[v0.1.0] - 2026-08-25
Added
- PR preview workflow for reviewing pull requests before merging
- GitHub Actions workflow for automated static site deployment to GitHub Pages

Changed
- Updated GitHub Pages deployment workflow to use JamesIves deploy action with clean: false to preserve PR preview folders

Reverted
- Removed experimental Hub integration (reverted to keep main branch stable)

[v0.0.1] - 2026-08-17
Added
- Initial CySA+ flashcard set
- First commit establishing project structure
- README with project overview
- GitHub Pages hyperlink added to README

This reads cleaner because it:

- Groups related commits into meaningful categories (Added, Changed, Reverted)
- Drops the merge commit since that's noise
- Explains the revert with context instead of just listing it
- Follows the Keep a Changelog standard format that most devs recognize
