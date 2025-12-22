# Update Checklist for IT Tech Positions Repository

Use this checklist to keep salary data, growth projections, and career guidance current.

## Quarterly Review (Every 3 Months)

### Q1 (January - March)
- [ ] Spot-check high-volatility roles (AI/ML Engineer, Prompt Engineer, Data Engineer, SRE)
- [ ] Check levels.fyi and Glassdoor for significant salary shifts (>10%)
- [ ] Update any roles with major market changes
- [ ] **Review Industry_Trends.md** - Check for H-1B policy changes, data center news, tech layoffs, AI developments
- [ ] Update date references from "early 2025" to current quarter
- [ ] Review AI Mastery Analysis percentages

### Q2 (April - June)
- [ ] Review remote work salary trends (geographic arbitrage opportunities)
- [ ] Check for new certifications or deprecated ones
- [ ] Update Career_Trends.md with any new employment patterns
- [ ] Verify all external links are still active

### Q3 (July - September)
**MAJOR UPDATE QUARTER - BLS releases new projections**
- [ ] Update ALL salary ranges across 18 roles
- [ ] Check BLS Occupational Outlook Handbook for new 10-year projections
- [ ] Update growth projections in README and all role files
- [ ] Update AI Mastery Analysis with 6-month progress
- [ ] Refresh data freshness table in README
- [ ] Tag a new version release (e.g., v1.2-Q3-2025)

### Q4 (October - December)
- [ ] Final cleanup and minor updates for the year
- [ ] Review Getting_Started.md for outdated resources
- [ ] Check certification costs (CompTIA, AWS, etc.)
- [ ] Plan major updates for next year

---

## Data Sources to Check

### Salary Data
- [ ] [BLS Occupational Outlook Handbook](https://www.bls.gov/ooh/) - median wages, growth projections
- [ ] [Glassdoor](https://www.glassdoor.com/Salaries/) - salary ranges by role and location
- [ ] [Built In](https://builtin.com/salaries) - tech hub specific salaries
- [ ] [levels.fyi](https://www.levels.fyi/) - FAANG and startup compensation
- [ ] [PayScale](https://www.payscale.com/research/US/) - experience-level breakdowns

### Growth Projections
- [ ] BLS OOH (updated annually in September)
- [ ] Industry reports (Gartner, McKinsey, LinkedIn Emerging Jobs)
- [ ] Tech hiring trend analyses (StackOverflow Survey, GitHub Octoverse)

### AI Impact
- [ ] OpenAI/Anthropic research papers on AI capabilities
- [ ] GitHub Copilot usage statistics
- [ ] Developer productivity studies
- [ ] AI coding assistant market reports

---

## Files That Need Regular Updates

### High Priority (Update Quarterly)
- [ ] README.md - salary table for all 18 roles
- [ ] AI_Mastery_Analysis.md - mastery percentages
- [ ] Career_Trends.md - job tenure patterns, remote work trends
- [ ] **Industry_Trends.md** - H-1B policy, data centers, tech layoffs, AI impact, cybersecurity threats

### Medium Priority (Update Semi-Annually)
- [ ] All 18 role files in `/Roles/` - salary snapshots and outlook
- [ ] Getting_Started.md - resource links, certification costs
- [ ] salary_sources.md - update "Last Updated" date

### Low Priority (Update Annually)
- [ ] Interview prep resources
- [ ] Certification recommendations
- [ ] Top hiring companies lists

---

## Quick Update Process

### For Salary Updates
1. Research new salary range from 2-3 sources
2. Calculate 25th percentile (low end) and 75th percentile (high end)
3. Update README.md salary table
4. Update corresponding role file in `/Roles/`
5. Update data freshness table in README
6. Commit with message: "Update [Role] salary: $X-$Y (Q[X] 2025)"

### For BLS Projection Updates
1. Visit BLS OOH page for occupation
2. Note new growth percentage and median wage
3. Update README.md growth projection column
4. Update role file outlook section
5. Update References section if BLS URL changed
6. Commit with message: "Update BLS projections (2025-2035 outlook)"

### For AI Mastery Updates
1. Review latest AI capability reports
2. Adjust mastery percentages (typically +1-2% per 6 months)
3. Update timeline estimates if major breakthroughs occurred
4. Update AI_Mastery_Analysis.md table
5. Commit with message: "Update AI mastery percentages (current as of [Month] 2025)"

---

## Version Tagging

Tag releases quarterly to track major updates:

```bash
git tag -a v1.0 -m "Initial release - December 2024"
git tag -a v1.1 -m "Q1 2025 update - March 2025"
git tag -a v1.2 -m "Q2 2025 update - June 2025"
git tag -a v1.3 -m "Q3 2025 major update - BLS projections refresh"
git push --tags
```

---

## Automation Reminders

- Link checker GitHub Action runs weekly (checks for broken URLs)
- Set calendar reminders for quarterly reviews
- Monitor GitHub issues for community-reported outdated data

---

**Last Updated:** December 2024  
**Next Major Review:** September 2025 (BLS projection release)
