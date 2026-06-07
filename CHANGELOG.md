# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.2] - 2026-06-07

### Changed
- **Repo structure**: Delete `.skill` binary files, merge `SKILL.md` + `instructions.md` into single `SKILL.md`
- **README**: Deduplicate inline reference content with links (401 → 266 lines)
- **Metadata**: Unify `metadata.author` → StronLing, sync `skill.yaml` description with `SKILL.md`
- **Version**: Bump to 1.1.2 across `SKILL.md`, `skill.yaml`, README badge

### Added
- `references/interdisciplinary-frameworks.md` — cross-disciplinary concept migration framework
- `CONTRIBUTING.md` — contribution guidelines
- China mainland npm mirror installation option in README

### Fixed
- Google Scholar alternatives (CNKI / 百度学术 / 万方) for China mainland users
- Twitter citation example replaced with 微博
- Test scenarios decoupled from Claude model names (Sonnet/Opus/Haiku → frontier/mid-tier/small)
- Updated Accessed dates from 2024 → 2026
- Fixed broken `stats.gov.cn/easyquery.htm` URL (403)
- Updated `http` → `https` for Chinese government URLs

## [1.0.0] - 2026-03-09

### Added
- **Core Framework**: Three-tier quality control system (Source Authority, Verification Protocols, Expert Methodology)
- **Source Authority System**: 
  - 150+ authoritative sources documented
  - 10-category blacklist
  - Tier 1A-F classification (academic monographs, journals, official data, legal, patents, corporate)
- **Dual Verification Protocols**:
  - Chinese data cross-validation (domestic + international)
  - Academic claim verification
  - Legal/regulatory verification
  - Corporate/financial verification
  - Historical claim verification
  - Technical/scientific verification
  - Real-time information verification
  - Multi-perspective synthesis
- **Citation Standards**: Complete formats for 15+ source types
- **Test Scenarios**: 6 evaluation scenarios with scoring rubrics
- **Documentation**:
  - Comprehensive README with badges
  - SKILL.md with AI instructions
  - 5 reference documents
  - Example research application
  - MIT License

### Features

- **Automatic Source Validation**: Identifies and rejects blacklisted sources
- **Temporal Accuracy Enforcement**: Requires timestamps and current data
- **Cross-Disciplinary Integration**: Framework bridging with theoretical justification
- **Polyphonic Presentation**: Multi-perspective synthesis with attribution
- **Chinese Research Specialization**: Dual verification for China-related topics

### Documentation

- Source authority whitelist (150+ sources)
- Source blacklist (10 categories)
- Verification protocols (8 procedures)
- Citation standards (15+ formats)
- Test scenarios (6 cases with rubrics)
- Research example (complete application)

## [Unreleased]

### Planned for 1.1.0
- Automated source verification script
- Expanded interdisciplinary frameworks
- Additional citation styles (APA, MLA, Chicago)
- Interactive source selection decision tree
- More test scenarios (target: 10+)

### Planned for 2.0.0
- Integration with Zotero/reference management
- Automated bibliography generation
- Source authority scoring algorithm
- Collaborative research features
- Real-time source validation API

---

## Version History Summary

| Version | Date | Key Changes |
|---------|------|-------------|
| 1.0.0 | 2026-03-09 | Initial release with complete framework |
