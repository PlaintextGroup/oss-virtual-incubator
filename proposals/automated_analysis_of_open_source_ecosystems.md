### Title

Automated analysis of open source ecosystems based on Awesome Lists

### Short description

The fully automated processing of Awesome lists allows the health of various open source ecosystems to be captured and analyzed. This gives developers, user and contributors a better understanding whether additional resources are needed and which software packages have a healthy community and development.

### Author(s)

Ly0n

### Proposal body

So-called Awesome List are a central part of the open source ecosystem. They allow developers to get an overview of open source projects in different areas. A cross-platform search engine for open source projects does not yet exist. Therefore, they represent the central dictionary for the most diverse areas within the open source ecosystem. The Awesome.re website offers a central point of contact here, as it provides an overview of all subdomains. The central task of this list is to make projects within a subject area easier to find. Thus, users can browse appropriate resources. At the same time, developers can check which projects already exist, so that resources are concentrated and the wheel is not always reinvented. 

The OpenSustain.tech website is based on such an Awesome list, and we are currently working on an open source tooling to analyze the state of the open source ecosystem in the area of climate change related open source technology.

Most of the projects are linked to GitHub or GitLab repository of the underlying project. Therefore, we are able to analyze every project via the platform API to extract meta data from the listed projects. In this way, various health indicators are extracted for every active and listed project within the ecosystem like:

* Last Activity
* Elephant Factor ( How much does the project depend on a single person)
* Number of Reviews per Pull Request
* Ratio of Closed to Open Issue
* Mean Time until an issue is closed
* ...

Here you will find the first running prototype for our study.

https://github.com/protontypes/AwesomeCure

The extracted data on the projects for our study: https://airtable.com/shr9we419r2TkpLkc

The data on the organizations with the ecosystem: https://airtable.com/shrBuNq6VkQQDzB36

I am convinced that the method of our study can be applied to other open source areas as well. Since all official Awesome lists are checked with a linter to the standard "awesome" format, we should be able to develop our tools generically so that they can be used everywhere. That is why we plan to release the tooling for our study as a seperated open source project. This should make it possible to easily repeat the study in the future and to transfer our method to other lists. 

### Due diligence

1. **What related work has already been done in this area?**  We developed a first very simple prototype: https://github.com/protontypes/AwesomeCure
2. **How is this proposal innovative -- what distinguishes it from other related work?** No one has yet developed a tool to study the health of hundreds of open source projects at the same time. 
3. **Who is your doer -- who will execute the proposed work?**  I'm leading the development of this tool. Unfortunately, I am the only experienced developer within the team at the moment. 
4. **How might this work be sustained long-term after an initial seed grant?**  I see the opportunity to use these tools to advise companies on how to use, co-develop, and invest in open source. Basic funding is possible on a donation basis. Services for companies also allow to generate revenue for the project. 

### Resources needed

I would need more experienced software developers to make the project usable for different types of awesome lists.  Also, it would be good to have a company as a customer to include their needs in the developers. Advice would also be helpful from people with sufficient experience in this area to weigh different use cases.  A grant would help me to free up enough capacity for the project to turn it into a professional open source tool in the medium term.
