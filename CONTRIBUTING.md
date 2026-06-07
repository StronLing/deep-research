# Contributing to Scholarly Excellence Framework

Thank you for your interest in improving research quality standards.

## How to Contribute

### Report Issues

Found a blacklisted source being used? Missing authoritative source in the whitelist? [Open an issue](https://github.com/StronLing/deep-research/issues) with:

- Clear description of the problem
- Relevant source/domain
- Suggested fix (if applicable)

### Suggest Sources

Propose additions to the whitelist with:

1. **Source name and URL**
2. **Authority justification**: Why should this source be considered authoritative?
3. **Domain coverage**: Which research areas does it serve?
4. **Verification**: Can claims from this source be independently verified?

### Improve Documentation

- Clarify existing protocols with better examples
- Add translations of key terms
- Fix broken links or outdated URLs
- Improve formatting and readability

### Add Test Scenarios

Contribute evaluation cases for specific domains:

1. **Domain**: What research area does this test?
2. **Query**: What question would a user ask?
3. **Expected Behaviors**: What should the skill do?
4. **Quality Criteria**: How to score the response (Minimum / Quality / Excellent)
5. **Haiku Pitfall**: What would a weaker model get wrong?

## Guidelines

### Source Additions

- Must include DOI/URL and justification for authority
- Must not duplicate existing entries
- Should serve a currently underserved domain

### Protocol Changes

- Must maintain backward compatibility or version appropriately
- Should include example demonstrating the change
- Must not weaken existing quality standards

### Citation Formats

- Follow established academic standards (Chicago, APA, or domain-specific)
- Include at least one example per format
- Note any discipline-specific variations

### Code of Conduct

- Prioritize factual accuracy over speed
- Respect intellectual property and attribution
- Acknowledge limitations and uncertainty
- Maintain neutrality in presenting contested views

## Development Workflow

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-change`)
3. Make your changes
4. Test with the [test scenarios](tests/scenarios.md) if applicable
5. Submit a pull request with a clear description

## Questions?

Open a [discussion](https://github.com/StronLing/deep-research/discussions) for questions about contributing.
