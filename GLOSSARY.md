# IT Industry Glossary

A beginner-friendly guide to common acronyms, slang, and terminology used in the IT career landscape.

---

## Companies & Organizations

**FAANG**  
Acronym for Facebook (Meta), Amazon, Apple, Netflix, Google. Refers to the five tech giants known for high salaries and competitive hiring.

**MAANG / MANGA**  
Modern variation adding Microsoft to the FAANG group.

**FAANG+**  
FAANG companies plus other high-paying tech companies like Stripe, Databricks, Coinbase, Uber, Airbnb.

**BLS**  
Bureau of Labor Statistics - US government agency that tracks employment data, salary medians, and job growth projections.

**Startup**  
Early-stage company, often tech-focused, with high growth potential but higher risk. Often offers equity instead of high salaries.

---

## Compensation & Benefits

**Total Comp (TC)**  
Total compensation = base salary + bonus + stock/equity + benefits. Example: "$150k base + $50k stock + $20k bonus = $220k TC"

**Base Salary**  
Your guaranteed annual salary before bonuses, stock, or benefits.

**RSUs (Restricted Stock Units)**  
Company stock granted as part of compensation. "Restricted" means it vests over time (typically 4 years). Common at public companies.

**Stock Options (ISO/NSO)**  
Right to buy company stock at a fixed price. Common at startups. ISO = Incentive Stock Options, NSO = Non-Qualified Stock Options (tax treatment differs).

**Vesting**  
Schedule for when stock/equity becomes yours. Common: "4-year vest with 1-year cliff" = nothing for first year, then 25%/year or monthly after that.

**Signing Bonus**  
One-time cash payment when you join a company, typically $10k-$50k+ for in-demand roles.

**Equity**  
Ownership stake in a company, usually as stock options (startups) or RSUs (public companies).

**401(k)**  
US retirement savings account. Employer often matches contributions (e.g., match 50% of first 6% you contribute = free money).

**Roth IRA**  
Individual retirement account with tax-free growth. Contribution limit $7,000/year (2025).

**HSA (Health Savings Account)**  
Tax-advantaged account for medical expenses. Triple tax benefit: deductible, tax-free growth, tax-free withdrawals for medical.

---

## Salary & Negotiation Terms

**Market Rate**  
Typical salary for a role based on location, experience, and company size. Check levels.fyi, Glassdoor, Built In.

**Comp Band / Pay Band**  
Salary range a company has budgeted for a specific role/level. Example: "L5 band is $150k-$200k"

**Geo-Arbitrage**  
Earning a high-location salary while living in low-cost area. Example: SF salary ($150k) while living in Idaho (rent $1,200 vs $3,500).

**Location-Adjusted Salary**  
Company pays different salaries based on where you live (SF = 100%, Austin = 85%, etc.).

**W2 vs 1099**  
W2 = employee (get benefits, company withholds taxes). 1099 = contractor (no benefits, you pay all taxes, but higher hourly rate).

---

## Job Levels & Roles

**IC (Individual Contributor)**  
Non-manager role. You're responsible for your own work, not managing people.

**L3, L4, L5, etc.**  
Job levels (Google/Meta system). Roughly: L3 = Junior, L4 = Mid, L5 = Senior, L6 = Staff, L7 = Senior Staff/Principal.

**Junior / Mid-Level / Senior**  
Experience levels. Junior = 0-2 years, Mid = 3-5 years, Senior = 5-8+ years.

**Staff Engineer / Principal Engineer**  
Very senior IC roles (above Senior). You influence architecture across teams/org. Salary $200k-$350k+.

**Tech Lead (TL)**  
Senior engineer who leads technical direction for a team, but may not manage people directly.

**Engineering Manager (EM)**  
People manager responsible for hiring, performance reviews, career development. May or may not code.

**TPM (Technical Program Manager)**  
Coordinates complex technical projects across teams. More process/planning, less coding.

---

## Development & Engineering

**Full-Stack Developer**  
Developer who works on both frontend (user interface) and backend (server, database).

**Frontend / Backend**  
Frontend = what users see (HTML, CSS, JavaScript, React). Backend = server logic, databases (Python, Java, Node.js).

**DevOps**  
Development + Operations. Focus on automation, CI/CD, infrastructure, deployments. Bridges dev and ops teams.

**SRE (Site Reliability Engineer)**  
Google-created role. Software engineers focused on reliability, uptime, incident response, and scaling systems.

**MLOps**  
Machine Learning Operations. DevOps for ML models - deployment, monitoring, retraining pipelines.

**API (Application Programming Interface)**  
Way for software systems to talk to each other. REST APIs and GraphQL are common types.

**Microservices**  
Architecture where app is broken into small, independent services instead of one big application ("monolith").

**CI/CD (Continuous Integration / Continuous Deployment)**  
Automated testing and deployment pipelines. Code → automated tests → deploy to production.

**Git / GitHub / GitLab**  
Version control systems for tracking code changes. Git = tool, GitHub/GitLab = platforms hosting your code.

**Pull Request (PR) / Merge Request (MR)**  
Proposed code changes for review before merging into main codebase.

**Tech Debt (Technical Debt)**  
Shortcuts or quick fixes that make code harder to maintain long-term. Like financial debt, it accumulates "interest."

**Refactoring**  
Re-writing code to be cleaner/more maintainable without changing functionality.

---

## Infrastructure & Cloud

**On-Prem (On-Premises)**  
Running servers in your own data center (vs. cloud). Less common now, higher upfront cost.

**Cloud**  
Renting servers/infrastructure from AWS, Google Cloud, or Azure instead of owning hardware.

**IaaS / PaaS / SaaS**  
Infrastructure/Platform/Software as a Service. IaaS = rent VMs, PaaS = rent platform (like Heroku), SaaS = use software (like Gmail).

**Kubernetes (K8s)**  
Container orchestration system. Manages deploying and scaling Docker containers across many servers.

**Docker / Containers**  
Package software + its dependencies into a "container" that runs the same everywhere.

**Load Balancer**  
Distributes traffic across multiple servers so no single server is overwhelmed.

**CDN (Content Delivery Network)**  
Caches content (images, videos, static files) geographically closer to users for faster load times.

---

## Site Reliability & Operations

**SLO (Service Level Objective)**  
Target for how reliable a service should be. Example: "99.9% uptime" = ~43 minutes downtime/month allowed.

**SLI (Service Level Indicator)**  
Metric used to measure service health. Example: request success rate, latency.

**Error Budget**  
Amount of unreliability you can "afford" before slowing feature velocity. If SLO = 99.9%, error budget = 0.1% failures.

**On-Call**  
Being available to respond to production incidents outside normal hours (nights, weekends). Usually rotates across team.

**Incident / Outage**  
Service failure or degradation. Severity 1 = total outage, Severity 2 = major feature broken, etc.

**Postmortem / RCA (Root Cause Analysis)**  
Document written after incident explaining what failed, why, and how to prevent it. Should be blameless.

**Runbook / Playbook**  
Step-by-step instructions for handling common issues or operational tasks.

**Toil**  
Repetitive manual work that should be automated. SREs aim to reduce toil to <50% of time.

---

## Data & Analytics

**ETL / ELT**  
Extract, Transform, Load (or Extract, Load, Transform). Moving data from sources → warehouse → usable format.

**Data Warehouse**  
Central repository for analytics data (e.g., Snowflake, BigQuery, Redshift).

**Data Lake**  
Storage for raw, unstructured data (often cheaper than warehouse, less organized).

**SQL**  
Structured Query Language. Language for querying databases. Critical skill for data roles.

**NoSQL**  
Non-relational databases (MongoDB, Cassandra). Good for unstructured data or very high scale.

**DAG (Directed Acyclic Graph)**  
In Airflow: visual representation of data pipeline tasks and their dependencies.

**Pipeline**  
Automated workflow that processes data from source → destination (e.g., API → S3 → Redshift → dashboard).

---

## AI & Machine Learning

**LLM (Large Language Model)**  
AI models like GPT, Claude, Gemini. Trained on massive text data to generate human-like text.

**Prompt Engineering**  
Writing effective instructions (prompts) to get desired output from AI models.

**Few-Shot Learning**  
Giving AI a few examples in your prompt to guide its response.

**Hallucination**  
When AI makes up false information that sounds plausible.

**Fine-Tuning**  
Customizing a pre-trained AI model on your specific data/task.

**ML (Machine Learning)**  
Branch of AI where computers learn patterns from data without explicit programming.

**Model Training**  
Process of teaching an ML model using data. Can take hours to weeks for large models.

**Inference**  
Using a trained model to make predictions on new data.

---

## Work Culture & Practices

**Agile / Scrum / Kanban**  
Project management methodologies. Agile = iterative approach, Scrum = 2-week sprints, Kanban = continuous flow.

**Sprint**  
Time-boxed work period in Scrum (typically 2 weeks). Team commits to delivering specific features.

**Standup (Daily Standup)**  
Short daily team meeting (often 15 min) where everyone shares what they're working on and any blockers.

**WFH (Work From Home)**  
Remote work. "WFH policy" = company's rules about remote work.

**Hybrid**  
Mix of office and remote work (e.g., "3 days in office, 2 days WFH").

**RTO (Return to Office)**  
Company policy requiring employees to come back to office (post-COVID trend at some companies).

**PTO (Paid Time Off)**  
Vacation days, sick days. "Unlimited PTO" = no fixed limit (but cultural pressure varies).

**PIP (Performance Improvement Plan)**  
Formal warning that your performance is below expectations. Often precedes termination if no improvement.

**Equity Refresh**  
Additional stock granted to retain employees (after initial grant vests). Common at FAANG.

---

## Hiring & Interviews

**LeetCode**  
Platform with coding interview practice problems. "LeetCode-style interview" = algorithmic problem-solving.

**System Design Interview**  
Interview where you design a large-scale system (e.g., "design Twitter"). Common for senior roles.

**Behavioral Interview**  
Interview testing soft skills and past experiences using STAR method (Situation, Task, Action, Result).

**Take-Home Assignment**  
Coding project you complete on your own time as part of interview process (2-8 hours typical).

**Whiteboard Interview**  
Solving coding problems on a whiteboard (or virtual equivalent). Often criticized but still common.

**STAR Method**  
Framework for answering behavioral questions: Situation, Task, Action, Result.

**Lowball Offer**  
Job offer significantly below market rate. Usually a sign to negotiate or walk away.

**Backfill**  
Hiring to replace someone who left. Often easier/faster than creating a new position.

---

## Remote Work & Freelancing

**Async / Asynchronous**  
Work style where team doesn't need to be online at same time. Documentation-heavy, fewer meetings.

**Overlap Hours**  
For global teams: hours when all time zones are working (e.g., 2pm-5pm UTC for US-EU overlap).

**Geo-arb (Geographic Arbitrage)**  
See "Geo-Arbitrage" in Salary section.

**Digital Nomad**  
Someone who works remotely while traveling frequently.

**Corp-to-Corp (C2C)**  
Contracting where you operate as a corporation rather than individual contractor.

---

## Certifications

**CompTIA A+, Network+, Security+**  
Entry-level IT certifications. A+ for support, Network+ for networking, Security+ for cybersecurity.

**AWS Certified (Solutions Architect, Developer, etc.)**  
Amazon Web Services cloud certifications. Very valuable for cloud/DevOps roles.

**CISSP (Certified Information Systems Security Professional)**  
Advanced cybersecurity certification. Requires 5 years experience.

**CKA (Certified Kubernetes Administrator)**  
Kubernetes certification. Valuable for DevOps/SRE roles.

---

## Slang & Informal Terms

**Yak Shaving**  
Getting sidetracked fixing unrelated problems. "I just wanted to fix the bug, but ended up yak-shaving the config system."

**Bike-shedding**  
Arguing over trivial details while ignoring important issues. From "arguing about bike shed color instead of nuclear reactor design."

**Rubber Ducking**  
Explaining your problem out loud (to a rubber duck) often reveals the solution.

**Imposter Syndrome**  
Feeling like you're not really qualified despite evidence of competence. Extremely common in tech.

**Crunch / Crunch Time**  
Period of intense overwork to meet deadline. Toxic if happens regularly.

**Greenfield Project**  
New project starting from scratch (vs. brownfield = working with existing legacy code).

**RTFM (Read The F***ing Manual)**  
Impolite way of saying "the answer is in the documentation."

**LGTM (Looks Good To Me)**  
Approval on pull request/code review.

**Nuke and Pave**  
Completely wipe and reinstall system instead of trying to fix. "I couldn't fix the config, so I nuked and paved."

**Dogfooding**  
Using your own product internally ("eating your own dog food"). Tests product before customers see it.

---

**Last Updated:** December 2024 | **Next Review:** June 2025

---

**Contributing:** If you encounter terms not listed here, open an issue or PR! See [CONTRIBUTING.md](CONTRIBUTING.md).

## Additional AI/ML Terms (Expanded)

**AI vs Machine Learning**  
AI (Artificial Intelligence) = broad concept of machines performing tasks that require human-like intelligence. Machine Learning = subset of AI where computers learn from data without explicit programming. All ML is AI, but not all AI is ML. Example: Rules-based expert system = AI but not ML. Neural network = both AI and ML.

**LLM (Large Language Model)** *(Expanded)*  
AI models trained on massive text datasets (GPT, Claude, Gemini, Llama). "Large" refers to billions/trillions of parameters. Can generate human-like text, code, translations. Foundation of ChatGPT and similar tools.

**RAG (Retrieval Augmented Generation)**  
Technique where LLM retrieves relevant information from external knowledge base before generating response. Reduces hallucinations by grounding answers in real data. Example: Instead of LLM guessing company policy, RAG retrieves actual policy document first, then generates answer based on that.

**Vibe Coding / Vibes-Based Programming**  
Informal term for coding with heavy AI assistance where you describe what you want ("vibe") and AI generates code. Less about deep understanding, more about directing AI and validating output. Controversial - critics say it produces developers who can't debug when AI gets things wrong.

**Context Window**  
Amount of text an LLM can "remember" in a conversation. Measured in tokens (~4 characters). GPT-4: 128k tokens = ~96k words. Larger context = can process longer documents, but more expensive.

**Tokens**  
Units LLMs use to process text. Roughly 1 token = 0.75 words. Used for billing: GPT-4 charges per million tokens. If your prompt is 1,000 tokens and response is 500 tokens, you're charged for 1,500 tokens.

**Temperature (in LLMs)**  
Parameter controlling randomness of AI output. Low temperature (0.1-0.3) = consistent, predictable responses. High temperature (0.8-1.0) = creative, varied responses. Set temperature based on task: code = low, creative writing = high.

**Vector Database**  
Database storing "embeddings" (numerical representations of text/images). Used in RAG systems. Popular: Pinecone, Weaviate, ChromaDB. Enables semantic search: "find documents similar to this concept" vs. keyword search.

**Embedding**  
Converting text/images into numerical vectors (arrays of numbers). Similar meanings = similar vectors. Allows computers to understand "dog" and "puppy" are related. Used in search, recommendations, RAG.

**AI Agent**  
AI system that can take actions autonomously (not just respond to prompts). Can use tools, make decisions, iterate until task complete. Example: "Book me a flight to NYC" → agent searches flights, checks calendar, books ticket without further input.

