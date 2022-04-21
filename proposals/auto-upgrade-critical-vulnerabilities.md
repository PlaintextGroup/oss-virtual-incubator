### Title

<!-- A short, pithy title for the proposal. -->
Auto-Upgrade Critical Vulnerabilities

### Short description

<!-- A short, one-sentence description of the proposal. -->
If package managers performed auto-upgrades for vulnerabilities when severity is high and risk is low, the Internet as a whole would recover more rapidly from critical failures such as Log4J.

### Author(s)

<!-- Put your GitHub username(s) here. The proposal author(s) will "own" the proposal and will be able to accept future PRs that change it. -->
[GitHub: lucasgonze](https://github.com/lucasgonze/)

### Proposal body

<!-- Explain your proposal. Add as much as you want, within reason! -->
Critical vulnerabilities often linger in deployed software long past the point when a patch is available. Maven estimates that [35% of Log4J downloads continue to pull the version with the world-famous vulnerability](https://www.sonatype.com/resources/log4j-vulnerability-resource-center?smtNoRedir=1). 

I propose tooling and an organization dedicated to making automatic patching of critical vulnerabilities safe and reliable enough to be adopted widely. 

#### Requirements

##### Site

There must be a website for submitting, maintaining, and fetching auto-updates. It would be a centralized site shared by all package managers, regardless of language or platform, to reduce attackable surface area and limit the cost of bringing auto-upgrades to the many package managers that need them.

Functionality, organized by user role:

- As a patch submitter, I need a user interface to create and edit an alert. I am most likely a maintainer of the affected package, but might also be an interested third party, like a security researcher or an administrator in the auto-upgrade team.
- As an administrator of the auto-upgrade project, I need to be able to maintain alerts, including the ability to:
  - Message submitters to bring an alert to a publishable state 
  - Edit metadata
  - Publish a completed alert
  - Reject an alert that does not meet stringent criteria
- As a user of a package management tool, I need to be able to:
  - Use a REST API to match the packages I use with the catalog of alerts
  - Use human-friendly documentation to learn more about recommended upgrades

Metadata for each candidate auto-upgrade:

* Package name
* Repository URL
* Versions containing the vulnerability
* First patched version (an array, to enable patches without a breaking change for different top-level versions)
* Vulnerability score (use First.org rubric calculator at https://www.first.org/cvss/calculator/3.1 and submit the resulting URL)
* ID or URL in package management catalogs (NPM, CPAN, etc...)
* CVE and CWE identifiers
* Description of the vulnerability
* Description of the patch
* Submitter contact information

##### Global Scale

Localization is relevant to the mission because excluding non-dominant locales risks allowing pockets of infected computers. 

- Servers must be accessible on a global scale, including within politically sensitive zones such as China.

- UI should be available in multiple languages, including the top five most-spoken languages (Chinese, Spanish, English, Hindi, and Arabic). 

##### Package Management Integration

CLI tools for package management would need UI additions. A developer using the package manager would be able to learn about the auto-upgrade, accept or reject a particular upgrade, and configure settings for future auto-upgrades.  There might be new CLI operations such as `--auto-upgrade`. For example, in an application using NPM affected locations might be `package.json`,  `package-lock.json`, and `node-modules`. Most importantly, existing CLI operations such as `npm install` would change to incorporate auto-upgrade. 

New documentation would be needed for users of package management tools.

#### Risks

1. Upgrades might contain breaking changes, despite developer claims. These might be design changes or bugs. Amelioration: automated updates will only begin after a gray period in which the changes are available for discretionary updates.

2. Upgrades might be attacked by insiders within the auto-upgrade system, whether motivated by personal goals or coercion. Amelioration: at least three people should approve an auto-upgrade. To prevent nation-state coercion, the approvers must span more than one country.

3. Technical vulnerabilities in upgrade infrastructure might be used to trigger malicious upgrades. Amelioration: security practices are good enough to bear the responsibility.

#### Operations

There is an organization or group administering the project. 

There is a website for submitting, maintaining, and fetching auto-updates.

- Submitters have a UI to create and edit an alert. They are most likely a maintainer of the affected package, but they might also be a security researcher or an interested third party. In some cases, an administrator might submit an alert.
- Administrators maintain alerts. They can edit metadata. They can publish or reject an alert. They can also message submitters to bring an alert to a publishable state. In a separate line of responsibility, they do development on the site.
- Fetchers are probably users of a package manager checking for alerts. They can match the packages they use with active alerts. Their main point of contact is a REST API.
- Package consumers are users of a package manager investigating an auto-update.

#### Go-To-Market and Roadmap

On the demand side, the main distribution channel for upgrades is package management tooling. To ease the bottleneck, the auto-update project will contribute as much of the package management labor as possible. It will work closely with maintainers of package management tooling such as NPM, submitting PRs for necessary code changes in CLIs and websites.

On the supply side, the bottleneck is learning about relevant patches. Maintainers of the auto-update project will develop relationships with the CVE community, raising awareness with articles and conference talks.

Roadmap:
1. Sign-off and funding
2. Website for creating and publishing auto-upgrades
3. REST API for fetching auto-upgrades
4. Implementation in the first package manager
5. First production auto-upgrade
6. Iterate through most common package managers
7. Widely available and in use

### Due diligence

<!-- Please answer the following due diligence questions; it's okay to answer "N/A" if you don't know yet. -->

1. **What's your theory of change -- what impact do you expect this project to have? What's its goal?** <!-- Insert answer here -->
  * Critical vulnerabilities will be flushed out of the open-source ecosystem much more quickly, leaving the Internet more secure. 
2. **What related work has already been done in this area?** <!-- Insert answer here --> 
  * These features allow a user of a package to break through the ordinary logic of dependency resolution and force a non-standard result:
    * Yarn [resolutions](https://github.com/yarnpkg/rfcs/blob/master/implemented/0000-selective-versions-resolutions.md)
    * NPM [overrides](https://medium.com/microsoftazure/how-to-fix-your-security-vulnerabilities-with-npm-override-c4b5be0ab4f6). 
  * Dependabot can automatically perform some updates. However, it only runs within GitHub; it does not perform a qualitative analysis of upgrade targets, and so is not trustworthy enough for high-stakes applications; and it is susceptible to legal and politicals pressures. 
3. **How is this proposal innovative -- what distinguishes it from other related work?** <!-- -->
  * The proposal makes automated upgrades feasible in important new contexts by substantially improving reliability and by working outside of GitHub.  
4. **Who is your doer -- who will execute the proposed work?** <!-- Insert answer here -->
  * Lucas Gonze
    - email: [lucas@gonze.com](mailto:lucas@gonze.com)
    - CV: [gonze.com/cv.pdf](https://gonze.com/tmp/LucasGonze-CV-OSS_virtual_incubator.pdf)
5. **How might this work be sustained long-term after an initial seed grant?** <!-- Insert answer here -->
  * Additional grants would be needed for development and maintenance.

### Resources needed

<!-- What resources are needed (grant money, advisors, expertise, etc.) to realize this proposal? -->

I'm seeking an initial grant of $10,000 to validate key assumptions:

- There has been a critical mass of important vulnerability patches that fit this model.
- Maintainers of package management tooling would embrace the feature.
- Verifying patches to the degree necessary is feasible.
- This is the simplest system design that could work. 

