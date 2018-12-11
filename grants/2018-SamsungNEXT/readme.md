
# Samsung NEXT Stack Zero Grant

> Description: a non-equity grant program that aims to support early-stage teams building decentralized technologies with funding, expertise, and access to the Samsung NEXT network.

https://samsungnext.com/whats-next/introducing-the-samsung-next-stack-zero-grant/


## Application: Dat CLI and Evangelism

> 1. First, tell us your project's name.**
 
Distributed real-time file sharing, by The Dat Project
 
> 2. Give us your high-level pitch and tell us what problem you're trying to solve

Ever tried collaboratively editing large files and folders with multiple machines? Usually this involves one of a few strategies: being in the same location (usb), using a cloud service (Dropbox, email), or using old but reliable technical tools (rsync). None of these easily store, track, and share your data over time. Git is the closest tool in wide use today, but is designed for editing source code, not large datasets. Because Git was designed to track changes to relatively small text files, many datasets are too big for it. While Git has revolutionized the way that open source code is written for the software development world, workflows around sharing data remain primitive. Users are stuck choosing between security, speed, or ease of use. So, we've taken the best parts of Git, BitTorrent, and Dropbox to design Dat, a next-generation file sharing tool that has the potential to rival all three. 

Dat boasts a host of user-facing applications, including a command line tool, desktop application, web browser, and a wide variety of modules for storing and sharing data. When data is shared with Dat, other users with the link can copy, modify, and contribute back to that data if they are granted permission. Our approach is to give a practical strategy for avoiding privatized and siloed data storage services that dominate the space. Dat is simple: we believe that by keeping Dat focused on low-level data version control and replication tasks, we can keep the user interface simple and encourage collaboration across data silos, improving the interoperability, transparency, and openness of the data shared on the web.


> 3. Which fields or areas does your technology impact the most? Feel free to use comma-separated tags.

Distributed applications, Peer-to-peer web

> 4. Do you have a website? A public code repository would do.

datproject.org

> 5. Where is the team based? If distributed, give us a general idea.

We work with community members globally. The grant would be managed by Dat's core governance team based in Portland, OR, Oakland, and Denmark. 
 
> 6. If accepted, how will you utilize the grant?

Currently, the command line tool has no core maintainers, while the list of feature requests has increased substantially. This grant would be used to support the equivalent of one core software developer at 8k per month. 

The following activities are planned within the course of the grant. Proposed timelines are if the full 70k are granted, and would be adjusted accordingly for smaller award sizes.

Objective 1:  Needfinding and Maintenance (3 months)

*   Full triage and prioritization of open and outstanding bugs on the datproject/dat GitHub repository. 
*   Bug fixing for the most pressing issues with accompanying tests.
*   Facilitation of weekly Dat community sync meetings where developer-volunteers can learn about the next steps, blockers, and pressing issues for the CLI tool.

Objective 2: Feature parity with similar tools (4 months)

*   Modify the history of an archive to create branches and perform merges, just like git. This is a long-standing feature request which exists in the Dat web browser called Beaker, but not yet in the command line tool. 
*   Run a daemon that manages local Dat instances, exposing commands through a local tcp connection that can be queried from other applications. This is a feature that exists in similar tools such as ipfs.
*   Pass more detailed options for specifying how the client machine accesses the network, such as bandwidth caps and bootstrap servers for peer discovery. These options are already available in lower-level APIs, but need to be exposed through easy-to-use interface. 

Objective 3: Documentation (1 month)

*   A thorough documentation review of the command line tool, including interviews with developer-users. 
*   Complete update of the documentation, including a review of the interactive 'Try Dat' user guide.

> 7. Tell us your story: how long have you been working on this project, how is the community involved, or any other detail you want.

The governance team currently consists of Mathias Buus, Karissa McKelvey, Joe Hand, and Danielle Robinson. Our team has long experience in open access and data problem solving, and each team member is committed to creating more open access to knowledge. The team comes directly from academia, and have been working on open source technology for most of their careers. Finally, our team builds code modularly, meaning that even "failure" of our implementation with a particular partner could still see the overall project succeed in unforeseen ways, by emitting components that can have impact on their own.

The first code went into Dat on August 17, 2013. Throughout its history, Dat has had a primary focus on Dat sharing in civic data and research. The team grew to include 8 people at its height in 2016, with both Sloan foundation and Knight Foundation funding. Together, we created a community of open data advocates who use dat to publish data as decentralized public resources. The core command line tool has an important role to play by providing a solid foundation that can be used across organizations that need to share data seamlessly, securely, and efficiently. 

The command line tool's GitHub repository now has over 7,200 followers, and a wide variety of contributors. Dat is an open source project with community governance through a set of working groups. Over the next year, we aim to create a sustainable model for Dat through consulting contracts, grants, and donations. We've already begun this process, but need help with core maintenance support for the basic file sharing tool, and maintenance is difficult to fund.

> 8. What is the most groundbreaking thing about your solution?

Collaborative, versioned development and distribution is a useful model for many data-driven tasks — not just for source code. For people and organizations accustomed to a Git-based development model, it is natural to want to extend that model to data. For example, those who sit at the nexus of software development and data production — librarians, scientists, government agencies, etc.— have started using Git for the development and distribution of datasets. However, many data managers post their raw data online as read-only, never taking contributions from peers and downstream contributors, because there is no system in place for tracking changes to the data. Git enables code to get better as more people use it, because it enables collaboration between programmers. For lack of similar systems for data, improvements to data rarely make it back to the original dataset in this way. 

Dat is built with Node.js, which we use because of its excellent cross-platform support (Linux, Mac, and Windows) as well as its emphasis on data streaming. This means that Dat will never crash if you put too much data into it. The upper limit in terms of dataset size depends on available storage and bandwidth. To test Dat's capability to work with large datasets, we worked with *RESEARCHER*, of Ohio State University, and *RESEARCHER2*, a data analyst and programmer, to build a system for importing and indexing the 400 GB Wide-field Infrared Survey Explorer (WISE) dataset from NASA/Caltech, which includes data on over 600 million stars. We were able to effectively build a query engine on top of Dat that allowed users to get access to particular data on any cluster of stars in the sky. In this way, a scientist could use a Dat HTTP endpoint to refer to a particular set of data that they used in their analysis, getting data points immediately, despite the large size of the initial dataset. This versioned workflow and query engine would be time-consuming to build, and necessarily out of reach for most researchers without Dat.

> 9. How does your solution further decentralization?

Our primary audiences to date include the scientific research community, librarians, open government/civic data hackers, activists, and data scientists. Bringing decentralized technology to these hard-to-reach sectors is a crucial step towards the legitimization of decentralized technology in the public sphere. Over the years, we have chosen development priorities through conversations with data-driven researchers and open data experts at GovLab, Freeman Lab, FiveThirtyEight, California Civic Data Coalition, Wikimedia Community, California Digital Library, Indiana University, Trillian Project, The Wurm Lab, USGS, Ocean Health Index, International Monetary Fund, Data & Society, BetaNYC, Digital Ocean, and Jupyter Project. Through these personal relationships, we have identified significant pain points that span the open data landscape centered around the discovery and distribution of data. By offering a simple command line tool, we increase the interoperability of decentralized data storage and access between organizations like these.

> 10. Where can we find you online (social media, Gitlab, Github, etc.)?

@dat_project, github.com/datproject

> 11. How should we contact you (e-mail or other)?

hi@datproject.org
