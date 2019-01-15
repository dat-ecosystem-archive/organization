
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


## Enabling Multi-User Collaboration with the Hyper* Ecosystem

> 1. First, tell us your project's name.**
 
Distributed real-time file sharing, by The Dat Project
 
> 2. Give us your high-level pitch and tell us what problem you're trying to solve

Decentralized software has potential to return control of digital information to the people. Yet, wide adoption of peer-to-peer technology is hindered by technical and ethical challenges. Dat Project is an open source, community driven, nonprofit-backed initiative that develops peer-to-peer tools to reimagine how information is owned, shared, and accessed. With Dat, the secure, fully-decentralized sharing of dynamic data is as easy as sharing a web link. Dat achieves this by building on a suite of modular components for data discovery, storage, and indexing called the Hyper* stack.

The Hyper* stack occupies a unique spot in the world of decentralized tech: easy-to-use Lego blocks for building decentralized applications. At its core lies a cryptographically-secure append-only log, somewhat like a blockchain minus the strong consistency requirement, that we’ve named a “hypercore.” Using a hypercore, it’s dead-simple for a single writer to securely and efficiently distribute an ever-changing dataset to its readers, with no risk of tampering, no need for always-on connectivity, and no wasted bandwidth. For a huge class of P2P applications, this simple primitive has proven transformative.

A worldwide ecosystem of developers is already using Hyper* modules as building blocks to solve novel problems for their communities, many far beyond Dat’s original scope. Over 200 public NPM projects currently depend on Hyper*, with major projects including a P2P web browser (Beaker Browser), a desktop science library (Science Fair) and a user-controlled alternative to YouTube (Hypervision).

Our community has already built incredible things on the single-writer version of Hyper*, yet years of feedback reveal crucial missing pieces, the foremost being a lack of multi-user collaboration. We believe allowing multiple writers to modify a shared, distributed hypercore will lay the foundation for groundbreaking decentralized applications that put community ownership of digital information first. Even better, our existing users have laundry lists of radical improvements to their existing systems that depend on multi-user features. Beaker wants to enable new tools for collaborative publishing on the web. Science Fair wants to fundamentally change the peer-review process, where papers, annotations, and comments can be fluidly exchanged between collaborators. The list goes on.

Our users are eagerly waiting; we’re very excited to deliver these features to them.

> 3. Which fields or areas does your technology impact the most? Feel free to use comma-separated tags.

Developer tools, Data Science, Distributed computing, Networking

> 4. Do you have a website? A public code repository would do.

datproject.org

> 5. Where is the team based? If distributed, give us a general idea.

We work with community members globally. The grant would be managed by Dat's core governance team based in Portland, OR, Oakland, and Denmark. 
 
> 6. If accepted, how will you utilize the grant?



As of now, all development on the Hyper* stack is done by module consumers, application developers who depend on the stack but have primary obligations elsewhere. This grant will fund a dedicated developer ($8k/month for one year) to work on critical improvements to our low-level modules and protocol specifications that will enable collaborative peer-to-peer data sharing.

To give clarity, here's a brief overview of the relevant modules in the Hyper* ecosystem, along with how they're currently used:



*   **_Hypercore _**is our bread and butter. It's an append-only log combined with a Merkle tree whose cryptographic properties make it easy to efficiently distribute among untrusted peers. Fundamentally, a hypercore only has a single writer, but allows for many readers.
*   **_Hyperdrive _**behaves more like a P2P Dropbox. It's a distributed filesystem that, under the hood, is just two hypercores. Like hypercore, the current version of hyperdrive only supports a single writer with many readers.
*   **_Hyperdb _**combines many hypercores, from different writers, into a single directory-structured view. This is the key step that enables multi-user collaboration! It's powered by a trie-like data structure, and uses vector clocks to ensure correct ordering.
*   **_Hypertrie_** is the core data structure currently used in hyperdb, but extract into its own module and with multiple performance improvements. It only allows for a single writer, but provides hyperdb's kv-store interface.
*   **_Hyperswarm _**is the next generation of our networking stack. It focused on provided easy to use APIs for things like UDP hole punching (NAT traversal), distributed discovery using modular DHTs, and authenticated connectivity using the NOISE framework.

We've spent time implementing these foundational pieces for multi-user collaboration. The next step is to integrate these components into our stack as first-class citizens, then deploy them to users. Our developer will perform the following tasks to achieve this goal:

<span style="text-decoration:underline;">Test hypertrie performance in hyperdrive</span>

By deploying a hypertrie-backed version of hyperdrive to users, we'll be able to test the performance of the data structure while retaining our current single-writer API. With this change alone, we're anticipating a large performance boost for hyperdrive, which will be a boon to existing projects built on Hyper*.

Since this step happens behind the scenes and does not alter our public APIs, it won't involve any additional documentation. We will, however, gather community feedback about performance and stability to ensure that no regressions have occured.

<span style="text-decoration:underline;">Integrate hypertrie into hyperdb</span>

By separating core data structures (hypertrie) from coordination logic, we have the opportunity to create a more modular version of hyperdb which can combine each writer's trie in novel ways (to support union mounting and symlinking, for example, both of which are not possible in our current prototype).

With this feature complete, we'll have an extensible, fast, multi-user database that will serve as the backbone both for the next iteration of Dat, and for apps which currently depend on our hyperdb prototype.

<span style="text-decoration:underline;">Integrate hyperdb into hyperdrive</span>

Once we're confident that our hypertrie-based version of hyperdb performs correctly, we can then replace hypertrie with hyperdb in hyperdrive. Since hyperdb exposes a superset of the hypertrie API, this will not be a breaking change for any existing applications.

Most importantly, this will give us access to hyperdb's multi-user collaboration API in hyperdrive, which is the top-level module in the Hyper* stack. Since most of the ecosystem, including the Dat CLI tool itself, is built on hyperdrive, we anticipate that this change will have the largest impact on the community.

Deploying this step to users will be the final task in our push to deploy multi-user collaboration.

<span style="text-decoration:underline;">Add noise-network to discovery modules</span>

Currently the Hyper* stack uses a capability system for authentication. This capability system works similar to something Github gists where you share a secret link that gives you access to read the underlying data.

Based on community feedback we want to expand this into a fully featured authentication system that gives users the ability to whitelist exactly which peers they want to provide access to, and also a way to revoke that access. We've already implemented the cryptographic part of this in a module called noise-network and the next step will be to integrate this functionality into the actual stack.


> 7. Tell us your story: how long have you been working on this project, how is the community involved, or any other detail you want.

The first code went into Dat on August 17, 2013. Throughout its history, Dat has had a primary focus on data sharing in civic data and research, only recently with a wider focus on more general decentralized applications. We quickly realized that Dat had potential beyond than open data sharing, and began applying it to everything that uses a file system -- including websites and applications.

We now have over 30 partners who are directly using our code, and a network of over 7,200 open source developers who are following us. Our adopters are diverse: from indigenous people protecting the Amazon rainforest (Digital Democracy) to librarians preserving scientific artifacts (California Digital Library). What these projects have in common is that they embed the values of decentralized ownership directly into the code. 

> 8. What is the most groundbreaking thing about your solution?

The Hyper* ecosystem is unlike any other P2P project out there. While other decentralization projects build monolithic systems that require total buy-in from developers, we’ve instead chosen to embrace the Unix philosophy at all levels of our stack: build small component that do one thing well. Mixing and matching these components allows users to build powerful applications we never could have anticipated at the outset, and the possible combinations are endless. We believe the emergence of our sizable community reflects the value and utility of these principles.

Adding more collaborative data structures in addition to upgrades our existing modules will make the stack even more powerful and we are super excited about the future projects this will allow users to build.

> 9. How does your solution further decentralization?

By creating a modular core of reusable, stable, well-documented modules, we aim to enable a lot with a little. Developers in our community often know how each module works, how it can be replaced if necessary, and how it fits together with other modules to accomplish a high-level task.

Our “standard library” of reusable components spans a variety of features that developers often want: video streaming (hypervision), versioning (dat), file sharing (hyperdrive), distributed p2p database (hyperdb), graph structures (hypercore-graph), consensus (hyperquorum), distributed indexes (hypertrie), swarming data exchange on intermittent connections (hyperswarm), and encrypted p2p communication (noise-peer), to list just a handful. Importantly, most of these components are, under the hood, just different ways of arranging hypercores! 

Once developers understand our core principles, they are empowered to play with and rearrange our modules as they see fit for their own use-cases. The total is greater than the sum of its parts.

> 10. Where can we find you online (social media, Gitlab, Github, etc.)?

@dat_project, github.com/datproject

> 11. How should we contact you (e-mail or other)?

hi@datproject.org
