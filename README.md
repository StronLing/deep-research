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
npx skills add StronLing/deep-research -g
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

### Tier 1: Authoritative (Mandatory Priority)

| Category | Examples |
|----------|----------|
| **Academic Monographs** | Borgolte, Maitland, 夫馬進专著 |
| **Top Journals** | Nature, Science, Cell, *Social Sciences in China* |
| **Official Data** | stats.gov.cn, OECD, World Bank, BIS |
| **Patents** | USPTO, EPO, JPO patent documents |
| **Standards** | ISO/IEC technical standards |
| **Archives** | SEC filings, FOIA documents |

### Tier 2: Conditionally Permitted

| Category | Examples | Requirements |
|----------|----------|--------------|
| **Chinese Academic** | CNKI core journals | With international peer review comparison |
| **Government White Papers** | State Council white papers | Official publication channel |
| **Corporate Reports** | Listed company 10-K/annual reports | Original filing, not news summary |

### Tier 3: Strictly Prohibited

| Category | Examples |
|----------|----------|
| **Web Encyclopedias** | Baidu Baike, all variants |
| **Social Media** | Zhihu, Xiaohongshu, Douyin, Weibo |
| **Content Aggregators** | Toutiao, Tencent News, Sohu |
| **Document Sharing** | Baidu Wenku, Doc88, Douding |
| **Finance Portals** | East Money, 10jqka (non-official) |

## Verification Protocols

### Chinese Topic Verification

**Required Steps**:
1. Retrieve Chinese authoritative source
2. Retrieve international authoritative source
3. Cross-validate for consistency
4. Document discrepancies
5. Synthesize with attribution

**Example Query Flow**:
```
Query: "中国2024年GDP增长率"

Step 1: Retrieve stats.gov.cn preliminary data
Step 2: Retrieve World Bank/OECD data for China
Step 3: Compare methodologies (coverage, revisions)
Step 4: If divergent, present range with explanation
Step 5: Cite both sources with access dates
```

### Cross-Disciplinary Research

**Concept Migration Protocol**:
1. Identify core concept in Source Discipline
2. Map to Target Discipline framework
3. State theoretical justification
4. Define applicable boundaries
5. Provide empirical examples

**Example**:
```
Concept: Entropy (Physics) → Organizational Management
Justification: Both systems exhibit irreversible disorder increase
Boundary: Only applies to closed systems with no external input
Example: Corporate bureaucracy growth without restructuring
```

## Polyphonic Presentation

### Structure Template

```markdown
## Academic Consensus
[What top experts generally agree on, with 3-5 primary citations]

## Alternative View A
[Position, with attribution to specific scholar/school]
- Key argument
- Evidence base
- Limitations

## Alternative View B
[Opposing position, with attribution]
- Key argument
- Evidence base
- Limitations

## Practitioner Perspective
[Industry/frontline view, with attribution]
- Operational constraints
- Real-world applications
- Deviation from theory

## Synthesis
[Integrated conclusion acknowledging uncertainty]
- Points of agreement
- Remaining controversies
- Implications for practice
```

## Citation Standards

### By Source Type

**Academic Monograph**:
```
Author (Year), *Title in Italics*, Place: Publisher, p.XX.
Example: Borgolte (2014), *Das europäische Mittelalter im Spannungsbogen des Vergleichs*, Berlin: Akademie Verlag, S.123.
```

**Journal Article**:
```
Author (Year), "Article Title", *Journal Name*, Vol(Issue), pp.XX-XX, DOI:xxx
Example: 夫馬進 (1997), "中国善会善堂史研究", *《史学雑誌》*, 106(3), pp.45-67.
```

**Government Database**:
```
Agency (Date), "Indicator Name", Database Name, Accessed: Date, URL
Example: 国家统计局 (2024-01-17), "2023年国内生产总值", 国家数据, Accessed: 2024-03-09, https://data.stats.gov.cn/
```

**International Organization**:
```
Organization (Year), *Report Title*, Place: Publisher, Dataset Code.
Example: OECD (2024), *Economic Outlook*, Paris: OECD Publishing, EO2024.
```

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

We welcome contributions from researchers, academics, and practitioners!

### How to Contribute

1. **Report Issues**: Found a blacklisted source being used? Missing authoritative source? Open an issue.
2. **Suggest Sources**: Propose additions to whitelist with justification
3. **Improve Documentation**: Clarify protocols, add examples
4. **Add Test Scenarios**: Contribute evaluation cases for specific domains

### Contribution Guidelines

- **Source Additions**: Must include DOI/URL and justification for authority
- **Protocol Changes**: Must maintain backward compatibility or version appropriately
- **Citation Formats**: Follow established academic standards
- **Test Scenarios**: Include minimum/quality criteria and weighting

### Code of Conduct

- Prioritize factual accuracy over speed
- Respect intellectual property and attribution
- Acknowledge limitations and uncertainty
- Maintain neutrality in presenting contested views

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

- **v1.0.0** (2026-03-09) - Initial release
  - Complete source authority framework
  - 8 verification protocols
  - 6 test scenarios
  - 150+ authoritative sources documented
  - 10-category blacklist

## License

MIT License - See [LICENSE](LICENSE) for details

---

**Cite This Skill**:
```
Research Excellence Institute (2026), "Scholarly Excellence Framework: Global Top-Tier Interdisciplinary Research Standards", 
Version 1.0.0, https://skills.sh/StronLing/deep-research
```
