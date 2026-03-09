# Source Blacklist (Absolute Prohibited)

**CRITICAL**: Under no circumstances should these sources be cited or used as authoritative information.

## Category 1: Chinese Web Encyclopedias

**Strictly Forbidden**:
- 百度百科 (Baidu Baike)
- 搜狗百科 (Sogou Baike)
- 头条百科 (Toutiao Baike)
- 快懂百科 (Kaidong Baike)
- 360百科 (360 Baike)
- 维基百科中文镜像 (Wikipedia Chinese mirrors)
- 互动百科 (Hudong Baike) [defunct but archived content remains]

**Why**: Crowdsourced, no peer review, frequent errors, anonymous authorship, commercial manipulation.

---

## Category 2: Content Aggregation Platforms

**Strictly Forbidden**:
- 今日头条 (Toutiao)
- 腾讯新闻 (Tencent News) - **unless citing original Xinhua/CCTV source**
- 网易号 (NetEase号)
- 搜狐号 (Sohu号)
- 百家号 (Baijiahao)
- 新浪看点 (Sina Kandian)
- 一点资讯 (Yidian Zixun)
- 趣头条 (Qutoutiao)

**Why**: Algorithmic aggregation of unknown sources, clickbait optimization, no editorial standards, frequent plagiarism.

**Exception**: If Tencent News explicitly attributes to Xinhua, People's Daily, or CCTV original report, trace to original source.

---

## Category 3: Q&A and Community Platforms

**Strictly Forbidden**:
- 知乎 (Zhihu) - **all content including "verified" answers**
- 百度知道 (Baidu Zhidao)
- 悟空问答 (Wukong Wenda)
- 搜狗问问 (Sogou Wenwen)
- 天涯问答 (Tianya) [archived]
- Quora Chinese content

**Why**: User-generated content, no verification mechanism, opinion presented as fact, rampant misinformation even from "verified" users.

---

## Category 4: Social Media and Short Video

**Strictly Forbidden**:
- 抖音 (Douyin/TikTok) - **all content except official government accounts**
- 快手 (Kuaishou)
- 小红书 (Xiaohongshu)
- 微博 (Weibo) - **non-official accounts only**; official accounts (e.g., @人民日报) are permitted
- Bilibili - **non-academic UP主 content only**; university channels and academic lectures are permitted
- 微信视频号 (WeChat Channels)

**Why**: Entertainment-optimized, algorithm-driven, no fact-checking, influencer marketing disguised as information.

**Exception**: Official government accounts (verified with blue V and government badge) are authoritative.

---

## Category 5: Document Sharing Platforms

**Strictly Forbidden**:
- 道客巴巴 (Doc88)
- 原创力文档 (Original Doc)
- 百度文库 (Baidu Wenku)
- 豆丁网 (Douding)
- 爱问共享资料 (iAsk)
- MBA智库文档

**Why**: Copyright violations, document quality unverified, frequent academic paper piracy with errors, no peer review.

---

## Category 6: Technical Blogs and Forums

**Strictly Forbidden**:
- CSDN博客 (CSDN Blog) - **all content**
- 博客园 (CNBlogs)
- 简书 (Jianshu)
- 开源中国 (OSChina) - **community content only**
- 掘金 (Juejin) - **for factual claims**
- 思否 (SegmentFault)

**Why**: Tutorial-focused, often outdated, no verification, frequently copy-pasted from unknown sources.

**Exception**: Can reference for code examples with explicit testing, but never for factual claims about technologies, companies, or markets.

---

## Category 7: Financial and Business Portals (Non-Official)

**Strictly Forbidden**:
- 东方财富网自媒体频道 (East Money self-media)
- 同花顺财经号 (10jqka finance accounts)
- 雪球 (Xueqiu) - **non-verified users only**
- 和讯网博客 (Hexun blogs)
- 金融界博客 (JRJ blogs)
- 新浪财经博客 (Sina Finance blogs)

**Why**: Rampant manipulation, paid promotion disguised as analysis, no accountability for predictions, frequently violate securities regulations.

**Exception**: 
- Snowball verified institutional accounts (with verification badge)
- East Money official data center (e.g., 数据中心 → 官方统计)
- Trace all claims to primary sources (company filings, exchange data)

---

## Category 8: Academic Paper Mills and Predatory Journals

**Strictly Forbidden**:
- 所有 "论文网"、"代写代发" 网站
- Beall's List predatory journals (Chinese language variants)
- 没有DOI或无法通过Crossref验证的 "期刊"
- 会议论文声称被 "EI收录" 但无法 Engineering Village 验证

**Why**: Academic fraud, no peer review, pay-to-publish, damage to research integrity.

---

## Category 9: Translation and Summary Sites

**Strictly Forbidden**:
- 彩云小译、DeepL等翻译平台社区内容
- 各种 "X分钟读完一本书" 网站
- 学术论文 "解读" 网站（未经原作者授权）

**Why**: Translation errors, loss of nuance, cherry-picking, frequent misrepresentation of original arguments.

**Exception**: Machine translation tools (Google Translate, DeepL) can be used to assist reading, but original source must be cited, not the translation.

---

## Category 10: AI-Generated Content Platforms

**Strictly Forbidden**:
- 文心一言、通义千问等AI平台的社区分享内容
- ChatGPT对话截图作为 "权威回答"
- 各种AI写作工具生成的 "分析报告"
- AI生成内容循环引用（AIGC citing AIGC）

**Why**: Hallucinations, no verification, circular reasoning, training data cutoffs.

**Exception**: AI tools can assist in research process (translation, summarization, brainstorming), but all factual claims must be independently verified with authoritative sources.

---

## Detection Rules

### Automatic Red Flags

**URL Patterns to Reject**:
```
*baike.baidu.com/*
*zhihu.com/*
*zhihu.com/question/*
*daodu.baidu.com/*
*doc88.com/*
*wenku.baidu.com/*
*book118.com/*
*csdn.net/*
*blog.csdn.net/*
*jianshu.com/*
*mp.weixin.qq.com/* (unless verified official account)
*weibo.com/* (unless verified blue V government)
*toutiao.com/*
*douyin.com/*
*xiaohongshu.com/*
```

**Content Patterns to Reject**:
- "小编了解到..." (No author attribution)
- "有网友表示..." (Anonymous sourcing)
- "据统计..." (Without citation)
- "专家认为..." (Without naming expert)
- 大量感叹号、emoji堆砌的内容
- 明显AI生成痕迹（过度结构化、空洞套话）

### Verification Protocol

**Before Using Any Source**:
1. Check URL against blacklist above
2. Verify if source has editorial board (academic journals)
3. Verify if source has government authorization (official statistics)
4. Check for peer review process (academic)
5. Check for original data collection methodology (research)
6. Verify author credentials and affiliations
7. Check publication date and update history

**If Uncertain**: 
- Do not use the source
- Search for the same information in authoritative sources
- When in doubt, leave it out

---

## Consequences of Violation

Using blacklisted sources compromises:
- **Research Integrity**: Contaminated data foundation
- **Factual Accuracy**: Unverified claims become "facts"
- **Professional Credibility**: Loss of trust from informed readers
- **Cross-Verification**: Cannot pass dual-verification protocols

**Policy**: If blacklisted source is detected during research, immediately discard and search for authoritative alternative.

---

## Related Documents

- [source-authority.md](source-authority.md) - Whitelist of authoritative sources
- [verification-protocols.md](verification-protocols.md) - How to verify source legitimacy
- [interdisciplinary-frameworks.md](interdisciplinary-frameworks.md) - Cross-disciplinary source evaluation

---

*Last Updated: 2026-03-09*
*Version: 1.0*
