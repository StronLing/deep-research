# Test Scenarios

Test scenarios for evaluating skill quality across different models.

## Scenario 1: Chinese Economic Data Query

**Difficulty**: Medium  
**Domain**: Economics, China Studies

### Query
"What was China's GDP growth rate in 2023, and how does it compare to government targets?"

### Expected Behaviors

#### 1. Dual Verification Protocol
- **Minimum**: Retrieve at least one Chinese source and one international source
- **Quality criteria**: 
  - Chinese: stats.gov.cn official release
  - International: World Bank or OECD data
  - Explicit cross-comparison
- **Haiku pitfall**: Only retrieves Baidu Baike or Zhihu summary
- **Weight**: 5 (critical)

#### 2. Temporal Accuracy
- **Minimum**: States figure as "2023" without specifying preliminary/final
- **Quality criteria**: 
  - Notes "5.2% (National Bureau of Statistics, final figure, January 2024)"
  - Distinguishes preliminary vs. final
- **Haiku pitfall**: Uses outdated preliminary figures
- **Weight**: 4

#### 3. Policy Context
- **Minimum**: Mentions "around 5% target"
- **Quality criteria**: 
  - Cites specific target from Government Work Report
  - Discusses whether target was met
  - References relevant policy context
- **Haiku pitfall**: No policy context at all
- **Weight**: 3

#### 4. Citation Format
- **Minimum**: Mentions sources informally
- **Quality criteria**: 
  - Proper citation format for both Chinese and international sources
  - Access dates included
  - URLs or database references
- **Haiku pitfall**: No citations or only "according to reports"
- **Weight**: 4

### Output Validation
- Must include: stats.gov.cn citation
- Must include: World Bank or OECD citation
- Must not include: Baidu Baike, Zhihu, or news aggregator as primary source
- Pattern check: `stats.gov.cn|data.stats.gov.cn` AND `worldbank.org|oecd.org|imf.org`

---

## Scenario 2: Chinese Historical Claim

**Difficulty**: Hard  
**Domain**: History, Sinology

### Query
"How did the Ming Dynasty civil service examination system work?"

### Expected Behaviors

#### 1. Dual Verification (Chinese History Protocol)
- **Minimum**: Cites at least one English-language academic source
- **Quality criteria**: 
  - International Sinology: *Cambridge History of China* or equivalent
  - Chinese authoritative: 中华书局点校本 or CSSCI journal
  - Explicit comparison of perspectives
- **Haiku pitfall**: Only cites Chinese web encyclopedia or popular history book
- **Weight**: 5 (critical)

#### 2. Primary Source Reference
- **Minimum**: Mentions Ming Dynasty records generally
- **Quality criteria**: 
  - Specific reference to 《明实录》 or 《明史》
  - Notes edition (e.g., 中华书局点校本)
  - Cites specific historian's analysis of primary sources
- **Haiku pitfall**: No primary source awareness
- **Weight**: 4

#### 3. Scholarly Attribution
- **Minimum**: Mentions "historians say"
- **Quality criteria**: 
  - Names specific scholars (e.g., 宫崎市定, Ping-ti Ho)
  - Attributes specific interpretations to named scholars
  - Notes different historiographical schools
- **Haiku pitfall**: General claims without attribution
- **Weight**: 4

#### 4. Conceptual Nuance
- **Minimum**: Describes three-tier examination system
- **Quality criteria**: 
  - Distinguishes 童试/乡试/会试/殿试
  - Discusses social mobility debate
  - References regional variations
- **Haiku pitfall**: Oversimplified description
- **Weight**: 3

### Output Validation
- Must include: English-language academic monograph or Cambridge History reference
- Must include: Primary source reference (Ming Shilu or Ming Shi)
- Must not include: Baidu Baike, Chinese Wikipedia, or general web article
- Pattern check: `Cambridge History of China|宫崎|Miyazaki|Elman|Ho Ping-ti`

---

## Scenario 3: Cross-Disciplinary Synthesis

**Difficulty**: Hard  
**Domain**: Economics, Law, Political Science

### Query
"How do trust law principles apply to blockchain governance structures?"

### Expected Behaviors

#### 1. Cross-Disciplinary Integration
- **Minimum**: Mentions both legal trusts and blockchain
- **Quality criteria**: 
  - Legal framework: Maitland on trusts or modern trust law principles
  - Technical: Academic blockchain governance literature
  - Explicit bridge between concepts
- **Haiku pitfall**: Only describes one domain superficially
- **Weight**: 5 (critical)

#### 2. Concept Migration Justification
- **Minimum**: States "trusts are like blockchain governance"
- **Quality criteria**: 
  - Explains theoretical basis for analogy
  - Notes applicable boundaries
  - Discusses limitations of analogy
- **Haiku pitfall**: No theoretical justification
- **Weight**: 4

#### 3. Multiple Perspectives
- **Minimum**: Presents one view on application
- **Quality criteria**: 
  - Legal perspective: property vs. contract theory of trusts
  - Technical perspective: code-is-law vs. governance models
  - Regulatory perspective: SEC, EU approaches
- **Haiku pitfall**: Single perspective presented as truth
- **Weight**: 4

#### 4. Practitioner vs. Academic
- **Minimum**: All academic or all practitioner sources
- **Quality criteria**: 
  - Academic legal theory
  - Industry practitioner perspectives
  - Regulatory viewpoints
- **Haiku pitfall**: Only news articles or blog posts
- **Weight**: 3

### Output Validation
- Must include: Legal academic source (law review or Maitland/Milsom)
- Must include: Technical academic source (IEEE, peer-reviewed CS paper)
- Must not include: Crypto blogs, Medium posts, unverified claims
- Pattern check: `trust|fiduciary` AND `blockchain|governance|DAO`

---

## Scenario 4: Conflicting Data Scenario

**Difficulty**: Hard  
**Domain**: Economics, International Relations

### Query
"What is the current status of China-US trade volume?"

### Expected Behaviors

#### 1. Conflict Identification
- **Minimum**: Presents one figure
- **Quality criteria**: 
  - Acknowledges multiple measurement methodologies
  - Notes divergence between Chinese and US reported figures
  - Explains reasons for discrepancy (FOB vs. CIF, HK transshipment, etc.)
- **Haiku pitfall**: Single figure without context
- **Weight**: 5 (critical)

#### 2. Dual Reporting
- **Minimum**: Mentions "China says X, US says Y"
- **Quality criteria**: 
  - Specific figures from General Administration of Customs (China)
  - Specific figures from US Census Bureau
  - Analysis of methodological differences
- **Haiku pitfall**: Uses third-party aggregator without noting source conflict
- **Weight**: 5 (critical)

#### 3. Methodological Transparency
- **Minimum**: Notes "different calculation methods"
- **Quality criteria**: 
  - Explains FOB vs. CIF valuation
  - Discusses Hong Kong re-export issue
  - Notes timing differences in reporting
- **Haiku pitfall**: No methodological discussion
- **Weight**: 4

#### 4. Presentation of Range
- **Minimum**: Presents single "best estimate"
- **Quality criteria**: 
  - Presents range: "China reports $X, US reports $Y"
  - Notes which methodology is used by which organization
  - Avoids false precision
- **Haiku pitfall**: Arbitrary selection without justification
- **Weight**: 3

### Output Validation
- Must include: Chinese Customs data citation
- Must include: US Census Bureau or ITA data citation
- Must acknowledge: Discrepancy between sources
- Pattern check: `customs.gov.cn|census.gov|trade.gov` AND `discrepancy|differ|methodology`

---

## Scenario 5: Legal Text Interpretation

**Difficulty**: Medium  
**Domain**: Law, China Studies

### Query
"What does Article 1165 of the Chinese Civil Code say about tort liability?"

### Expected Behaviors

#### 1. Primary Source Citation
- **Minimum**: Summarizes Article 1165
- **Quality criteria**: 
  - Direct citation from flk.npc.gov.cn (National Laws Database)
  - Quotes official text
  - Notes effective date (2021-01-01)
- **Haiku pitfall**: Cites second-hand summary or legal blog
- **Weight**: 5 (critical)

#### 2. English Translation Comparison
- **Minimum**: Provides one English version
- **Quality criteria**: 
  - Notes official translation vs. scholarly translation
  - Cites specific translation (e.g., NPC official, Chinalawinfo)
  - Notes translation difficulties if relevant
- **Haiku pitfall**: Translation without attribution
- **Weight**: 3

#### 3. Academic Legal Commentary
- **Minimum**: General explanation of fault liability
- **Quality criteria**: 
  - Cites Chinese legal scholar (e.g., 王利明, 杨立新)
  - References comparative law perspective
  - Notes implementation issues
- **Haiku pitfall**: No scholarly commentary
- **Weight**: 4

#### 4. Contextual Placement
- **Minimum**: Discusses Article 1165 in isolation
- **Quality criteria**: 
  - Places within Chapter VI (Tort Liability)
  - Contrasts with previous Tort Liability Law
  - References related articles (1166, 1167, etc.)
- **Haiku pitfall**: No context
- **Weight**: 3

### Output Validation
- Must include: flk.npc.gov.cn citation
- Must include: Direct quotation or accurate paraphrase with attribution
- Must not include: Law blog, legal service website, or unverified translation
- Pattern check: `flk.npc.gov.cn|民法典.*第1165条`

---

## Scenario 6: Technical/Scientific Claim

**Difficulty**: Medium  
**Domain**: Science, Technology

### Query
"What is the current state of TSMC's 3nm chip production?"

### Expected Behaviors

#### 1. Corporate Primary Source
- **Minimum**: Cites news article about TSMC
- **Quality criteria**: 
  - TSMC official investor presentation or 20-F filing
  - Specific data on yield rates, capacity, customers
  - Distinguishes announced vs. actual production
- **Haiku pitfall**: Only tech media reports
- **Weight**: 5 (critical)

#### 2. Technical Parameter Verification
- **Minimum**: Mentions "3nm" generally
- **Quality criteria**: 
  - Specific technical parameters (transistor density, power consumption)
  - Comparison with previous node (5nm)
  - Industry benchmarks (IEDM papers, IEEE)
- **Haiku pitfall**: Marketing specs without technical sourcing
- **Weight**: 4

#### 3. Industry Context
- **Minimum**: Discusses TSMC in isolation
- **Quality criteria**: 
  - Competitive landscape (Samsung, Intel)
  - Customer adoption (Apple, AMD, etc.)
  - Industry analyst reports (with appropriate caveats)
- **Haiku pitfall**: No competitive context
- **Weight**: 3

#### 4. Temporal Specificity
- **Minimum**: Current status as of vague "now"
- **Quality criteria**: 
  - Notes specific quarter (e.g., Q4 2023)
  - Distinguishes roadmap vs. current production
  - Acknowledges rapid changes in semiconductor industry
- **Haiku pitfall**: Outdated information presented as current
- **Weight**: 4

### Output Validation
- Must include: TSMC official filing or investor material citation
- Must include: Technical specification with source
- Must not include: Tech blog, unverified leak, or speculation
- Pattern check: `tsmc.com|sec.gov.*2330|20-F|investor.*tsmc`

---

## Evaluation Scoring

### Score Calculation

For each scenario:
```
Total Score = Σ (Weight × Quality Level)

Quality Levels:
- 0: Not attempted / Failed (used blacklisted source)
- 1: Minimum criteria met
- 2: Good quality criteria met
- 3: Excellent quality with nuanced analysis
```

### Model Comparison Benchmarks

| Model | Scenario 1 | Scenario 2 | Scenario 3 | Scenario 4 | Scenario 5 | Scenario 6 | Total |
|-------|-----------|-----------|-----------|-----------|-----------|-----------|-------|
| Sonnet | Target: 85%+ | Target: 80%+ | Target: 75%+ | Target: 80%+ | Target: 90%+ | Target: 85%+ | Target: 82%+ |
| Opus | Target: 90%+ | Target: 85%+ | Target: 80%+ | Target: 85%+ | Target: 95%+ | Target: 90%+ | Target: 87%+ |
| Haiku | Target: 60%+ | Target: 50%+ | Target: 45%+ | Target: 55%+ | Target: 70%+ | Target: 60%+ | Target: 57%+ |

### Pass/Fail Criteria

**Minimum Passing Score**: 60% of total possible points
**No Blacklisted Sources**: Automatic fail if any blacklisted source cited as authoritative
**Dual Verification**: Automatic fail if Chinese topic lacks dual verification

---

## Using These Scenarios

### For Skill Development
1. Run each scenario through skill
2. Score against rubric
3. Identify failure modes
4. Refine SKILL.md to address gaps

### For Model Evaluation
1. Test same scenarios across models (Sonnet, Opus, Haiku)
2. Compare scores
3. Identify model-specific limitations
4. Adjust skill instructions for model capabilities

### For Regression Testing
1. After skill updates, re-run all scenarios
2. Ensure no degradation in scores
3. Document improvements

---

*Last Updated: 2026-03-09*
*Version: 1.0*
