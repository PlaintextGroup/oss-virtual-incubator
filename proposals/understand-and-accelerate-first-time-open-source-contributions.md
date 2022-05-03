<!--

Please note that by submitting a PR with a new proposal, you agree to release this proposal text under the Creative Commons Zero v1.0 Universal license. See https://github.com/PlaintextGroup/oss-virtual-incubator/blob/main/LICENSE.

If you'd like to submit a proposal yourself, you have two options:

1. Fork this repo and make a copy of [PROPOSAL-TEMPLATE.md](PROPOSAL-TEMPLATE.md). Write up your proposal in the `proposals` directory, then [make a pull request](https://github.com/PlaintextGroup/oss-virtual-incubator/pulls) to this repository.
2. If you'd rather just use a form, [fill out this form][form]. Unless you tell us otherwise, we will copy over your proposal to this GitHub repository.

-->

### Title

Increase Open Source Participation by Better Understanding Effective Issues and Highlighting Them

### Short description

We seek to better understand what makes a successful “good-first-issue” so that we can bring more people into open source and help train maintainers on how to write these issues.

### Author(s)

logankilpatrick

### Proposal body

Open Source provides an incredible opportunity to make meaningful contributions to real world projects. The entry point for many into open source is looking at “help-wanted” or “good-first-issues”. The problem is, despite these titles, the issues are often not well written nor do they give enough context for a first time contributor to be able to fix the issue. This leads to a high bounce rate for those who wanted to contribute to open source but get overwhelmed or quit because of the lack of context. We propose addressing this in 3 parts:

1. Work with the Open Source community to craft guidelines on how to write a good “help-wanted” and “good-first-issue” issue. 
2. Build a training program to support maintainers with this work.
3. Implement a machine learning tool to help new users discover places to contribute to.

For part 1, lots of literature already exists on this, but most maintainers do not follow it. The goal for part one is to create a definitive resource and then make sure it gets placed in high quality places like GitHub and freeCodeCamp for visibility. In part two, we will train maintainers of open source projects why they should make “good-first-issue” issues and how to create them effectively. Given my background with NumFOCUS, we will likely start with those projects since the connections are already there and then branch out to more projects. Lastly, it is worth investigating whether a machine learning tool trained on good first issues would be valuable for the community. The biggest issue here would be getting the labeled dataset. We would collect “good-first-issue” labeled issues and then have them put in front of experts and new contributors to decide if thy are good. After that, we can train a simple sentiment analysis NLP model to understand if the issue meets our bar or not. If it does, we could make a basic web interface to search theses issues. We would also use this to “advertise” to maintainers that they should write these issues such that they can be on the site.


### Due diligence

<!-- Please answer the following due diligence questions; it's okay to answer "N/A" if you don't know yet. -->

1. **What related work has already been done in this area?**
- There is lots of writing about how to create a good first issue but no active training I have seen.

2. **How is this proposal innovative -- what distinguishes it from other related work?**
- The biggest piece of innovation here is applying ML to the problem. Most platforms / websites just show you all the potential issues regardless of quality. It would be very impactful to have somewhere where anyone can go and find an issue.

3. **Who is your doer -- who will execute the proposed work?**
  - The doer for this project is me, with potentially some help from other open source maintainers depending on the grant amount.
 
5. **How might this work be sustained long-term after an initial seed grant?** 
- Housing this work under NumFOCUS as a program will likely lead to the longest term sustainability.

### Resources needed

I have both the experience in Open Source and ML to make this project a reality. With that said, most of my ML experience is not in NLP so having a mentor / advisor that knows that space well could be helpful. I also think getting GitHub and GitLab involved in this project as early as possible will be helpful since they could provide resources to support it.

### Other links and resources

<!-- Add any other links, images, or resources that are relevant to the proposal -->
