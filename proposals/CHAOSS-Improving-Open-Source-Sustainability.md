### Title

CHAOSS: Improving Open Source Sustainability 

### Short description

CHAOSS is an open source project focused on creating practices to help define community health. Work in the CHAOSS Project community is organized around software, metrics, and projects aimed at helping improve how we all understand the health and sustainability of open source projects.

Our project goals are to advance work in the CHAOSS project in directions which our long standing membership and newcomers view as areas of increasing importance for understanding the health and sustainability of open source software. Specifically, we propose three interconnected thrusts: (1) advancing ecosystem level understanding of open source software health, and distinguishing characteristics across ecosystems of: a) software distributed by different package managers (Python, Rust, and NPM), b) corporatized open source infrastructure, and c) scientific open source software. We will use machine learning analysis, and dependency analysis embedded within the CHAOSS/Augur software project, (2) advancing CHAOSS diversity, equity, and inclusion (DEI) metrics and programs to help open source projects best center DEI in their own efforts, and (3) building collections of CHAOSS metrics (i.e., metrics models) and providing the technical mechanisms necessary for these metrics models to be readily deployable using CHAOSS software.


### Author(s)

- Sean Goggins, University of Missouri
- Elizabeth Barron, CHAOSS 
- Matt Germonprez, University of Nebraska at Omaha


### Proposal body

In little more than 20 years, open source has come to represent a collection of activities and innovations defined by an ever-changing and dynamic landscape of engagement. In the complex setting of open source projects, research and applied efforts are shedding light on people, conventions, resources, distribution systems, and aesthetics that define the rapidly shifting state of open source projects in today’s modern organizational settings. In many cases, organizations assume a future for a set of projects, but cannot see within or across these complex systems to assess internal project health, and the corresponding level of risk to their infrastructure. Improving the transparency and actionability around open source project health -- the potential that an open source project will continue developing quality software – is therefore an important issue for all.

Rapid growth in open source software, combined with limited understanding of how the larger ecosystem is interdependent, makes the absence of transparency a risk for businesses and scientific organizations alike. Open source projects sometimes go dormant, leaving a technological dust bowl in their wake for dependent projects and organizations. To address these risks to health and sustainability, which are a latent and significant problem for a wide range of critical technical infrastructure, we extend our work found in the CHAOSS project to grow common metrics, software, and practices. 

CHAOSS is an open source project focused on creating metrics, software, and practices to help improve community health and sustainability. As the importance of open source software is no longer in question, its central role in technology work raises vital questions about how we understand the health and sustainability of the open-source projects we rely on. Unhealthy projects can have negative impacts on the community involved in the project as well as organizations that rely on such projects. In response, people want to know more about the open-source projects they are engaged with. For example:

Open source contributors want to know where they should place their efforts and know that they are making an impact.

Open source communities want to attract new members, ensure consistent quality, and reward valuable members.

Open source companies want to know which communities to engage with, communicate the impact the organization has on the community, and evaluate the work of their employees within open source.

Open source foundations want to identify and respond to community needs, evaluate the impact of their work, and promote communities.

In response, CHAOSS was founded as a project at the Linux Foundation in 2017. Over these five years, CHAOSS has improved how all understand open source project health and sustainability in key ways, helping relevant stakeholders make more informed decisions about open source project engagement and community development. More information on CHAOSS is available at: https://chaoss.community. 

With respect to the current proposal, we aim to advance three key projects with CHAOSS: (1) developing CHAOSS software to map open source software ecosystems and identify areas of critical concern within a specified ecosystem, (2) advancing CHAOSS diversity, equity, and inclusion (DEI) metrics and programs to help open source projects best center DEI in their own efforts, and (3) building collections of CHAOSS metrics (i.e., metrics models) and making these collections deployable through CHAOSS software.

Each of the three projects leverages the CHAOSS Project's established community and technology in specific ways intended to catalyze adjacent corporate, university, and non-government organization open source software initiatives. 

Outputs of the three projects include: 
1. Software (CHAOSS/Augur) advanced to build maps of open source software ecosystems  using machine learning and other techniques at a scale previously not possible.    
2. Processes and collaborations that enable open source software projects to accomplish goals of more diverse, equitable, and inclusive communities, without placing greater strain on oftentimes overloaded project maintainers. 
3. A hosted software platform **designed** to make newcomer understanding of the health and sustainability of complex, interconnected open source software projects easy to create for their own projects of interest, navigate, and explore for the first time, using CHAOSS metrics models. 

Outcomes of the three projects include: 
1. Maps of five different, substantial open source software ecosystems, including at least one each from corporatized open source software, scientific open source software, and non-government organization (NGO) open source software. We assert this outcome has the potential to fundamentally alter how open source software is understood by the general population. 
2. An active, functional DEI Project Badging program that incorporates peer review and constructive feedback to help open source software project maintainers earn and promote credit for their DEI efforts. This outcome builds on the CHAOSS DEI Event badging program's principles.
3. Increased individual, and organizational engagement in open source software projects enabled by human centered design of CHAOSS metrics models. Our design goal is to make open source software more accessible to newcomers, and to make newcomers needs, and desires more understandable for open source software project maintainers. 

**Project 1: Ecosystem Health and Sustainability.** 
In almost all areas of open source software, from package managed libraries to core corporatized infrastructure, and scientific software our ability to manage and navigate the complexity of open source ecosystems is limited. While the importance of open-source software is widely acknowledged across research communities, the creation, development, and maintenance of open-source software varies across and within distinct ecosystems. The interdependencies between software and the work undertaken and needed to sustain open-source software at an ecosystem-level are nearly invisible. In response, we will build on the work of the CHAOSS community to make the identification of the properties of open source software ecosystems more visible by mapping known software and critical interdependencies so that we can all better discuss, analyze, coordinate, and improve our software dependent work. Specifically, we will identify and target two big problems in open-source software ecosystems:

Discovery: The process of identifying related open source software components is ad-hoc, leading to an unclear picture of software present within an ecosystem.
Health Assessment: Software can be available without a healthy, active contributor community to keep it useful and synchronized with software around it. Without sustained effort software can create problems in the supply chain of nearby open-source software projects. These characteristics include identifying ecosystem-level characteristics that correspond with reliability, safety, security, inclusivity, and what might generally be described as health trajectories. 

As users coalesce around open-source software toolchains, support and skill flow also coalesce, generating valuable, and stabilizing network effects. If developers and maintainers of open-source software know who is using the software and how it is being used and combined in workflows and infrastructure, then they will be better able to support their users. In turn, this will help ensure compatibility with nearby software, and anticipate the future software needs of cutting-edge projects. 

More subtle effects are also valuable. For example, clearer understanding of dependencies and patterns of use in software make local ecosystems more able to compose software from smaller packages, each more specialized. Smaller, more specialized packages increase “option value” or the innovative potential from recombination. An increased option value can help fix problems or provide new capabilities in fewer locations, meaning fewer partial, redundant, and desynchronized changes.

The first part in this project will scale the dependency analysis and machine learning components of the CHAOSS/Augur software project. Specifically, we will engage the CHAOSS community in an iterative process of identifying critical sub-ecosystems in package managed libraries, core corporatized infrastructure, and scientific software. We will then scale CHAOSS/Augur’s existing machine learning algorithms to discover, assess, and identify ecosystem-level characteristics that generate an ecosystem map. The map will substantially accelerate the open-source community writ large’s ability to discover opportunities for improvement, and models of practice that are effective in similar ecosystems and sub-ecosystems. 

The second part in this project will identify specific metrics and metrics models necessary to identify critical health concerns within a mapped ecosystem.  Scaling the application of CHAOSS/Augur’s machine learning capabilities will reveal characteristics and similarities within and across projects within an ecosystem. Specifically, Augur takes a collection of projects defined by the user, and conducts local and global clustering analysis, topic modeling, discourse analysis (parts of speech in issues, pull requests, and associated comments), message novelty, message sentiment, probabilistic evaluation of a pull request’s likelihood of acceptance, and anomaly detection (i.e., acceleration and deceleration of distinct types of project and ecosystem activity against a normed model built from a configurable training period). 

**Project 2: Centering DEI.** A key component of CHAOSS is the development of DEI metrics to help, not only ourselves, but others best center DEI within their projects. Improving open source work and the DEI share a common geography. For open source community health, the key for aligning our efforts lies in the application of research and practice illustrating how advancing DEI within open source communities enables us to overcome key open source challenges from new perspectives. More productive teams and healthier communities will emerge through this recognition, the introduction of new points of view, and a growing understanding that open source software faces shared challenges advanced through new alignments.

We will draw our work forward in a new CHAOSS DEI Project Badging Program to help others in better centering DEI in their own communities. In particular, we will help other community members consider (1) challenges in centering DEI in globally distributed and culturally diverse communities, (2)  a focus on new and existing contributor retention as critical for better centering DEI with an open source project, and (3) that any DEI reflection is not always about end goals but can serve as inspiration for a community as a whole.

The first part of this project will identify necessary CHAOSS metrics used to help center DEI at a project level. This work will extend current CHAOSS efforts in the development of metrics and metrics models necessary for open source project maintainers and community ways to improve their experiences for all. 

The second part of this project will develop an open and transparent application and review process through which open source projects can request DEI Project Badges for accomplishing specific, measurable goals that demonstrate progress toward centering DEI within their own projects. This work will build from our current DEI Event Badging program that has badged over 40 open source events in their efforts to best center DEI within their events. In doing so, the CHAOSS project can serve to help open source projects consider DEI as an important part of building and sustaining healthy open source projects. 

**Project 3: Metrics Models.** To date, CHAOSS has developed over 70 health and sustainability metrics in the areas of project risk, evolution, value, and DEI. The metrics provide standard definitions around health and sustainability concerns such as issue age, contributor volume, and license coverage. Yet, we have found that each metric in isolation is limited in its ability to build knowledge of health and sustainability. In response, CHAOSS members have begun to assemble collections of metrics, or metrics models, to provide more meaning to any individual metric. Such models include project responsiveness, contributor retention, and DEI within a project. 

Our exploration of metrics models are implemented using Jupyter Notebooks. We have the technical mechanics for building metrics models through a robust pilot phase. To advance metrics models to meet demand, we need to provide a well designed user interface that pairs the models with CHAOSS software and CHAOSS programs to enable their easy deployment for people and organizations. By pairing metrics models with CHAOSS software and programs, we improve accessibility to critical health and sustainability knowledge that enables open source program offices, technology companies, project maintainers, and other stakeholders to quickly apply metrics models to answer new questions as they evolve in a project’s context.  

The first part of this project includes the development and distribution of metrics models that help people, communities, and organizations best consider how their available data can be drawn together in meaningful and actionable ways to improve the health of open source communities of interest. Metrics models can include such concerns as project responsiveness, project engagement, member burnout, and community welcomingness.

The second part of this project includes the deployment of metrics models for people, communities, and organizations looking to immediately understand how metrics models apply to their communities of interest. This will include integration with the CHAOSS Augur software in making metrics models live through web and mobile interfaces -- making open source community health questions and answers more immediately available than they currently are. 


### Due diligence

<!-- Please answer the following due diligence questions; it's okay to answer "N/A" if you don't know yet. -->

1. **What related work has already been done in this area?** All the proposed project work exists in pieces with the CHAOSS project. 

In the case of ecosystem health and sustainability, CHAOSS/Augur has already developed and tuned the dependency analysis and machine learning algorithms and run them on repository collections up to 3,500. 

In the case of centering DEI, numerous CHAOSS DEI metrics have been released around event diversity, leadership & governance, and project & community. Further, the CHAOSS DEI Event Badging Program has issued over 50 badges to events working to improve their own DEI efforts. Yet, work needs to be done to advance our CHAOSS DEI project-level efforts. 

In the case of metrics models, no metrics models have been released nor have they been tied to existing software or programs. Yet, there exist over 70 CHAOSS metrics from which to build metrics models. The success of our metrics and software work are driving demand for metrics models. 

2. **How is this proposal innovative -- what distinguishes it from other related work?** The proposal builds from the solid base that the CHAOSS project provides. It is distinguished from other related work as the CHAOSS project is the leading open source project focused precisely on open source community health and sustainability. Our position with the open source landscape sets us apart as a community with members from industry, academia, and funding agencies all focused on improving the health and sustainability of open source communities. 

The particular projects are innovative as they advance prior efforts within the CHAOSS project and start to place them in front of people who want easy and quick views of open source community health and sustainability, as informed by years of community research. The projects will move the CHAOSS work from articulated documents to activities in practice available for all. We’ve built the base, now we are putting the base into practice for broad audiences. 

As a whole, each project in this proposal contributes to the scaling of CHAOSS standards and software so they can answer larger questions, contribute to the development of ecosystem level maps, and be more easily applied by a larger community of open source stakeholders. 

3. **Who is your doer -- who will execute the proposed work?** The doers include the authors of this proposal as well as CHAOSS community members engaged in different projects described here. Further, funds would be used to support two graduate students and one graphic design consultant. 

4. **How might this work be sustained long-term after an initial seed grant?** Members of the proposing team have been long-term contributors to open source community health and sustainability efforts. Our work has been funded by the Alfred P. Sloan Foundation, the Ford Foundation, the Chan Zuckerberg Initiative, Mozilla, the National Science Foundation, and several for-profit organizations. We are experienced in partnering with external funding organizations - understanding the goals of funding for all the parties involved. Our efforts not only include the aforementioned projects in this proposal but the ongoing securing of external financial support to ensure the longevity of the CHAOSS project. 

### Resources needed

Amount requested (please specify payment breakdown by year and quarter, and by recipient if
there are multiple): $400,000 ($320,000 on start, $120,000 in Q3 FY22)

Project Team Leads: $90,000
Graphic Designer: $80,000
Software Community Manager: $80,000
Graduate Student: $65,000
Hardware for Metrics Models Deployment: $15,000 
Hardware for Ecosystem Machine Learning Analysis $40,000
Travel: $30,000
Overhead costs (10%): $40,000

Total:  $440,000

#### Timeline
During year 1 we will hire a software community manager to coordinate the advancement of projects 1 and 3. We will also hire a graphic designer to advance all three projects.  Our proposed budget covers this first year, during which we plan to complete initial deployments of each project. We will effectively deliver the core technology, design, and community assets by the end of year one. This will include the purchase of computing hardware in the first half of year 1. Year 1 is aimed at building the outputs that catalyze the outcomes for each project. 

During year two the team leads, graduate student, and CHAOSS community will continue to advance the technology, processes, and community to catalyze sustainable advancement of our goals through the efforts of current partners including GitHub, Red Hat Software, VMWare, and other, new partnerships developed during year one.  


### Other links and resources

CHAOSS Project: https://chaoss.community/
Augur Project: https://www.augurlabs.io/
CHAOSS DEI Event Badging: https://github.com/badging/event-diversity-and-inclusion 
