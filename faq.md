# FAQ

## What projects and personal achievements are you proud of?

From a personal point of view, completing the [GFNY](/personal.md#cycling) is what I'm most proud of.
From a professional point of view, the [Balance](/projects.md#randomization-and-trial-supply-management----medidata) project is one of my greatest achievements.

## Have you managed multimillion-dollar technology budgets and vendor relationships? 

While VP of Engineering at Medidata, I managed a P&L of $30M. Approximately $5M of this budget was used for vendor relationships with Microsoft, AWS, PagerDuty, SAS, Codacy, Codecov, Pluralsight, Travis CI, and GitHub, to name a few. The remaining $25M covered headcount and was managed monthly with our finance business partner. Annual performance reviews and raises, attrition replacement, out-of-band pay increases, and pay-bias mitigation were all part of the budgeting process. Job descriptions and levels were defined as part of my engineering leadership responsibilities, and pay was indexed to Radford benchmarks across multiple geographic regions.

## Have you influenced executive decision-making to support major technology initiatives?

Yes — I have dozens of examples. I'll highlight a few here:

**Automated traceability in support of computer systems validation (CSV):** To provide data services to a sponsor or CRO, software systems must be validated under 21 CFR Part 11 and ICH E6 (R2/R3). Historically, Medidata documented this process manually using a traceability matrix that mapped requirements to design and test results. To reduce manual effort, I pitched three progressive ideas (in 2010) to the CEO and CTO after vetting them with the head of compliance and project management:

  - GitHub-to-JIRA integration: include the JIRA issue ID in a GitHub pull request so we could programmatically map requirements from JIRA tickets to system design.
  - TDD and unit tests as design specs: treat unit-test-driven development as a source of system design, in addition to its value for catching regressions.
  - BDD and Cucumber for test cases and results: leverage Selenium and Cucumber to capture screenshots and results automatically during integration and end-to-end tests.

These ideas, combined with automated deployment pipelines that generated a PIR, enabled us to build a validation portal that removed much of the busy work for testers, engineers, system administrators, and product managers. The approach reduced the code-freeze-to-deployment timeline from months to weeks, and in some cases to a single day.

**CEO pitch for a fully configurable SIMT RTSM system:** I pitched this idea to the CEO of Medidata (Glen DeVries) as part of my interview process. I was hired, put in charge of the project, and promoted to head of engineering within two years. To be fair, Glen and I had the same vision, so we were essentially cross-pitching each other on the idea. I executed our collective vision with precision, speed, and quality, which ultimately led to rapid growth to the head of a 100+ engineer organization.

## Have you presented complex technical concepts to senior leadership or non-technical stakeholders? 

Yes — dozens of times. Here are a few select examples:

 - How ML medical coding works and why operational efficiency is important for scaling systems
 - How to optimize for geo-diversity, and specifically in China, via CDNs
 - Microservice architecture and how client customizations can impact service delivery
 - Bringing cloud-native and SIMT concepts to clinical trial systems
 - Doubling team output from 10 to 20 engineers in 4 weeks — why TDD/BDD and radical automation enable rapid scaling
 - Automating traceability to improve operational efficiency and regulatory compliance

## Are you experienced in implementing security and data privacy measures in digital platforms? 

Yes — for my entire career I've worked almost exclusively in healthcare, and more specifically in clinical trials. This is one of the most heavily regulated industries because experimental drugs and devices are tested on humans. Not only could a defect in the system harm trial participants, but data leaks can compromise PHI, PII, and SPII. If a less obvious defect causes a corrupted data submission to the FDA, MHRA, or EMA, many people could experience adverse events (AEs) as a result of compromised data integrity. To operate in this space, the entire organization must conform to standards, guidance documents, and frameworks including, but not limited to:

 - HIPAA
 - HITECH
 - GDPR
 - ISO-27001/9001
 - SOC
 - ICH E6 (R2/R3)
 - FedRAMP
 - PCI DSS
 - OWASP

These standards impact every aspect of the business, but from an SDLC point of view they lead to the implementation of technologies such as:

 - FOSSA, Codacy, and Brakeman for source-code scanning
 - Dependabot and dependency graphs for security scanning and management
 - Artifactory for secure supply-chain management of software packages
 - GitHub secret scanning for secret detection
 - GHA, Travis CI, Jenkins, and GoCD for automation and orchestration of scanning tools
 - Integration with SIEM and log-aggregation tools like Sumo Logic and Graylog
 - IaC and containerization via Terraform, Docker, and Kubernetes to support easier rebuilds and upgrades of a fleet of 50,000+ virtual machines


## Have you implemented AI-driven features? 

Yes — I worked with OpenAI APIs, prompt engineering, one-shot prompting, and tool-calling to internal APIs as part of the vacation recommendation system I architected, designed, and prototyped. I'm also working with RAG, fine-tuning (FT), advanced tool-calling (MCP), and zero-shot prompting as part of the ai-me personal project to create my digital twin.

## Do you use analytics frameworks to measure ROI, user engagement, and impact? 

From a software-development point of view, I typically use DORA metrics (from the book Accelerate) to increase delivery rate and quality:

 - Lead time to change — the time it takes a commit to reach production.
 - Deployment frequency — how often changes are deployed to production.
 - Mean time to restore (MTTR) — how long it takes to recover from a failure.
 - Change failure rate — the percentage of changes that cause failures in production.

These metrics encourage shipping smaller, lower-risk, and more manageable pieces of code, which improves customer satisfaction.

From a services point of view, uniform logging standards and log aggregation enable teams to build dashboards that measure many SLIs with automated alerting for SLO violations or near violations. I typically start with a baseline 24-hour error rate of less than 0.1% and web-page response times under 500 ms at the 95th percentile. For more complex systems like ETL pipelines, component runtimes, data-update latency, and integrity-check violations are typically used.

From a financial controls point of view, I typically set team budgets (AWS/Azure cost control) and let each team manage their own "small business." Budgets are set at the start of a project and adapted over time as the product evolves.

From a user-engagement point of view, I've done A/B testing and feature toggling to experiment with varied UX workflows and staged feature releases for our change-adverse clients.

## Have you collaborated cross-functionally within the organization?

I've worked with every department and at every level of the organization, from IC to CEO.

 - Legal: developed a patent program, enabled source-code scans via FOSSA to protect IP, participated in interviews for lawsuits involving IP infringement, and advised on legal-discovery mitigation strategies.
 - Sales: conducted technology demonstrations and feasibility assessments for enterprise clients such as Alcon, Novartis, and J&J; participated in multi-year contract renewal negotiations in excess of $30M.
 - Strategy: performed technology assessments for potential acquisitions and new product directions.
 - Services: multiple engagements to improve Services (T1–T3) to Engineering (T4) handoff and resolution times; worked with senior leadership to improve CSAT scores.
 - Product: most of my cross-functional collaboration was with the product team. As a manager I was engaged with PMs in backlog grooming, long-term roadmap planning, and strategy. As VP of Engineering, my partnership with the head of product focused on strategy and ensuring alignment between engineering and product teams.
 - Project: I love data. My partners on the project management team adopted the foundation I built within my first team at Medidata (Balance/RTSM) and applied it across the organization. My emphasis on practical sprint planning and long-term forecasting gave the project team the data to provide internal and external clients confidence that we would ship on time about 95% of the time.
 - Finance: strong budget forecasting and control to manage within 1% of my allocated $30M budget; implemented lightweight cost controls to give teams ownership of their budgets and run their departments like small businesses.
 - Service Delivery: focused on CI/CD pipelines to automate deployments so an ever-growing fleet of VMs could be deployed more frequently. When I joined Medidata, we had about 5,000 VMs supporting one product, partially deployed every 8–12 weeks. When I left, we had ~50,000 VMs across five major on-premises and cloud data centers, 200+ applications, 15 frameworks, and 400+ product deployments every quarter — a 10–100x increase in fleet size and deployment cadence.
 - Compliance: worked with compliance partners to craft SOPs that satisfied regulatory standards while maintaining team efficiency and morale by eliminating busy work; designed and implemented a CIRT/IM system in JIRA and used metrics to drive CIRT RCA and mitigation implementation.
 - HR: worked with HR business partners on performance reviews, job leveling, and performance management. Multiple strategic engagement initiatives that started within my team expanded across the organization. Planning and responding to annual engagement surveys helped our 100+ person team achieve scores that outperformed the rest of the organization by double digits (CultureAmp).
 - C-suite: see [executive decision-making](#have-you-influenced-executive-decision-making-to-support-major-technology).

## Do you have experience mentoring and developing global engineering teams? Building a high-performance culture?

While VP of Engineering at Medidata, I managed a team of 100+ engineers across multiple time zones in London, Tokyo, California, Texas, Ohio, and New York/New Jersey. I've directly managed hundreds of ICs, managers, directors, and VPs throughout my career. I've hired, fired, mentored, sponsored, and performance-managed over 200 individuals and partnered with 200+ more across every part of a 2,000+ person organization.

The engineering initiatives led by our teams contributed to our Best Place to Work award on Glassdoor. Some initiatives included:
 - Brown-bag lunches
 - Developer blog (internal and external)
 - Innovation time
 - Poker/game night
 - Open-source contributions
 - A culture of celebration via grand (C-suite and department-wide) reveals
 - Eliminating tedious busy work like timesheets, process-heavy CSV deliverables, and cumbersome expense-report processes
 - A culture of communication via chat (HipChat then Slack) and memorialization in Git/GitHub/Confluence/JIRA when information needed to be persisted, enabling more asynchronous work and improved alignment
 - A culture of learning (Pluralsight subscriptions and internal promotion)
 - Clearly defined career paths and job leveling
 
## Do you have hands-on experience with full-stack development?

Yes — a little: about 25 years across a dozen tech stacks in healthcare, education, and finance.

## Are you proficient with cloud platforms such as AWS? 

Yes — though does anybody really understand the AWS or Azure user interface? How else could a company like Vercel exist?

In 2009, Medidata was among the first companies to use AWS for clinical trial data and one of the first to audit them. As the platform grew more complex, tools like Terraform, Ansible, and Capistrano became necessary to programmatically manage the services required to operate a five-nines clinical trial data platform. Manually deploying tens of thousands of resources across 100+ resource types isn't feasible unless you want most of your budget spent on a service-delivery team to manage it.

## Do you have experience leveraging nearshore or offshore engineering resources? 

Yes — I've worked with offshore teams in India to accelerate product development and compliance initiatives.

## Have you led the modernization of legacy systems to cloud-based architectures? 

Yes — Rave EDC was built in the late '90s to capture clinical trial data (EDC) and was architected as a MIST solution that was highly customizable. The system allowed custom functions written in C# to execute within the application server layer. When I assumed responsibility for this application in 2013, thousands of clinical trials were running on the platform, some spanning 10+ years. Evolving a platform of this scale required surgical precision.

 - Overhauled the status roll-up engine to be 10x faster and less impactful to transactional workloads
 - Sandboxed the custom-function engine to prevent it from affecting an entire instance running hundreds of clinical trials
 - Decoupled the custom-function operating environment from the transactional DB/web services to have zero impact on transactional workloads
 - Decomposed functions such as "core clinical objects" to leverage platform microservices for managing common clinical-trial entities shared across a suite of clinical-trial data-management systems

All of these efforts required tenacity and client hand-holding to not only achieve the technical transformation but also bring the organization—and our clients—along during the evolution of a legacy MIST solution.