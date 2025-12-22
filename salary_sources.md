# Salary Data Sources and Update Process

This document provides references for salary data sources and instructions for keeping the IT Career Navigator repository current.

## Primary Data Sources

### U.S. Bureau of Labor Statistics (BLS)
**URL:** https://www.bls.gov/ooh/
**Update Frequency:** Annual (updated September/October each year for 10-year projections)
**Cost:** Free, publicly available

**Relevant Occupation Codes:**
- Information Security Analysts: https://www.bls.gov/ooh/computer-and-information-technology/information-security-analysts.htm
- Data Scientists: https://www.bls.gov/ooh/math/data-scientists.htm  
- Software Developers: https://www.bls.gov/ooh/computer-and-information-technology/software-developers.htm
- Network and Computer Systems Administrators: https://www.bls.gov/ooh/computer-and-information-technology/network-and-computer-systems-administrators.htm
- Database Administrators: https://www.bls.gov/ooh/computer-and-information-technology/database-administrators.htm

**What to extract:**
- Median annual wage (use as baseline for salary ranges)
- Projected growth percentage (2024-2034 currently)
- Number of jobs projection

### Glassdoor
**URL:** https://www.glassdoor.com/Salaries/
**Update Frequency:** Real-time based on user submissions
**Cost:** Some data free, detailed breakdowns require account

**Search by:** Job title + location
**Use for:** Salary ranges, company-specific compensation, total comp (base + bonus)

### Built In
**URL:** https://builtin.com/salaries
**Update Frequency:** Quarterly
**Cost:** Free

**Particularly good for:** Tech hub salaries (SF, NYC, Seattle, Austin)

### PayScale
**URL:** https://www.payscale.com/research/US/
**Update Frequency:** Continuous
**Cost:** Free for basic data

**Use for:** Experience-level breakdowns (entry vs. mid vs. senior)

### Levels.fyi
**URL:** https://www.levels.fyi/
**Update Frequency:** Real-time based on user submissions
**Cost:** Free

## Automated Update Option (Experimental)

**Note for contributors:** If you want to help automate salary data gathering, here's a starting point. This is how similar automation could work, but it requires ongoing maintenance.

### Basic BLS Scraper (Python Example)

### Quarterly (Every 3 Months)
- Spot-check 3-5 high-volatility roles (AI/ML Engineer, Cloud Architect, Prompt Engineer)
- Update any salary ranges that have shifted >10%
- Review recent tech layoffs/hiring trends

### Annually (September/October)
- Full update of all 15 role salary ranges
- Update BLS growth projections when new 10-year outlook is released
- Update all references to data year (e.g., "early 2025" → "early 2026")
- Review and update AI Impact Analysis percentages
- Update Career Trends document with new market patterns

## Manual Update Process

### Step 1: Research Current Salaries
For each role, check 2-3 sources and calculate:
- **Low end:** 25th percentile or entry-level (2-3 years experience)
- **High end:** 75th percentile or senior level (7-10 years experience)

### Step 2: Update README.md
Edit the main salary table with new ranges:
```bash
cd /opt/sideprojects/IT-Tech-Positions
nano README.md  # or your preferred editor
```

Look for lines like:
```markdown
| 2 | **[AI/ML Engineer](Roles/AIML_Engineer.md)** | **$135,000 - $210,000+** | ...
```

### Step 3: Update Individual Role Files
Edit each role file in `Roles/` directory:
```bash
nano Roles/AIML_Engineer.md
```

Update the "Role Snapshot & Outlook" table.

### Step 4: Update Data References
Update the disclaimer section in README.md to reflect current data year.

### Step 5: Commit Changes to Git
```bash
git add .
git commit -m "Update salary data for Q[X] 202[X] - BLS projections and market research"
git push origin main
```

## Automated Update Option (Experimental)

### Basic BLS Scraper (Python)
A simple Python script could automate BLS median wage extraction:

```python
#!/usr/bin/env python3
import requests
from bs4 import BeautifulSoup

# Example for Data Scientists
url = "https://www.bls.gov/ooh/math/data-scientists.htm"
response = requests.get(url)
soup = BeautifulSoup(response.content, 'html.parser')

# BLS uses specific tags for median pay
# This is a simplified example - actual implementation needs robust parsing
median_pay_section = soup.find('p', class_='sub-content-type-callout')
if median_pay_section:
    print(f"Median Pay: {median_pay_section.text}")
```

**Note:** This is fragile and breaks when BLS changes their HTML structure. Manual review is recommended.

### Limitations of Automation
- **Paywalls:** Glassdoor, Built In, and others limit API/scraping access
- **Context:** Salary ranges require human judgment (regional variations, experience levels)
- **Quality:** Machine-scraped data needs validation

**Recommendation:** Use automation for **data gathering**, but require human review before committing changes.

## Contact for Questions

For questions about data sources or update process, file an issue on the GitHub repository or contact the repository maintainer.

---

**Last Updated:** December 2025
**Next Scheduled Review:** March 2026 (Q1 2026)
