
### Title

<!-- A short, pithy title for the proposal. -->
Calls to Action for Better Patch Adoption

### Short description

If patches are available for upstream vulnerabilities, why don't more projects upgrade? What are the simplest systemic improvements that could make a difference at scale?

### Author(s)

<!-- Put your GitHub username(s) here. The proposal author(s) will "own" the proposal and will be able to accept future PRs that change it. -->
[GitHub: lucasgonze](https://github.com/lucasgonze/)

### Proposal body

<!-- Explain your proposal. Add as much as you want, within reason! -->
Critical vulnerabilities often linger in deployed software long past the point when a patch is available. Maven estimates that [35% of Log4J downloads continue to pull the version with the world-famous vulnerability](https://www.sonatype.com/resources/log4j-vulnerability-resource-center?smtNoRedir=1). Why?

More importantly, what are the most promising remediations? 

Let's fix that. Let's go find out. I propose research into the reasons why patches aren't being applied.

#### Go-To-Market and Roadmap

0. Gather a list of potential remediations
 - Survey prior research
 - Brainstorm
 - Document steps to apply each remediation

1. Gain access to repositories

  - Identify impactful repos
    - Avoid toy projects, unreleased code, projects with low adoption
    - Find some commercial code bases that use open source libraries
  - Gain access to repos
    - For proprietary code bases, may need to cultivate relationships in order to have access. OSPOs may be able to help.
    - Focus on open source projects, because we have easy access to the code
  - Span source-code hosting tools
    - GitHub
    - GitLab
    - Independent

2. Identify open vulnerabilities

  - Gather a manifest
  - Compare manifest to CVE catalog

3. Categorize causes of vulnerabilities

  - Not using Dependabot at all
  - Not applying auto-upgrades
  - Auto-upgrades blocked on breaking changes in upgrade path
  - Inadequate infrastructure (tooling, test coverage, QA) to perform auto-upgrades
  - Upgrades applied in dev but not released to production
  - Distrust in reliability of supposed non-breaking changes
  - Pinned version in package lock file

4. Document findings
  - Map remediations to causes and identify most promising options
  - Report to OpenSSF
  - Conference presentation

### Due diligence

<!-- Please answer the following due diligence questions; it's okay to answer "N/A" if you don't know yet. -->

1. **What's your theory of change -- what impact do you expect this project to have? What's its goal?** 

This project will enable future work by myself and others to improve adoption of patches. This project will be a partial success if it correctly identifies the most important causes. It will be a complete success if it finds causes that can be addressed with a high probability of success.

2. **What related work has already been done in this area?** <!-- Insert answer here --> 

Package management, dependency chains, open source, and security are a relatively new topic. There is little closely related research, but it is gathering momentum. The proposed project will build on and add to the available body of knowledge.

- In Dependencies We Trust: How vulnerable are dependencies in software modules? (2015)

https://repository.tudelft.nl/islandora/object/uuid:3a15293b-16f6-4e9d-b6a2-f02cd52f1a9e

> We studied the npm registry, a popular centralized repository for hosting JavaScript modules by using information from security advisories in order to determine: prevalence of modules depending on vulnerable dependencies, the propagation in the dependency chain and the time window to resolve a vulnerable dependency. This was followed by a qualitative study to understand dependency management practices in order to investigate why dependencies remain unchanged. The outcome of this study shows that one-third of the modules using at least one advisory dependency resolve to a vulnerable version. The qualitative study suggested that a majority of the modules lacked awareness or discussion about known vulnerabilities. Furthermore, the key findings indicate that the context use of the module and breaking changes are potential reasons for not resolving the vulnerable dependency.

- Vulnerable open source dependencies: counting those that matter (2018)

https://dl.acm.org/doi/abs/10.1145/3239235.3268920

> We found that about 20% of the dependencies affected by a known vulnerability are not deployed, and therefore, they do not represent a danger to the analyzed library because they cannot be exploited in practice. Developers of the analyzed libraries are able to fix (and actually responsible for) 82% of the deployed vulnerable dependencies. The vast majority (81%) of vulnerable dependencies may be fixed by simply updating to a new version, while 1% of the vulnerable dependencies in our sample are halted, and therefore, potentially require a costly mitigation strategy.

- Beyond Metadata: Code-Centric and Usage-Based Analysis of Known Vulnerabilities in Open-Source Software 

https://ieeexplore.ieee.org/abstract/document/8530051 (2018)

> In the early phases of development, updating a library to a more recent release is relatively unproblematic, because the necessary adaptations in the application code can be performed as part of the normal development activities. On the other hand, as soon as a project gets closer to the date of release to customers, and during the entire operational lifetime, all updates need to be carefully pondered, because they can impact the release schedule, require additional effort, cause system downtime, or introduce new defects.
>
> To evaluate precisely the need and the urgency of a library update, it is necessary to answer the key question: “is the vulnerability exploitable, given the particular way the library is used within the application?”. Answering this question is extremely difficult: vulnerabilities are typically described in advisories that consist of short, high-level, textual descriptions in natural language, whereas a reliable assessment of the exploitability and the potential impact of a vulnerability demands much lower-level, detailed, technical information.

- On the Threat of npm Vulnerable Dependencies in Node.js Applications (2020)

https://arxiv.org/abs/2009.09019

> Our findings show that although 67.93% of the examined applications depend on at least one vulnerable package, 94.91% of the vulnerable packages in those affected applications are classified as having low threat. Moreover, we find that in the case of vulnerable packages classified as having high threat, it is the application's lack of updating that makes them vulnerable, i.e., it is not the existence of the vulnerability that is the real problem.

- Out of sight, out of mind? How vulnerable dependencies affect open-source projects (2021)

https://link.springer.com/article/10.1007/s10664-021-09959-3

> We found that project activity level, popularity, and developer experience do not translate into better or worse handling of dependency vulnerabilities. We found that most dependency vulnerabilities persist throughout the observation period (mean of 78.4%, 97.7%, and 66.4% for publicly-known vulnerabilities in our Java, Python, and Ruby datasets respectively), and the resolved ones take 3-5 months to fix.

3. **How is this proposal innovative -- what distinguishes it from other related work?** 

This proposal is innovative in that it is a precursor to direct action. Asking the question of how we can improve adoption of security-related patches for open source libraries begs for resolution in the form of work to implement the findings.

This is not academic research. It is groundwork for development.

4. **Who is your doer -- who will execute the proposed work?** <!-- Insert answer here -->
  * Lucas Gonze
    - email: [lucas@gonze.com](mailto:lucas@gonze.com)
    - CV: [gonze.com/cv.pdf](https://gonze.com/tmp/LucasGonze-CV-OSS_virtual_incubator.pdf)

5. **How might this work be sustained long-term after an initial seed grant?** <!-- Insert answer here -->
  * The work is a complete deliverable in itself. Follow-up work will be to put identified remediations into action. The follow-up work can be performed independently by the doer and others. 

### Resources needed

<!-- What resources are needed (grant money, advisors, expertise, etc.) to realize this proposal? -->
$10K grant money for one doer to spend six weeks gathering data and two weeks writing it up. 
