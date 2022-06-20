### Title

Cultural and technological exchange between the Wikimedia and open-source ecosystems

### Short description

The Wikimedia ecosystem, including Wikipedia and Wikidata, has a range of workflows for presenting general reference information on any topic. There has never been a systematic attempt to review or improve how Wikimedia presents or shares information pertaining to the field of OSS. We propose model activities to showcase OSS culture and tools at their best in the Wikimedia ecosystem.

### Author(s)

[Daniel Mietchen](https://github.com/Daniel-Mietchen), for the Wikimedia community

### Proposal body

Below is a list of various project models which are common in the Wikimedia ecosystem, each focusing on some aspects of the OSS ecosystem. Since this phase of the proposal process includes public discussion, we presents various ideas, and ask what others feel should be priorities. If this proposal is selected, then our team can address one or more of these in a year. All of these ideas scale - they can be done massively for completeness or only in part, so as to prototype and demonstrate the process as applied to OSS.


1. Survey and description of [*Wikipedia's* articles on open source software](https://en.wikipedia.org/wiki/Category:Free_software)
    1. deliverables
        1. list the articles
        1. report their user traffic
        1. do so for all languages in which they exist
    1. scope
        1. individual software products themselves
        1. related fundamental concepts, such as algorithms, file types, operating systems
1. Survey of [*Wikidata's* content holdings on open source software](https://w.wiki/59vA
)
    1. deliverables
        1. exported dataset published for off-wiki examination
        1. present Wikidata data model
        1. list example queries for subsetting the data
        1. demonstrate Wikidata content curation workflows
        1. profile sample use cases
    1. scope
        1. software itself
        1. academic papers on software
        1. people in software
        1. topics around software
1. Mapping of dependencies of MediaWiki as structured data
    1. deliverable
        1. data profile ([current draft](https://scholia.toolforge.org/software/Q83#software-dependencies)) of a major software platform
        1. model case using something maximally open and community oriented
        1. Wikimedia community engagement in a model that is relevant to this community
        1. Documentation of the method and social impact of having dependency maps
    1. scope
        1. MediaWiki is the software which runs Wikipedia
        1. estimated software dependencies: 10,000+
        1. some of this we can automate
        1. a lot of this needs to be manually curated
1. Suggested guidelines for presenting [Jupyter notebooks in Wikipedia articles](https://doi.org/10.5281/zenodo.4031806)
    1. deliverable
        1. ~5 Wikipedia articles in ~3 languages will link to a Jupyter notebook complementing the content in the article
        1. we draft user guidelines for using Jupyter notebooks in Wikipedia
        1. we organize community conversation about the relationship between Jupyter and Wikipedia, with this relationship being a model for inclusion of other new media files in Wikipedia
    1. scope
        1. test case
        1. community discussion
        1. documentation
        1. multilingual / multicultural / diverse outreach
    1. need in Wikipedia:
        1. demonstrations, for example in the [Wikipedia article for "bubble sort"](https://en.wikipedia.org/w/index.php?title=Bubble_sort&oldid=1086722594#Use) (more examples [here](https://commons.wikimedia.org/wiki/File:Animation_of_media_files_in_the_Wikimedia_Commons_category_for_animations_of_sort_algorithms,_as_of_18_September_2020.gif))
1. Curation of example Jupyter notebooks
    1. identify famous Jupyter notebooks to share in Wikimedia projects, e.g. the one [used](https://github.com/minrk/ligo-binder) for visualizing and sonifying the initial detection of gravitational waves by LIGO
    1. examples
        1. bottleneck algorithm
        1. black hole
    1. create a certain number of Jupyter notebooks upon requests from Wikipedia editors
1. outreach packet to academics: how to register software in Wikidata
    1. deliverable
        1. instructions for academics to use Wikidata to register software
        1. instructions on how to use Wikidata for credit, acknowledgement, promotion
        1. [10 simple rules for editing Wikidata](https://github.com/Daniel-Mietchen/ideas/issues/129)
    1. scope
        1. present FAIR data to researchers
        1. present Wikidata as a place for creating, distribution, and archiving of FAIR data
1. structured data model for software
    1. deliverable
        1. community reviewed Wikidata data model for software
        1. automated entity schema for software in Wikidata, developed from [existing draft](https://www.wikidata.org/wiki/EntitySchema:E16)
    1. scope
        1. report of Wikidata software statistics
            1. how many software items
            1. what data properties they have
        1. comparison of Wikidata's model with other existing models
        1. community review of the models
        1. (optional?) expert review of the models
1. file formats of software
    1. not consistently covered in Wikidata
    1. we lack a link between data, software, instruments, and file formats
    1. consider [ImageJ](https://wikidp.org/Q1659584/preview?qid=Q1659584)
        1. accepts many file formats as input
        1. only outputs open formats
        1. many devices produce all sorts of file formats
        1. ImageJ has dedicated importers
1. Wikipedia article editing for [key concepts in open source software](https://en.wikipedia.org/wiki/Template:FOSS)
    1. deliverable
        1. conventional English Wikipedia development of 1-3 Wikipedia articles
        1. articles will be highly popular, highly linked, and fundamental to understanding OSS
        1. push through Wikipedia's article review and grading process
    1. scope
        1. follow [development model of Wiki Education Foundation](https://outreachdashboard.wmflabs.org/training)
        1. literature review
        1. English Wikipedia writing
        1. negotiating peer review from uninvolved editors
1. [language translation](https://en.wikipedia.org/wiki/Special:ContentTranslationStats) of key concepts in software, for *Wikipedia*
    1. deliverable
        1. language translation of English Wikipedia article into 3 underserved languages
    1. scope
        1. ideally find excellent English Wikipedia article which is already reviewed, and translate it to other Wikipedia language version, or vice versa
        1. in addition to approval of hired translator who does the work, seek and receive review from the language community
        1. probably collaborate with Wikimedia Language Diversity Hub or Wikitongues
1. Wiki99 for open source software
    1. ["Wiki99" is a Wikipedia outreach model](https://meta.wikimedia.org/wiki/Wiki99) for presenting ~99 Wikipedia articles as important for covering a field
    1. 99 is a number of concepts for which the Wikipedia community can reasonably aspire to review, edit, discuss, and translate
    1. deliverable
        1. a Wiki99 instance for open source source software
        1. community outreach events with feedback discussing the selection
        1. published report using Wikipedia evaluation tools on a snapshot of these articles, grading length, quality, existing translations, and community engagement
    1. scope
        1. on-wiki project page
        1. structured data list of 99 concepts usable in Wikipedia evaluation tools
        1. record of community discussion critiquing this list
        1. academic case study publication presenting the current status
1. language translation  ([demo](https://w.wiki/57uc)) of key concepts in software, for *Wikidata*
    1. deliverable
        1. list of important concepts in software
        1. present as structured data in Wikidata
        1. all terms in English plus 3 underserved languages
    1. scope
        1. research essential terms
        1. get approval and confirmation that terms are rightly selected
        1. in addition to approval of hired translator who does the work, seek and receive review from the language community
        1. probably collaborate with [Wikimedia Language Diversity Hub](https://meta.wikimedia.org/wiki/Wikimedia_Language_Diversity_Hub) or [Wikitongues](https://meta.wikimedia.org/wiki/Wikitongues), which are existing community organizations supporting projects like this one proposed
1. research article on place of Wikimedia sites in the software media ecosystem ([demo](https://doi.org/10.3897/rio.7.e68121) for healthcare)
    1. deliverable
        1. research article presenting findings from this project
        1. publish in peer reviewed academic journal
        1. write it anticipating that policy makers, business executives, journalists, and academics need information to be able to form opinions on how to react to Wikipedia
    1. scope
        1. depends on what else we do in this project
        1. probably must include these things
            1. traffic to relevant articles
            1. measurement of quality
            1. description of audience
        1. likely should include these things
            1. options for engagement
            1. case studies


### Due diligence


1. **What's your theory of change -- what impact do you expect this project to have? What's its goal?**

The Wikimedia Foundation claims a billion unique annual users. Beyond that audience, Wikimedia is openly licensed content and Linked Open Data, and propagates around the Internet through reuse by its many content consumers. Our theory of change is that by integrating software-related text and datasets into the Wikimedia platform they will become accessible to this existing userbase who already are requesting content. The result will be hundreds of millions of user requests and views for the content we integrate into Wikimedia.


2. **What related work has already been done in this area?**

There are more than 3000 academic papers &mdash; plus 20 years of journalism &mdash; on Wikipedia alone. Some relevant facts about Wikipedia are that it is popular, global, community managed and the nucleus of an ecosystem of open knowledge platforms and openly colloborating communities that use open-source software, open data, open-access publications and other resources to make knowledge accessible to as many people as possible.

For this project, the most relevant prior work on this ecosystem is that which shows that when contributors submit content there, then reusers benefit from it. The majority of research about reuse and benefit is for Wikipedia articles to benefit typical readers. Although less discussed by journalists and researchers, there is external recognition &mdash; e.g. by search engines or cultural heritage institutions &mdash; that content in Wikidata has public impact, and internally within the Wikimedia community, support for Wikidata is immense.

Our team makes this proposal as experienced Wikimedia contributors who already understand community norms, usual workflows, and the typical sorts of projects in which Wikimedia contributors engage. Our proposal is a list of those typical projects applied to OSS; while Wikimedia projects and workflows are frequently not documented or even considered as methodologies, what we propose are conventional projects inside the community.

3. **How is this proposal innovative -- what distinguishes it from other related work?**

This project matches the strengths of the Wikimedia platform to the OSS sector, and brings resources of the OSS sector into the Wikimedia platform. Although Wikipedia was established in 2001, and despite deep ideological values alignment in the Open Movement, the software sector has few partnership precedents with Wikimedia. There should be more cultural exchange between OSS and Wikimedia, and this proposal is innovative for presenting actionable ways to collaborate along these lines.


4. **Who is your doer -- who will execute the proposed work?**

All the activities proposed here would be community projects conducted in the open way typical for Wikimedia activities, with everyone being invited to contribute. They will be coordinated by [Daniel Mietchen](https://en.wikipedia.org/wiki/User:Daniel_Mietchen), a [data scientist](https://en.wikipedia.org/wiki/Data_scientist) working on opening up the ways in which research is being done, scrutinized and integrated into our collective knowledge and practice. His activities at Wikimedia concentrate on science, medicine, disaster management and sustainable development, on cooperation across languages, projects and Wikimedia community organizations as well as on outreach to scientific communities. He served on the [European Commission expert group on FAIR data](https://doi.org/10.2777/54599) and is part of the team that develops [Scholia](https://iw.toolforge.org/scholia), an open-source tool that is based on Wikidata and allows to profile and browse networks spanning between the scholarly literature, researchers ([demo](https://scholia.toolforge.org/author/Q20895785)), research institutions and other elements of the research landscape, including research software. 


6. **How might this work be sustained long-term after an initial seed grant?**

Wikimedia's community of editors will maintain this content after the seed grant. Content in the Wikimedia platform is longer lasting than many other digital publications because it is presented for updating as needed, and actively curated by a sizeable community. Beyond that, any institution which wishes to make content contributions to the Wikimedia platform can follow our precedent for doing more or for otherwise building on these projects, either directly or by sponsoring anyone else to contribute further. 

Usually, the most difficult part of organizing good content in the Wikimedia platform is arranging for it to have a good start. When Wikipedia and Wikidata have poor coverage of a popular topic, the usual reasons include that volunteers have been unable to identify suitable information sources to ingest into the Wikimedia platform, and that they lack starting documentation for describing this difficulty to off-wiki experts who would contribute sources if they were asked in a way that fits with their workflows. For strategic development beyond the labor capacity of volunteers, sponsored Wikimedia contributors can develop Wikimedia content on topics of general interest which improves the development environment for everyone. This project will lower the barriers of engagement with the open-source software ecosystem for anyone contributing to Wikimedia projects in the future.


### Resources needed

The above presents a list of pilot proposals. We cannot do all of them and would like feedback on which ones we should prioritize to best match with goals of the foundation.

A reasonable scale for any of the projects sketched out here would be about $50,000 per year, all of which will go to personnel who will invoice their labor hours against this while contributing in accordance with Wikimedia's policies on paid editing. As stated above, the projects can all be rescaled in both directions, e.g. scaled down for prototyping or scaled up for increased impact.


### Other links and resources

There is a body of literature about Wikipedia's place in society, media, and openness &mdash; see [here](https://scholia.toolforge.org/topic/Q52) for a quick overview. We invite readers of these lines to ask us anything about Wikipedia and its position in the Open Movement or to peruse the following recent publications that provide some good starting points to explore interactions between the ecosystems around Wikimedia and the wider Open Movement: 
 * [WikiProject Clinical Trials for Wikidata](http://dx.doi.org/10.1101/2022.04.01.22273328)
 * [Developing a scalable framework for partnerships between health agencies and the Wikimedia ecosystem](https://doi.org/10.3897%2FRIO.7.E68121)
 * [Representing COVID-19 information in collaborative knowledge graphs: The case of Wikidata](https://doi.org/10.3233%2FSW-210444)
 * [The LOTUS Initiative for Open Natural Products Research: Knowledge Management through Wikidata](https://doi.org/10.1101%2F2021.02.28.433265)
 * [Wikidata as a knowledge graph for the life sciences](https://doi.org/10.7554%2FELIFE.52614)

Free and open-source software is an integral part of what these papers describe but has so far not been the main focus.
Depending on anyone's interest, we can suggest further resources, including in other languages.

