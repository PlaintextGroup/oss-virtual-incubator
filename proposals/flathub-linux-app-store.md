### Title

Flathub: Linux App Store

### Short description

Promote diversity and sustainability in the Linux desktop community by adding payments, donations and subscriptions to the Flathub app store.

### Author(s)

@ramcq @neilmcgovern @aleixpol

### Proposal body

The GNOME Foundation and KDE e.V. have been jointly building and growing Flathub as a vendor-neutral service for Linux application developers to build and publish their applications directly to their end users. A healthy application ecosystem is essential for a the success of the OSS desktop, so end-users can trust and control their data and development platforms on the device in front of them.

In order to incentivise participation in the Linux application ecosystem, and remove financial barriers that prevent diverse participation, GNOME has sponsored work over the past year to add donations and payments to Flathub via Stripe, as well as a process to verify developer identities and allow direct uploads to ease the publishing process. This year we are planning to launch this work together with appropriate legal and governance setup, and are seeking additional funding to add: subscriptions / recurring donations, review tools to prevent abusive application submissions and automated security/vulnerability scanning. Over time we hope that Flathub can become self-sustaining through transaction fees and corporate sponsorship.

The GNOME Foundation is a non-profit organization that believes in a world where everyone is empowered by technology they can trust. We do this by building a diverse and sustainable free software personal computing ecosystem. We have been operating as a project since August 1997, and as a Foundation since August 2000. Together with KDE e.V., we maintain that end-user trust, transparency and control of the devices in front of them, such as desktops, laptops and workstations, is an essential pre-requisite so that we posess neutral platforms from which user-respecting internet and cloud experiences can continue to be developed.

### Due diligence

1. **What's your theory of change -- what impact do you expect this project to have? What's its goal?** 

A key barrier to the growth and adoption of open source software on the desktop is the requirement for certain applications to be available so that they are able to be fully productive using the open source desktop. The current nature of open source operating systems, especially for end users where applications are distributed at zero cost alongside the OS itself precludes establishing any incentives for application developers and prevents the distribution of paid-for applications. Intentionally or not, many stakeholders such as traditional Linux OS vendors act as gatekeepers, slowing the ability of potential application developers to publish to their users, as well as disincentivizing any application developer who is unable to learn, produce and support their application without any remuneration.

Through our organisations' participation in schemes such as Google Summer of Code and Outreachy, we have observed the impact of this effect on individuals from diverse and underpriveleged backgrounds - by electing to participate in our internship schemes, they missed opportunities for internships with other local technology employers, and struggle to find employment compared to their peers who work outside the free and open source space. By opening new pathways for individuals and small businesses to monetise their participation in the OSS desktop space, we hope to create a more level playing field for innovation and creation of sustainable economic models, as can be found on competing proprietary platforms.

We feel it is key for a broad range of applications to be available that software developers are able to receive funds for their applications, and we are building a vendor-neutral commercial and technical ecosystem to publish and distribute end-user applications for personal computing devices running Linux. Our goals are to increase the availability of applications available for Linux desktop users, and remove financial barriers for entry for diverse participants to join the developer community.

2. **What related work has already been done in this area?**

Building on top of the existing Flathub build and distribution service, which has been enjoying consistent year on year growth since 2017, over the past year the GNOME Foundation has been preparing the technical pre-requisites for Flathub to collect optional donations or mandatory payments from users on behalf of app developers. We have introduced a verification process to ensure that the uploader of the application is a bona fide representative of the developer, set up API integration with Stripe Connect to handle marketplace payments, added the necessary authentication steps for users to create accounts on the store, complete the checkout process, and issue tokens to users and developers to download and upload applications. This work is currently drawing to a close and we are ready to launch a beta service for testing/consultation with application developers.

Outside of the Linux desktop space, actors such as F-Droid provide a home for free and open source Android applications on mobile devices. However on Linux desktops and workstations, the Linux distributions have historically held near-exclusive control on the selection and delivery of applications to the users, stifling the pace of innovation (apps develop at a very different pace to the OS itself) and removing any financial incentives for developer participation.

There have been various niche efforts to bring app stores to specific Linux distributions - Lindows/Linspire pioneering the "Click'n'Run" app store some 20 years ago, and more recently Elementary OS has been experimenting with their "pay what you can" app store. These efforts, specific to one Linux OS or another, are by definition pursuing a niche of a niche as they have not been able to aggregate supply and demand between application developers or users.

Our largest "competitor" in the Linux app store space is Canonical's Snap Store, which (aside from any debates as to the relative technical merits of Flatpaks versus Snaps) sits under the control of one corporate entity rather than a community-controlled nonprofit, requiring copyright assignments for contributions to both Snap and the Store, and effectively making it very hard or unappealing to run your own stores. It consequentially enjoys far less support across community Linux-based platforms and is included by default in very few distributions apart from Canonical's own Ubuntu. Commercially vendor-neutral and under the governance of long-standing trusted nonprofits in the space, Flathub is uniquely positioned to start offering these app store services in support of the OSS application ecosystem and development community.

3. **How is this proposal innovative -- what distinguishes it from other related work?**

The Flathub platform is undergoing a number of transitions as a result of growing from a build and delivery service to an app store that allows binary uploads, and introduces fiscal incentives which may encourage abusive or misleading uploads. We are not aware of many pre-existing solutions in the open source space to this problem set, and those which do exist are not immediately applicable to the tooling around managing and publishing repositories of Flatpak applications.

We have added programmatic verification (via DNS, GitLab or GitHub credentials, etc) of application authorship based on their programmatic "app ID" identifiers, but this does not account for misleading application names, descriptions, screenshots, etc, so we need to develop tooling that detects changes in these areas and blocks submissions until these changes have been reviewed. Similarly, changes in (purported) license have an effect on how Flathub will promote and price applications, so these claims and any changes need to be checked.

As we also open the ability for applications to be uploaded in binary form, which is essential for low-friction compatibility with popular language-specific build systems such as Electron/Node, Rust, Go, etc - we also reduce the ability for users to scrutinise the source in the Flathub build system that was used to build their application. The importance of automated scanning for malware and outdated/vulnerable components therefore increases - there are tools in the cloud space which can do such automated scanning of OCI containers, and we intend to adapt these tools to apply to the desktop application space. (We can draw on pre-existing work to represent Flatpak applications as OCI container images and vice versa.)

4. **Who is your doer -- who will execute the proposed work?**

Robert McQueen was one half of the team that launched the original Flathub service in 2017, and continues to serve as part of the Flathub governance process overseeing the ongoing development work, as well as President of the GNOME Foundation board of directors. The GNOME Foundation has acted as fiscal sponsor for Flathub since this time, hiring a full-time devops engineer to operate the service, as well as providing legal support, operational costs, handling donations, managing and sponsoring development work.

In the past year, the GNOME Foundation has outsourced $50k of work to a combination of corporate and individual contractors active in the Flatpak community, which has worked extremely well to bring the combined expertise of Codethink and James Westman to developing our app verification, direct uploads, and adding Stripe integration with payments, donations, tax invoicing, card payments, receipts, etc.

We plan to continue the next phase of work in a similar manner, working with community contractors for the development work, and recruiting an additional staff member to the GNOME Foundation team to help establish the operations, review and security processes around the new paid service.

5. **How might this work be sustained long-term after an initial seed grant?**

Flathub is already governed by a desktop-neutral committee involving key representatives from GNOME Foundation and KDE e.V., and currently enjoys 1500 collaborators maintaining some 1800 apps on the existing service. In parallel with the technical development of the platform and launch of the app store functionality, the GNOME Foundation and KDE e.V. will be establishing a new legal entity, Flathub LLC to own and operate the service. We will establish a transparent governance process to help maintain community trust and accountability, and build an advisory board / sponsorship process to attract commercial sponsorship to the service in parallel to our grant applications.

The paid application service will be operated at a subsidized fee for free and open source software applications in support of the GNOME Foundation and KDE e.V’s shared missions, and running costs will be supported by the fees collected, and a combination of corporate sponsorship and grant funding.

### Resources needed

Our total budget for the coming year is 200k USD, including 120k USD towards salaries for a devops engineer and review/operations staff, USD 30k towards legal, professional and administration costs, and USD 50k towards the development of the software platform itself.

Our previous phase of implementing the Flathub appstore functionality was funded by a 50,000 USD grant from Dalio Philanthropies, and we are in the process confirming a subsequent 100,000 USD grant which will cover 50% of our planned budget for the coming year.

We are seeking up to 100,000 USD support from the Plaintext Group to cover the remaining budget to establish the new Flathub organisation and paid service over the coming year.

### Other links and resources

* [Flathub](https://flathub.org/)
* [Flathub Beta](https://beta.flathub.org/) -- including running preview of user accounts, app verification and vending functionality
* [GNOME Foundation](https://foundation.gnome.org/)
* [KDE e.V.](https://ev.kde.org/)
