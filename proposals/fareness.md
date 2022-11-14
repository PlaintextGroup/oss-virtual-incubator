### Title

Fareness

### Short description

Enforced ecosystem funding via licensing.

### Author(s)

@balupton

### Proposal body

The current licensing options for the typical developer have been unsatisfactory:

* If a permissive license is used (MIT), this excludes the commons from derivative works, and drives the commons to reimplement derivative works.

* If a copyleft aka reciprocal license is used (AGPL/GPL/RPL), this excludes commerce from original works, and drives commerce to reimplement original works.

* If an all-rights-reserved license is used, then commons is excluded from original works, and drives both the commons and commerce to reimplement original works.

The current funding options for the typical developer have been unsatisfactory:

* If the developer is not funded to work on their own open-source work, then the commons shrinks while commercial derivative works expand, excluding the commons from derivative works, and drives the commons to reimplement derivative works.

* If the developer is funded to work on their own open-source work, then they are incredibly lucky; either an open-source celebrity or a top 100 project.

What is sought is licensing which supports the commons and commerce, and funding which supports packages over projects and celebrities. This is Fareness.

Fareness supports the commons and commerce through licensing:

* Packages have their **public distribution** use the [Reciprocal Public License](https://en.wikipedia.org/wiki/Reciprocal_Public_License) which requires source-sharing of the consuming project. The RPL is analogous to the (A)GPL, however the (A)GPL does not require source-sharing of internal projects, whereas the RPL requires source-sharing of any consuming project. This is a like-for-like reciprocation, the commons sustaining itself. [RPL-1.5](https://spdx.org/licenses/RPL-1.5.html) is an OSI approved license.

* Packages have their **premium distribution** use the [Artistic License](https://en.wikipedia.org/wiki/Artistic_License) which enables use in any project, but requires modifications of the package to be rebranded and source-shared. *This distribution checks for a license. Licenses are provided by funding your open-source dependencies.* This is a tit-for-tat reciprocation, the commons and commerce sustaining each other. [Artistic-2.0](https://spdx.org/licenses/Artistic-2.0.html) is an OSI and FSF approved license.

* Supported package systems are:

  * Node.js via NPM

  * Node.js via Yarn

  * If you are a stakeholder in other package managers, get in touch  package@fareness.dev 

Fareness supports the commons and commerce through funding:

* Ecosystems and packages are funded, not just celebrities and top projects:

  * This lets commerce support their entire dependency tree, or an ecosystem, to prevent [tragedies](https://github.com/PayDevs/awful-oss-incidents) affecting critical but unknown nested dependencies.

  * This reduces the need for reimplementation and monopolisation of an ecosystem, as original works gather the funding necessary to avoid becoming reimplemented works.

* Supported package funding services are:

  * [ThanksDev](https://thanks.dev) - integration underway

  * [StackAid](https://www.stackaid.us/invite?code=XPjRcdJeDz) - integration underway

  * [PayDevs](https://paydevs.com) - integration pending

  * If you are a stakeholder in another package funding service, get in touch service@fareness.dev 

Fareness is under active development, alpha version to be completed by end of November, beta testing throughout December, and launch in January.


### Due diligence

#### What's your theory of change -- what impact do you expect this project to have? What's its goal?

The terms of open-source funding so far have been dominated by the culture of industry, focusing on a few controlled relationships with celebrity projects, developers, and companies. The long-tail of the Pareto distribution is neglected by this, leading to tragedies of package abandonment, reimplementation, paywalling, breakage, and attacks. Solving this requires funding to move from the unscalable "one subscription per celebrity" to "one subscription for an entire ecosystem". Developers incentivise this change by opting-out of non-reciprocated relationships with commerce, and requiring reimbursement of either source or funds. Fareness is a combination of decisions to scale this to every developer, to benefit the commons and commerce.

#### What related work has already been done in this area?

Unable to scale beyond celebrities to the long-tail:

- Gittip/Gratipay (defunct), Liberapay (active): optional funding of individual teams
- GitHub Sponsors (active) / Patreon (active): optional funding of individual teams/projects/developers
- OpenCollective (active): optional funding of individual projects
- Business Licensing (active): required funding of individual projects; the more adoption within an ecosystem, the more it costs and uncertainty to the ecosystem
- Developer Protests (occasional): developers delete or break packages due to commercial use without reciprocity; causes industry to double down on celebrity-enterprise relationships and monopolisation
- TideLift Lifters (active): top packages receive funding and tasks to further enterprise relationships
- GitHub Accelerator (upcoming): top projects receive funding and training to further enterprise relationships

Can scale to the long-tail, but optional enforcement limits growth:

- Flossbank (defunct): optional subscription to the Node.js ecosystem, required a cryptocurrency technology for funds distribution, at launch required advert supported tooling to replace well-known tooling: stigma around these caveats hampered adoption
- ThanksDev (active): optional subscription to the Node.js and other ecosystems
- StackAid (active): optional subscription to the Node.js ecosystem

#### How is this proposal innovative -- what distinguishes it from other related work?

**Fareness does not break existing work;**
existing package versions continue to operate; licenses continue to work on package versions published prior to license expiry.

**Fareness enables easy compliance;**
open-source projects operate as normal, closed-source projects can reach compliance for $1/month for all collaborators, or $100/month for an entire organisation.

**Fareness funds the ecosystem to scale with the ecosystem;**
increased adoption increases reciprocation and revenue, while not increasing costs and uncertainty.

#### Who is your doer -- who will execute the proposed work?

@balupton — author of hundreds of npm packages that get over 500 million installs a month — projects used in millions of public github repositories

- https://github.com/sponsors/balupton 
- https://github.com/bevry/domain-browser/network/dependents example repo usage

#### How might this work be sustained long-term after an initial seed grant?

Post-launch funding will be pinned to its success and adoption; the license-checker is a dependency, so its ongoing maintenance will be funded proportional to its adoption within the ecosystem. Grants may be received to expand Fareness to post-launch ecosystems, and to ease enterprise adoption.

### Resources needed

Funding will ease the two-months of full-time development by @balupton required to get Fareness launched.

Networking and partnerships will ease development and preemptively reduce hurdles at launch.

### Other links and resources

- https://fareness.dev
- contact@fareness.dev
- https://balupton.com/meet
