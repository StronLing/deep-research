# Scholarly Excellence Framework

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-blue.svg)]()
[![Category: Research](https://img.shields.io/badge/Category-Research-green.svg)]()

> Achieve scholarly excellence with global top-tier interdisciplinary research standards. Enforces authoritative source mandates, dual verification protocols, and polyphonic expertise synthesis.

## Overview

This skill enforces rigorous research methodology including:
- **Source Authority Mandates** - Strict whitelist/blacklist for information sources
- **Temporal Accuracy** - Real-time verification and timestamp standards
- **Dual Verification Protocols** - Mandatory cross-validation for Chinese/international data
- **Polyphonic Expertise** - Multi-perspective synthesis with proper attribution
- **Cross-Disciplinary Integration** - Bridging frameworks with theoretical justification

## Installation

```bash
# Default (GitHub)
npx skills add StronLing/deep-research -g

# China mainland (use npm mirror if GitHub is slow)
npx --registry https://registry.npmmirror.com/ skills add StronLing/deep-research -g

# Install from local clone
git clone https://github.com/StronLing/deep-research.git
cd deep-research
npx skills add . -g
```

## When to Use This Skill

Use this skill when:
- Answering complex questions requiring authoritative sources
- Conducting cross-disciplinary research synthesis
- Handling Chinese data requiring international verification
- Presenting academic consensus and dissent fairly
- Writing research papers, reports, or policy briefs
- Fact-checking claims with primary sources

## Core Framework

### Three-Tier Quality Control

**Tier 1: Source Authority**
- Whitelist: Academic monographs, top journals, official databases
- Blacklist: Web encyclopedias, social media, content aggregators
- Chinese exception: Government sources, core journals, authoritative scholars

**Tier 2: Verification Protocols**
- Dual verification for Chinese topics (domestic + international)
- Triple verification for key data points
- Real-time information retrieval
- Timestamp all historical data

**Tier 3: Expert Methodology**
- Polyphonic presentation (consensus + dissent)
- Cross-disciplinary concept migration
- Practitioner + academic perspectives
- Uncertainty acknowledgment

## Quick Start

### Basic Research Query

```
User: "分析中国半导体产业现状"

Skill Actions:
1. Retrieve: 国家统计局 + OECD + SEMI data
2. Cross-validate: Production capacity, import dependency, policy documents
3. Academic sources: *Cambridge History of China* + *Journal of Chinese Economic Studies*
4. Present: Multiple expert viewpoints with attribution
5. Format: Chinese output with professional terms in original language
```

### Research Report Structure

```
1. Executive Summary
2. Data Sources & Methodology
3. Findings (with triangulation)
4. Multi-Perspective Analysis
5. Limitations & Uncertainties
6. Citations (full attribution)
```

## File Structure

```
deep-research/
├── SKILL.md                              # Core AI instructions
├── README.md                             # Human guide
├── CONTRIBUTING.md                       # Contribution guidelines
├── CHANGELOG.md                          # Version history
├── skill.yaml                            # Skill metadata
├── references/
│   ├── source-authority.md               # Detailed whitelist (150+ sources)
│   ├── source-blacklist.md               # Prohibited sources (10 categories)
│   ├── verification-protocols.md         # 8 verification procedures
│   ├── citation-standards.md             # Citation formats by source type
│   └── interdisciplinary-frameworks.md   # Cross-disciplinary mappings
├── examples/
│   └── research-example.md               # Complete research application
└── tests/
    └── scenarios.md                      # 6 test scenarios for evaluation
```

## Source Categories

Sources are classified into three tiers. See [references/source-authority.md](references/source-authority.md) for the full 150+ source whitelist and [references/source-blacklist.md](references/source-blacklist.md) for the 10-category prohibited list.

| Tier | Description | Examples |
|------|-------------|----------|
| **Tier 1** | Authoritative (mandatory priority) | Academic monographs, top journals, government databases, patents |
| **Tier 2** | Conditionally permitted | CNKI core journals, government white papers, corporate filings |
| **Tier 3** | Strictly prohibited | Web encyclopedias, social media, content aggregators, AI-generated content |

## Verification Protocols

Eight step-by-step procedures for verifying claims across domains (Chinese data, academic, legal, corporate, historical, technical, real-time, multi-perspective synthesis). See [references/verification-protocols.md](references/verification-protocols.md).

## Citation Standards

Complete citation formats for 15+ source types (academic, government, legal, corporate, archival, technical, web). See [references/citation-standards.md](references/citation-standards.md).

## Cross-Disciplinary Integration

Frameworks for responsible concept migration between disciplines. See [references/interdisciplinary-frameworks.md](references/interdisciplinary-frameworks.md).

## Anti-Patterns

❌ **Single-source claims**: No cross-validation
❌ **Timestamp omission**: Historical data without "as of" date
❌ **Attribution failure**: Views without scholar/school identification
❌ **Circular citations**: AI content citing other AI content
❌ **Aggregator dependence**: Using news portals as primary sources
❌ **Methodological confusion**: Mixing definitions without explanation

## Use Cases

### Use Case 1: Economic Analysis

**Query**: "分析中国房地产政策效果"

**Application**:
- Stats Bureau data + IMF/OECD housing reports
- Chinese legal database for policy texts
- Academic: *China Quarterly* + *Journal of Urban Economics*
- Present: Keynesian vs. Austrian school interpretations

### Use Case 2: Historical Research

**Query**: "明清时期的社会救济制度"

**Application**:
- 夫馬進专著 (primary)
- *Cambridge History of China* (cross-validation)
- Ming/Qing archives (primary documents)
- Present: Different historiographical schools

### Use Case 3: Technology Assessment

**Query**: "台积电3nm工艺技术参数"

**Application**:
- TSMC official investor presentations
- IEEE Xplore technical papers
- USPTO patent filings
- Present: Engineering vs. economic feasibility perspectives

## Related Skills

- `web-search` - For retrieving current information
- `pdf` - For processing academic documents
- `xlsx` - For analyzing statistical data
- `ms-office-suite` - For report formatting

## Features

### Core Capabilities

| Feature | Description | Status |
|---------|-------------|--------|
| **Source Authority Control** | Strict whitelist/blacklist with 150+ authoritative sources | ✅ |
| **Dual Verification** | Automatic Chinese/international source cross-validation | ✅ |
| **Temporal Accuracy** | Real-time verification with timestamp standards | ✅ |
| **Polyphonic Synthesis** | Multi-perspective presentation with proper attribution | ✅ |
| **Cross-Disciplinary Integration** | Framework bridging with theoretical justification | ✅ |
| **Citation Standards** | Complete citation formats for 15+ source types | ✅ |
| **Test Scenarios** | 6 evaluation scenarios with scoring rubrics | ✅ |

### Supported Domains

- **Economics & Finance**: GDP, trade, monetary policy, corporate finance
- **Law & Regulation**: Chinese law, US law, EU law, international treaties
- **History**: Chinese history (esp. Ming-Qing), European history, comparative history
- **Science & Technology**: Engineering standards, patents, technical specifications
- **Social Sciences**: Sociology, political science, international relations

### Special Protocols

| Protocol | Trigger | Action |
|----------|---------|--------|
| **Chinese History Verification** | Chinese historical topics | Retrieve English Sinology + Chinese authoritative sources |
| **Economic Data Cross-Check** | Chinese economic data | Cross-validate stats.gov.cn with OECD/World Bank/IMF |
| **Legal Source Verification** | Legal questions | Cite flk.npc.gov.cn (China) or Cornell LII (US) |
| **Technical Parameter Check** | Science/Engineering | Verify through IEEE/ISO/patent databases |
| **Conflict Resolution** | Divergent sources | Present range with methodological analysis |

## Roadmap

### Version 1.1 (Planned)
- [ ] Add automated source verification script
- [ ] Expand interdisciplinary frameworks (physics→economics, biology→sociology)
- [ ] Add more citation styles (APA, MLA, Chicago)
- [ ] Create interactive decision tree for source selection

### Version 1.2 (Planned)
- [ ] Add real-time source validation API
- [ ] Expand test scenarios to 10+
- [ ] Add domain-specific templates (legal briefs, policy memos, investment reports)
- [ ] Multi-language support expansion (German, French, Japanese citation standards)

### Version 2.0 (Future)
- [ ] Integration with Zotero/reference management
- [ ] Automated bibliography generation
- [ ] Source authority scoring algorithm
- [ ] Collaborative research features

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on reporting issues, suggesting sources, and submitting changes.

## Acknowledgments

This framework synthesizes best practices from:
- **German Historical School** (source criticism methodology)
- **Anglo-American Legal Tradition** (precedent and citation standards)
- **Chinese Historiography** (夫馬進, 宫崎市定 et al.)
- **Modern Data Journalism** (verification and transparency standards)
- **Academic Peer Review** (quality control mechanisms)

## Support & Community

- **Documentation**: [Full documentation](https://skills.sh/StronLing/deep-research)
- **Issues**: [GitHub Issues](https://github.com/StronLing/deep-research/issues)
- **Discussions**: [GitHub Discussions](https://github.com/StronLing/deep-research/discussions)

## Version History

See [CHANGELOG.md](CHANGELOG.md) for detailed version history.

## License

MIT License - See [LICENSE](LICENSE) for details

---

**Cite This Skill**:
```
StronLing (2026), "Scholarly Excellence Framework: Global Top-Tier Interdisciplinary Research Standards", 
Version 1.0.0, https://skills.sh/StronLing/deep-research
```
