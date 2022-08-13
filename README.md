Ruang lingkup software engineering.
Software engineering
Software engineering is a systematic engineering approach to software development. Engineering techniques are used to inform[clarification needed] the software development process which involves the definition, implementation, assessment, measurement, management, change, and improvement of the software life cycle process itself. 
It heavily uses software configuration management  which is about systematically controlling changes to the configuration, and maintaining the integrity and traceability of the configuration and code throughout the system life cycle. Modern processes use software versioning.
Definitions and terminology controversies
Notable definitions of software engineering include:
1. "The systematic application of scientific and technological knowledge, methods, and experience to the design, implementation, testing, and documentation of software"—The Bureau of Labor Statistics—IEEE Systems and software engineering – Vocabulary.
2. "The application of a systematic, disciplined, quantifiable approach to the development, operation, and maintenance of software"—IEEE Standard Glossary of Software Engineering Terminology.
3. "an engineering discipline that is concerned with all aspects of software production"—Ian Sommerville.
4. "the establishment and use of sound engineering principles in order to economically obtain software that is reliable and works efficiently on real machines"—Fritz Bauer.
5. "a branch of computer science that deals with the design, implementation, and maintenance of complex computer programs"—Merriam-Webster.
6. "'software engineering' encompasses not just the act of writing code, but all of the tools and processes an organization uses to build and maintain that code over time. [...] Software engineering can be thought of as 'programming integrated over time.'"—Software Engineering at Google.
 The term has also been used less formally: 
1. as the informal contemporary term for the broad range of activities that were formerly called computer programming and systems analysis;[23]
2. as the broad term for all aspects of the practice of computer programming, as opposed to the theory of computer programming, which is formally studied as a sub-discipline of computer science;[24]
3. as the term embodying the advocacy of a specific approach to computer programming, one that urges that it be treated as an engineering discipline rather than an art or a craft, and advocates the codification of recommended practices.
 Software requirements
   Requirements engineering is about the elicitation, analysis, specification, and validation of requirements for software. Software requirements can be of three different types. There are functional requirements, non-functional requirements, and domain requirements. The operation of the software should be performed and the proper output should be expected for   the user to use.
 Software design
 Software design is about the process of defining the architecture, components, interfaces, and other characteristics of a system or component. This is also called software architecture. Software design is divided into three different levels of design. The three levels are interface design, architectural design, and detailed design. Interface design is the interaction between a system and its environment. This happens at a high level of abstraction along with the inner workings of the system. Architectural design has to do with the major components of a system and their responsibilities, properties, interfaces, and their relationships and interactions that occur between them. Detailed design is the internal elements of all the major system components, their properties, relationships, processing, and usually their algorithms and the data structures.      
Software construction
Software construction, the main activity of software development, is the combination of programming, unit testing, integration testing, and debugging. Testing during this phase is generally performed by the programmer while the software is under construction, to verify what was just written and decide when the code is ready to be sent to the next step.
Software testing
Software testing is an empirical, technical investigation conducted to provide stakeholders with information about the quality of the product or service under test, with different approaches such as unit testing and integration testing. It is one aspect of software quality. As a separate phase in software development, it is typically performed by quality assurance staff or a developer other than the one who wrote the code.
Software maintenance
Software maintenance refers to the activities required to provide cost-effective support after shipping the software product. Software maintenance is modifying and updating software applications after distribution to correct faults and to improve its performance. Software has a lot to do with the real world and when the real world changes, software maintenance is required. Software maintenance includes: error correction, optimization, deletion of unused and discarded features, and enhancement of features that already exist. Usually, maintenance takes up about 40% to 80% of the project cost therefore, focusing on maintenance keeps the costs down.
Keterkaitan software engineering dengan SCM - Software Configuration Management.
Software configuration management
In software engineering, software configuration management (SCM or S/W CM) is the task of tracking and controlling changes in the software, part of the larger cross-disciplinary field of configuration management. SCM practices include revision control and the establishment of baselines. If something goes wrong, SCM can determine the "what, when, why and who" of the change. If a configuration is working well, SCM can determine how to replicate it across many hosts.
The acronym "SCM" is also expanded as source configuration management process and software change and configuration management. However, "configuration" is generally understood to cover changes typically made by a system administrator.
Purposes
The goals of SCM are generally:
1.	Configuration identification - Identifying configurations, configuration items and baselines.
2.	Configuration control - Implementing a controlled change process. This is usually achieved by setting up a change control board whose primary function is to approve or reject all change requests that are sent against any baseline.
3.	Configuration status accounting - Recording and reporting all the necessary information on the status of the development process.
4.	Configuration auditing - Ensuring that configurations contain all their intended parts and are sound with respect to their specifying documents, including requirements, architectural specifications and user manuals.
5.	Build management - Managing the process and tools used for builds.
6.	Process management - Ensuring adherence to the organization's development process.
7.	Environment management - Managing the software and hardware that host the system.
8.	Teamwork - Facilitate team interactions related to the process.
9.	Defect tracking - Making sure every defect has traceability back to the source.

Keterkaitan SCM dengan Version Control dan Distributed Version Control.
Version control
In software engineering, version control (also known as revision control, source control, or source code management) is a class of systems responsible for managing changes to computer programs, documents, large web sites, or other collections of information. Version control is a component of software configuration management.
Changes are usually identified by a number or letter code, termed the "revision number", "revision level", or simply "revision". For example, an initial set of files is "revision 1". When the first change is made, the resulting set is "revision 2", and so on. Each revision is associated with a timestamp and the person making the change. Revisions can be compared, restored, and, with some types of files, merged.
Version control systems are most commonly run as stand-alone applications, but revision control is also embedded in various types of software, such as word processors and spreadsheets, collaborative web docs,[3] and content management systems, e.g., Wikipedia's page history. Revision control enables reverting a document to a previous revision, which is critical for allowing editors to track each other's edits, correct mistakes, and defend against vandalism and spamming in wikis.
Overview
In computer software engineering, revision control is any kind of practice that tracks and provides control over changes to source code. Software developers sometimes use revision control software to maintain documentation and configuration files as well as source code.
Bugs or features of the software are often only present in certain versions (because of the fixing of some problems and the introduction of others as the program develops). Therefore, for the purposes of locating and fixing bugs, it is vitally important to be able to retrieve and run different versions of the software to determine in which version(s) the problem occurs. It may also be necessary to develop two versions of the software concurrently: for instance, where one version has bugs fixed, but no new features (branch), while the other version is where new features are worked on (trunk).
Structure
Graph structure
In terms of graph theory, revisions are generally thought of as a line of development (the trunk) with branches off of this, forming a directed tree, visualized as one or more parallel lines of development (the "mainlines" of the branches) branching off a trunk. In reality the structure is more complicated, forming a directed acyclic graph, but for many purposes "tree with merges" is an adequate approximation.
Revisions occur in sequence over time, and thus can be arranged in order, either by revision number or timestamp. In the simplest case, with no branching or undoing, each revision is based on its immediate predecessor alone, and they form a simple line, with a single latest version, the "HEAD" revision or tip. In graph theory terms, drawing each revision as a point and each "derived revision" relationship as an arrow (conventionally pointing from older to newer, in the same direction as time), this is a linear graph.
Source-management models
1. Atomic operations
An operation is atomic if the system is left in a consistent state even if the operation is interrupted. The commit operation is usually the most critical in this sense. Commits tell the revision control system to make a group of changes final, and available to all users. Not all revision control systems have atomic commits; Concurrent Versions System lacks this feature.
2. File Locking
File locking has both merits and drawbacks. If the files are left exclusively locked for too long, other developers may be tempted to bypass the revision control software and change the files locally, forcing a difficult manual merge when the other changes are finally checked in. In a large organization, files can be left "checked out" and locked and forgotten about as developers move between projects - these tools may or may not make it easy to see who has a file checked out.
3.  Version merging
Most version control systems allow multiple developers to edit the same file at the same time. The first developer to "check in" changes to the central repository always succeeds. The system may provide facilities to merge further changes into the central repository, and preserve the changes from the first developer when other developers check in.
Merging two files can be a very delicate operation, and usually possible only if the data structure is simple, as in text files. The result of a merge of two image files might not result in an image file at all. The second developer checking in the code will need to take care with the merge, to make sure that the changes are compatible and that the merge operation does not introduce its own logic errors within the files. These problems limit the availability of automatic or semi-automatic merge operations mainly to simple text-based documents, unless a specific merge plugin is available for the file types.
4. Baselines, labels and tags
Most revision control tools will use only one of these similar terms (baseline, label, tag) to refer to the action of identifying a snapshot ("label the project") or the record of the snapshot ("try it with baseline X"). Typically only one of the terms baseline, label, or tag is used in documentation or discussion they can be considered synonyms.
In most projects, some snapshots are more significant than others, such as those used to indicate published releases, branches, or milestones.
When both the term baseline and either of label or tag are used together in the same context, label and tag usually refer to the mechanism within the tool of identifying or making the record of the snapshot, and baseline indicates the increased significance of any given label or tag. 
Common terminology
Terminology can vary from system to system, but some terms in common usage include:
1. Baseline
An approved revision of a document or source file to which subsequent changes can be made. See baselines, labels and tags.
2. Blame
A search for the author and revision that last modified a particular line.
3. Branch
A set of files under version control may be branched or forked at a point in time so that, from that time forward, two copies of those files may develop at different speeds or in different ways independently of each other.
4. Change
A change (or diff, or delta) represents a specific modification to a document under version control. The granularity of the modification considered a change varies between version control systems.
5. Change list
On many version control systems with atomic multi-change commits, a change list (or CL), change set, update, or patch identifies the set of changes made in a single commit. This can also represent a sequential view of the source code, allowing the examination of source as of any particular changelist ID.
6. Checkout
To check out (or co) is to create a local working copy from the repository. A user may specify a specific revision or obtain the latest. The term 'checkout' can also be used as a noun to describe the working copy. When a file has been checked out from a shared file server, it cannot be edited by other users. Think of it like a hotel, when you check out, you no longer have access to its amenities.
7. Clone
Cloning means creating a repository containing the revisions from another repository. This is equivalent to pushing or pulling into an empty (newly initialized) repository. As a noun, two repositories can be said to be clones if they are kept synchronized, and contain the same revisions.
8. Commit (noun)
A 'commit' or 'revision' (SVN) is a modification that is applied to the repository.
9. Commit (verb)
To commit (check in, ci or, more rarely, install, submit or record) is to write or merge the changes made in the working copy back to the repository. A commit contains metadata, typically the author information and a commit message that describes the change.
10. Conflict
A conflict occurs when different parties make changes to the same document, and the system is unable to reconcile the changes. A user must resolve the conflict by combining the changes, or by selecting one change in favour of the other.
11. Delta compression
Most revision control software uses delta compression, which retains only the differences between successive versions of files. This allows for more efficient storage of many different versions of files.
12. Dynamic stream
A stream in which some or all file versions are mirrors of the parent stream's versions.
13. Export
Exporting is the act of obtaining the files from the repository. It is similar to checking out except that it creates a clean directory tree without the version-control metadata used in a working copy. This is often used prior to publishing the contents, for example.
14. Fetch
See pull.
15. Forward integration
The process of merging changes made in the main trunk into a development (feature or team) branch.
16. Head
Also sometimes called tip, this refers to the most recent commit, either to the trunk or to a branch. The trunk and each branch have their own head, though HEAD is sometimes loosely used to refer to the trunk.[14]
17. Import
Importing is the act of copying a local directory tree (that is not currently a working copy) into the repository for the first time.
18. Initialize
To create a new, empty repository.
19. Interleaved deltas
Some revision control software uses Interleaved deltas, a method that allows storing the history of text based files in a more efficient way than by using Delta compression.
20. Label
See tag.
21. Locking
When a developer locks a file, no one else can update that file until it is unlocked. Locking can be supported by the version control system, or via informal communications between developers (aka social locking).
22. Mainline
Similar to trunk, but there can be a mainline for each branch.
23. Merge
A merge or integration is an operation in which two sets of changes are applied to a file or set of files. Some sample scenarios are as follows:
•	A user, working on a set of files, updates or syncs their working copy with changes made, and checked into the repository, by other users.[15]
•	A user tries to check in files that have been updated by others since the files were checked out, and the revision control software automatically merges the files (typically, after prompting the user if it should proceed with the automatic merge, and in some cases only doing so if the merge can be clearly and reasonably resolved).
•	A branch is created, the code in the files is independently edited, and the updated branch is later incorporated into a single, unified trunk.
•	A set of files is branched, a problem that existed before the branching is fixed in one branch, and the fix is then merged into the other branch. (This type of selective merge is sometimes known as a cherry pick to distinguish it from the complete merge in the previous case.)
24. Promote
The act of copying file content from a less controlled location into a more controlled location. For example, from a user's workspace into a repository, or from a stream to its parent.[16]
25. Pull, push
Copy revisions from one repository into another. Pull is initiated by the receiving repository, while push is initiated by the source. Fetch is sometimes used as a synonym for pull, or to mean a pull followed by an update.
26. Pull request
A developer asking others to merge their "pushed" changes.
27. Repository
The repository (or "repo") is where files' current and historical data are stored, often on a server. Sometimes also called a depot.
28. Resolve
The act of user intervention to address a conflict between different changes to the same document.
29. Reverse integration
The process of merging different team branches into the main trunk of the versioning system.
30. Revision
Also version: A version is any change in form. In SVK, a Revision is the state at a point in time of the entire tree in the repository.
31. Share
The act of making one file or folder available in multiple branches at the same time. When a shared file is changed in one branch, it is changed in other branches.
32. Stream
A container for branched files that has a known relationship to other such containers. Streams form a hierarchy; each stream can inherit various properties (like versions, namespace, workflow rules, subscribers, etc.) from its parent stream.
33. Tag
A tag or label refers to an important snapshot in time, consistent across many files. These files at that point may all be tagged with a user-friendly, meaningful name or revision number. See baselines, labels and tags.
34. Trunk
The unique line of development that is not a branch 
35. Update
An update (or sync, but sync can also mean a combined push and pull) merges changes made in the repository (by other people, for example) into the local working copy. Update is also the term used by some CM tools (CM+, PLS, SMS) for the change package concept (see changelist). Synonymous with checkout in revision control systems that require each repository to have exactly one working copy (common in distributed systems)
36. Unlocking
releasing a lock.
37. Working copy
The working copy is the local copy of files from a repository, at a specific time or revision. All work done to the files in a repository is initially done on a working copy, hence the name. Conceptually, it is a sandbox.
Distributed version control
Distributed vs. centralized
Advantages of DVCS (compared with centralized systems) include:
•	Allows users to work productively when not connected to a network.
•	Common operations (such as commits, viewing history, and reverting changes) are faster for DVCS, because there is no need to communicate with a central server. With DVCS, communication is necessary only when sharing changes among other peers.
•	Allows private work, so users can use their changes even for early drafts they do not want to publish.
•	Working copies effectively function as remote backups, which avoids relying on one physical machine as a single point of failure.
•	Allows various development models to be used, such as using development branches or a Commander/Lieutenant model.
•	Permits centralized control of the "release version" of the project
•	On FOSS software projects it is much easier to create a project fork from a project that is stalled because of leadership conflicts or design disagreements
Disadvantages of DVCS (compared with centralized systems) include:
•	Initial checkout of a repository is slower as compared to checkout in a centralized version control system, because all branches and revision history are copied to the local machine by default.
•	The lack of locking mechanisms that is part of most centralized VCS and still plays an important role when it comes to non-mergeable binary files such as graphic assets or too complex single file binary or XML packages (e.g. office documents, PowerBI files, SQL Server Data Tools BI packages, etc.).
•	Additional storage required for every user to have a complete copy of the complete codebase history.
•	Increased exposure of the code base since every participant has a locally vulnerable copy
Work model
1. Central and branch repositories
2. Pull requests
Getting Started - About Version Control
About Version Control
1. Local Version Control Systems
Many people’s version-control method of choice is to copy files into another directory (perhaps a time-stamped directory, if they’re clever). This approach is very common because it is so simple, but it is also incredibly error prone. It is easy to forget which directory you’re in and accidentally write to the wrong file or copy over files you don’t mean to.
To deal with this issue, programmers long ago developed local VCSs that had a simple database that kept all the changes to files under revision control.
2. Centralized Version Control Systems
The next major issue that people encounter is that they need to collaborate with developers on other systems. To deal with this problem, Centralized Version Control Systems (CVCSs) were developed. These systems (such as CVS, Subversion, and Perforce) have a single server that contains all the versioned files, and a number of clients that check out files from that central place. For many years, this has been the standard for version control.
3. Distributed Version Control Systems
This is where Distributed Version Control Systems (DVCSs) step in. In a DVCS (such as Git, Mercurial, Bazaar or Darcs), clients don’t just check out the latest snapshot of the files; rather, they fully mirror the repository, including its full history. Thus, if any server dies, and these systems were collaborating via that server, any of the client repositories can be copied back up to the server to restore it. Every clone is really a full backup of all the data.
