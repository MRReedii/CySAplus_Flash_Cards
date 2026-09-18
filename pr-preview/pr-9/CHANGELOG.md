# Changelog

All notable changes to this project will be documented in this file. This project adheres to Semantic Versioning.

[v0.2.0] - 2026-09-18
Added
- Question parser helper utilities and CyberQuizz mode functionality
- Text-to-speech audio playback for flashcards with dedicated error handling
- Support for external data sources, dataset URL fetching, local set merging, and question set splitting
- Input validation on custom data sources
- Cross-site scripting (XSS) protections across user inputs and uploads
- Sign-In portal gated under a feature flag
- LICENSE file with MIT License and Commons Clause

Changed
- Moved "Upload Question Sets" call-to-action into the footer UI and updated overall Upload component styling
- Refactored question set fetching, URL resolution, and local storage handling routines
- Revised README.md with clearer section headers and updated links to the live application
- Updated .gitignore for static HTML/JS projects

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
