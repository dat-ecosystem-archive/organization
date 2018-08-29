# Dat MOSS Grant Application

*Submitted April 2018*

Mozilla Open Source Support (MOSS) "Foundational Technology" Application
Mozilla’s mission is big and ambitious, and we couldn't achieve it without relying on software built by others in our community. We are eager to support you in your work on an open source/free software project that Mozilla relies on.

* Before applying please make sure you have read and met the criteria for the MOSS Program 'Foundational Technology' track (found at https://wiki.mozilla.org/MOSS/Foundational_Technology). In particular, in order to apply for a award, you must submit this application with the name of a Mozilla champion who has agreed to support it.
* If your application is successful, we may publish any part of this application which is not Personally Identifying Information, to promote program transparency and/or to serve as examples for other applicants.
* We recommend you join the public mailing list for MOSS at: https://lists.mozilla.org/listinfo/moss , to make sure you receive updates on the progress of the program.
* Reports suggest that Google Forms have a global character limit of 18-19k characters, over and above the limit on individual fields.

#### Selection Criteria 

All criteria are indicative rather than determinative - that is to say, they will make us more or less likely to make an award, but none will guarantee a particular outcome.

* How reliant is Mozilla on the project's technology?
* Do others also rely on it outside of Mozilla products?
* Is the technology unique? Are they doing something different?
* What role does the project play in the open source ecosystem?
* What sort of reputation does the project have in general, if any? This includes reputation in technical, inclusion and other areas
* Is the project known for something besides the code we are relying on?
* Will this award make a significant impact on the project?
* Is the level of funding appropriate for the task to be accomplished?
* Does the person (or group) who will receive the money have a track record of delivering?
* What does the champion have to say? Is the case compelling?

The minimum award for the Foundational Technology track is $10,000, and the maximum is $250,000.

---

## Application

### Project description:

Dat is a nonprofit-backed data sharing protocol for applications of the future. With software built for researchers and data management, Dat empowers people with decentralized data tools.

### Requested amount:

$230,000

### What are the concrete, specific outputs and outcomes this award would produce? 

*Please describe what you would use the funds for - what you are going to build, hack or fix, and how that would be of benefit to the world. As long as the costs are well explained, we are happy to consider funding activities whose benefit is harder to quantify than adding features - for example, maintenance, standardization, metrics, usability, user support, community building, tooling improvements, performance or documentation. Please also explain how you arrived at the dollar figure requested, by breaking it down as necessary into smaller pieces. The level of detail given should reflect how much money you are requesting; a $250k award will need much more detail than a $20k one. (Max 8k chars)*

Our community and ecosystem is rapidly expanding to new areas including arts & humanities, offline applications in the Global South, and libraries and archives. To see these decentralized communities flourish, we need support to continue improving the core and unique features of Dat. The five proposed milestones, below, will create the foundation for decentralized applications for communities across a wide range of industries from work like Mozilla's Common Voice to offline mapping in the Amazon done by Digitial Democracy. 

Through these milestones, we will improve the user experience of the core Dat features. The innovative features of Dat will create new potential for connection and openness on the web.

1. Multiwriter Integration for Dat Command line and Node Library ($51,000)

Over the last 6 months, we’ve been working hard on the low-level technology to allow multiple people to collaborate with a distributed file system. With this milestone, we will integrate this into the Dat command line and Node.js library. 

Once released, a new class of decentralized file management and data processing pipelines will be open to a wide range of users. Cloud-based file management and backup helped to spur a new wave of online collaboration tools but these tools lock users into specific providers, without having control of their data or being able to collaborate offline. With this milestone, developers will be able to use Dat to create peer-to-peer applications with location and owner-agnostic data pipelines on top of a solid foundation of privacy and security.

In the process of developing the low-level libraries for this, we’ve made Dat much faster for handling small files. While we have much of the underlying work completed. But we need to work on integrating these improvements into our user-facing applications. This work will also include best practice guide for key management and data backups, as this is a new area for many users.

With the completion of this milestone, users will be able to collaborate on decentralized file sharing applications with the Dat command line interface and Node library.

(4 months for 2 people)

2. Versioning Integration for Dat Command line and Node Library ($51,000)

While often essential to data analysis, versioning of datasets continues to be a difficult task – especially when it comes to accessing different versions quickly. By using technology popular in other blockchain systems, append-only logs, Dat enables data creators to automatically version datasets. However, unlike most blockchain software we do not require a global public log or excessive computation to verify new additions, bringing Dat more into line with the use cases of git. While everything added to Dat is versioned, we have yet to expose versioning interfaces in our user-facing tools.

Through this milestone, we will work with the Common Voice project at Mozilla to identify the needs around data versioning and user interfaces to make these accessible. We recognize that, if done poorly, these features could cause a lot of user confusion and frustration. By grounding this work in specific use cases, we hope to improve their implementations. Once complete, users will be able to access automatically versioned subsets of data alongside human-tagged versions. Additionally, to improve reproducibility, users can create permanent identifiers for specific versions of data for replicating research and computation results.

All of these features are available under-the-hood of Dat already, and are exposed in some advanced API interfaces. However, we have not had the resources to expose these features in the Node library or the Dat command line interface. This work will add APIs to the Dat Node.js library for managing, storing, and accessing different versions of data. In the Dat command line, we will allow users to interact with these underlying APIs to manage and create different versions of data.

(3 months for 2 people)

3. Selective File Downloads for Dat Command line and Node Library ($34,000)

With data moving around to more places, and becoming larger and larger, it’s more important than ever to be able to easily subset parts of a large dataset and only download the needed parts. For instance, in the Mozilla Common Voice project, the entire dataset is downloaded as a 12GB zip file and expected to continue growing. But within the dataset, there are separate subsets for training or other uses. Rather than downloading everything, Dat will enable users to download these on an as-needed basis, saving disk space and bandwidth.

This feature is available in the current command line but is not interactive. This work will add a command line interface for selecting and managing partial downloads for a given dataset. Paired with the versioning milestone, these milestones will allow users to download and manage different versions of the same dataset.

By combining these two features, we envision users can run data analysis on different versions of data without managing the datasets separately.

(2 months for 1 person)

4. Community Building, Protocol Documentation, and Tooling ($34,000)

Over the last four years, Dat has grown from a data sharing tool to a wider community supporting the Dat Protocol. As we work to broaden our community, we recognize the need to improve onboarding new community members, documentation, and supporting implementations in other languages. We’ve organized a Dat Protocol working group to document the existing specification and support other implementations, but we still need someone to help with wider community engagement. Unfortunately, with our constrained resources focusing on development and maintenance, these crucial needs get left behind.

While harder to quantify, we recognize that this work is vital to the future of the Dat Project and for collaborations with groups like Mozilla Common Voice. Investments in documentation and community building make it easy for people to use Dat, to suggest improvements, and get answers to questions. With this milestone, we will support someone to conduct user testing on existing documentation, create an improved user funnel, and identify additional community needs.

(4 months for 1 person)

5. Improved Network Analytics and Tooling ($25,500)

One of our recurring challenges in building decentralized applications is providing analytics and debugging network problems. For example, in our work with libraries, the institutions want a measure of how often an asset it used so they can prioritize preservation and improved availability. Because not all downloads go through a single server, we have to use alternate methods for providing needed information about use.

In this milestone, we will create tooling for institution-focused analytics and debugging. These services will work with existing Dat discovery services and institutional software to provide improve analytics about data usage in Dat.

(3 months for 1 person)

Milestones Total: $195,500
Overhead: $34,500 (15% for Code for Science & Society)
Total: $230,000

This award will make a significant impact on the project, allowing us to bring on paid contributors who have previously been volunteers or short-term contractors. As an entirely grant-funded project, our funding is often project-based, making it more difficult to improve our core tooling. This award would be vital support for areas we have been under-resourced. 

### Please share an endorsement from your Mozillian champion:

*Ask your champion to write a paragraph or two on why supporting your work via this award is a great idea. This is not just about whether the goal is important, but also about whether you are the right team to achieve it. All endorsements must include the sentence: "I have read the text of this application and I believe the applicants are technically capable of achieving the work outlined." (Max 4k chars)*

*[Redacted]*

### Please tell us more about how your project is managed. Please describe your core team.

The Dat Project is an open source project with independent governance that is fiscally sponsored by the nonprofit Code for Science & Society (CS&S). The Dat Project is managed by three working groups that cover maintenance and development of the protocol (Protocol Working Group), community engagement (Community Working Group), and the project’s strategy, management, and funding (Core Governance Team). 

The Dat Protocol Working Group (PWG) governs changes to the protocol and is tasked with documenting existing implementations. We convened this team to enable community members to create Dat implementations in other languages. This team meets biweekly, and more information on their work including membership and past meeting minutes can be found https://github.com/datprotocol/working-group.

We are forming a Community Working Group (CWG) to manage Code of Conduct, review documentation designed to welcome folks to the project (Contributing Guide, etc), respond to issues within the community, and develop resources and guidelines to keep the community safe and inclusive. The CWG will meet monthly and new members are on-boarded annually, we expect this group to start with approximately 6 people.

The Dat Core Governance Team team is currently made up of four core Dat contributors and CSS leadership. This team develops the project’s strategic goals, assesses the project’s progress, makes decisions on Dat’s participation in partnerships and projects, writes grants and pursues funding to support work on Dat. The Core Governance Team contains members of both the PWG and the CWG, who keep the strategy team informed of activities and issues in those groups. This team also writes blog posts (https://blog.datproject.org/) and other public communication about the direction and priorities of the project, often in collaboration with the PWG and CWG. Membership on this team is limited to people who have more than one year of sustained involvement in Dat and can bring other skills and expertise (grant writing, financial planning, strategic partnerships) to the group. 

### Please tell us more about your community.

The Dat Project community brings together people working across different domains to solve problems of decentralized networks and data transfer. Our community includes researchers and scientists, people building peer-to-peer web applications, and activists committed to open public data. Our community is unified in its belief that decentralized approaches are a critical part of a better web. Dat participates in the quaretely Code for Science & Society Community calls, a summary of the last call is here.


Projects with existing code and an existing community are preferred but this is not decisive.
If you have participation guidelines / code of conduct please include pointers to them.

Code of Conduct  - https://github.com/datproject/Code-of-Conduct/blob/master/CODE_OF_CONDUCT.md
Contributing Guidelines - https://github.com/datproject/dat/blob/master/CONTRIBUTING.md



