# Michael Hitchcock 
## 13321 SE Linden Lane, Milwaukie OR 97222 / 503.997.0552 / mdhitchcock@gmail.com

Full stack developer with deep roots in each part of the stack. 

My 25+ years of computer-related work has been a progression through three realms: the first four years I was a UNIX sysadmin and taught myself enough to become network manager for a small tech shop. The next twelve years I worked on 'back-end' server-side programming and built a patented forms engine out of Apache, Perl, Tomcat, Java servlets, and DB2, capable of hosting thousands of college applications and other forms.

For the last nine and a half years I explored the 'front-end' client-side world of well-crafted dynamic web pages and consuming web services, by mastering Javascript, learning CSS and HTML5, and more recently helping build a single page app with Angular2 and Typescript. 

I remain keenly interested in continuing to learn this space and tackling the next challenge.

# Skills

* Expert: Javascript, HTML, DOM, JSON, vi/vim, \*nix, git, regexes
* Solid: Node, express, grunt and gulp, jQuery, SQL, MongoDB and mongoose, CSS, shell scripting, REST, XP/Agile/Scrum, jasmine/mocha, Chrome DevTools, Jenkins, AEM (Adobe Experience Manager, aka CQ), BitBucket, GitHub
* Novice: Typescript, Angular2, Less, SASS, ES6, responsive pages
* Currently investigating: React, Redux, AWS
* Formerly Expert: Perl, Apache, mod_perl, XML, Java, Tomcat, Struts, bugzilla, Redhat, CVS

# Work History

## 2/2008 -- Present: Software Engineer / *Cisco Systems (contractor)*

* Many projects over the years, most pertaining to the Cisco dot com (CDC) web site, some pertaining to the Cisco Employee Connection (CEC) internal web site:
* General Framework tasks
  * in-between the projects listed below, I was on various sprint teams in our larger ID team and pulled stories and defects related to general feature requests and defects
* NextGenWeb "backpack"
  * the backpack was a new component ("MyCisco") that spearheaded the personalization effort, it was a dropdown with a context-aware selection of modules that remembered the user's selections and choices and showed up on every page as part of the framework 
  * the backpack consumed and also posted back to a Java web service developed by a different team
  * because the service was not ready/was not yet reliable, I built a dummy service that honored the API so that I could write the backpack code and we could demo/discuss the backpack in cross-team meetings
  * coordinated with another team member who was crafting the css
  * we were added to the project in its final two sprints because the project leads discovered that somehow the backpack had been overlooked, and we managed to get a complex component completed and accepted by the project deadline
* Asset bundler and minimizer (js and css)
  * our team wanted to modularize the framework code for development, but have a way to assemble the modules into single asset files for production
  * I developed a perl module to read in a configuration file and concatenate files as per the config, then use the YUI compressor to minify the results
  * the bundler and its config were added to the framework CVS repo (and later git repo when we migrated) which allowed it to become part of the workflow
  * almost ten years later, it is still used for certain segments of the website 
* Homepage redesign (2008)
  * the homepage is an extremely mission critical project, code has to be as lean as possible and load as quickly as possible despite extensive complexity, and be pixel perfect and work cross browser -- including (at that time) IE6
  * worked on stripping down the framework code and css and minifying as separate bundles just for the homepage 
  * implemented the news ticker, a new component which consumed a feed from newsroom.cisco.com and rendered it realtime
  * also was the team lead on ensuring the vs/omniture metrics were all coded properly and delivering expected data to the metrics team
* Component Library
  * worked with third party 8Shapes to devise a nomenclature and component strategy
  * helped develop specs for the components and also implement some of them
  * wrote framework code to dynamically load component js and css based on page markup
  * many code reviews as offshore team inherited the next phases of CL development and maintenance
* CiscoIDTools
  * wrote a Firefox extension in XUL
  * it found and highlighted Cisco component library markup in the page
  * it also added menu item that showed the list of all component ids used in the page
  * rolling over a highlighted area popped up a modal with info about the component, including links to documentation and use cases
  * handed off to offshore team and helped manage updates and bug fixes by them
* SPoC for PCR (Product Category Redesign)
  * The main focus was a redesign of all the landing pages for product categories (Routers, Switches, Firewalls, etc.)
  * I volunteered to be the Single Point of Contact for this redesign -- all stakeholders communicated only with me, and any team questions were sent to me to track down with the stakeholders
  * this allowed all other team members to work heads down and undistracted, while I attended all the meetings and digested all the docs and emails
  * in order to maintain clarity, I wrote overview docs, MANY UE specs, and "speclets" and got signoff from the stakeholders and met with team members to review them
* Homepage redesign (2010)
  * worked with third party desing vendor 37signals via Basecamp
  * worked with the ID team to upgrade the UI and layout
  * scripted a process to package the current revision of the homepage project into a "DevKit" ("homepage in a box") to pass bewtween our team and the design vendor (37signals)
* Workspace/Portlets
  * entitled users could navigate from the MyCisco "backpack" to their Workspace page, which used a portal server (IBM WebSphere Portal) and had their personalization modules, implemented as portlets, in more detail
  * I worked on a UE redesign to layout the portlets better, offer switching between several views, and allow drag-and-drop
  * in addition this involved several meetings with the backend Java engineers regarding the web services 
  * this also entailed refactoring all the existing portlets to (at last!) behave properly
* Libra to Masterbrand migration
  * A huge project to migrate all pages from the "Libra" UE design to the "Masterbrand" UE design
  * at the time Cisco actually had three different web content platforms that were stitched together to show a seamless single website
  * this often meant templates, framework code, and data endpoints varied across the three platforms
  * thus changing UE simultaneously accross the production site involved the entire team doing meticulous development and testing
  * I was involved in the coding and template part of the migration
  * I also wrote a simulator webapp that could pull in any current production page and render it with the new framework code, for testing purposes
* Masterbrand 2.0
  * this was a UE design upgrade, as well as bugfixes from the initial migration -- mostly js and css work 
* Bluenote 
  * SHP (Support hompage) and Support MegaMenu optimaztion and UE upgrade
  * I wrote the CSS to spec and handed off to another team
* CEC migration from SJC
  * extensive project to move the intranet from a cluster of monolithic old Sun servers in San Jose to a distributed and load balanced architecture at data centers in Richardson and Allen, Texas
  * had to identify processes, files, cgi scripts, etc and update them to work in the new environment, which was not usually a one-to-one mapping
  * at the same time had to write the new version of the perl page framework templates and communicate with all consumers of the old templates to upgrade
  * this project was complex and allowed me to exercise a lot of my old sysadmin skills, as well as dust off my perl skills
* Ratings and Comments
  * a team member and I developed from scratch a Ratings and Comments component to utilize a web service newly created by another team
  * the service spec had several issues but was locked down, so we had to code around those
  * the initial standalone component was them made into a CQ/AEM page component
  * the AEM component has had a few iterations of feature updates
* Click to Chat
  * Many Cisco.com pages had existing "Click to Chat" buttons that were highly configured and connected to Liverperson agents who were on duty
  * Then the contract switched to Salesforce Liveagent with very little lead time to re-engineer the chat buttons to use the new service
  * The analysts on our team handed me a requirements doc and I coded up a "chat controller" that would go into the framework code on all pages
  * The code had to scan the page for chat button markup, if that was found, then determine the correct locale then pull in a JSON config file for button parameters based on the locale, pull in Salesforce code from their site, and wire up the button to poll the Salesforce API to determine if agents were online 
  * Almost all of the steps were asynchronous, so I got up to speed on Promises and fell in love with them
  * When the cutover from Liveagent to Liveperson occurred, the new code was ready and worked largely as expected
  * Since the initial deployment, several features have been added by me and other team members 
* DCBE / CCE
  * with a small tight team, developed an Angular2/MongoDB single page app that took the targeted user through a security analysis survey, scored the results, and suggested options for solutions tailored to the results
  * there was a lot of complicated behind-the-scenes logic and integration with other systems 
  * the app was then expanded so that it could serve up multiple surveys and be seamlessly embedded on partner's websites
  * the workflow included several virtual servers for dev, stage, and blue/green production using a nice CI pipeline that our DevOps team members built

## 5/2003 -- 1/2008: VP, Systems Engineering / *CollegeNET*

* In addition to managing the Systems group, I also started managing the Web Development group.
* After two years of managing both groups, I had rebuilt the Systems group into a much more effective and high-morale team. I decided I needed to focus on the Web Development group, and worked with the CEO to promote a senior SysAdmin to manage the IT staff.
* On a daily basis, I worked closely with Web Development to help them with ever-growing customer requirements. I could add features to the Forms Engine, to the forms markup language, and write tools that continue to streamline a very intensive workflow. The group was very involved in the requirements and spec design of these new features.
* This means on a daily basis I was designing and coding new features or enhancements to adapt the Forms Engine as needed, and released new code to production almost daily. Being able to support my team this way was very satisfying, especially when they were part of the process.

## 8/2000 -- 4/2003: Associate VP, Systems Engineering / *CollegeNET*
* Put together and managed a new team comprised of IT Services, Database Services, and senior engineers. 
* Introduced bug tracking company wide -- installed and configured bugzilla, advocated and educated others on it; required all requests for IT and Forms Engine be made via bugzilla; now it is indispensable to our development process
* Introduced wiki, IRC, and time management skills. Built an intranet server to host these services and build cross-team communication and effectiveness.
* Ongoing extensive design and coding on the Forms Engine.
* Initiated a massive cross-team effort to streamline the architecture; identified and refactored or rewrote much archaic code that was keeping us on old versions of the OS, etc.

## 11/1999 -- 7/2000: Chief Architect, Internet Engineering / *CollegeNET*
* Established new infrastructure standards to abstract web application code from direct database connections by introducing servlet middleware.
* Completely rebuilt the Forms Engine a third time to better incorporate new features, allow better and more flexible configuration across clusters, and to use the new middleware layer.
* Actively involved in research of new technologies, frameworks and architectures.
* Introduced CVS company-wide for software versioning -- set up the CVS server and migrated existing RCS files so that their versioning and comment history was preserved; trained and advocated others in how to use

## 9/1997 -- 10/1999: Senior Software Engineer / *CollegeNET*
* Early adopter of XML, rebuilt the Forms Engine from the ground up to use a markup language I designed for form descriptions.
* Added extensive data validation and a logic rules language to the Forms Engine.
* Researched, designed, built, tested, and deployed the webserver architecture still in use -- clustered mod_perl/Apache servers on the backend, and lightweight caching reverse proxies on the front end.
* As the Web Development group grew, increased support to aid their workflow via engine features, tools, internal CGIs, documentation and classes.

## 9/1996 -- 8/1997: Software Engineer / *CollegeNET*
* Met with other engineers to brainstorm and write specifications.
* Started a formal requirements capture process to improve specifications and include input from Sales and Marketing.
* Learned the product code from the inside out -- commenting, documenting, and testing the code as I progressed up the stack.
* Inherited the flagship ApplyWeb forms project when the lead senior engineer who wrote it left the company.
* Convinced the CEO to not terminate the ApplyWeb project until I had three months with it.
* Completely rewrote the ApplyWeb scripts into a Forms Engine.
* Started work on writing the patent specification for the Forms Engine.

## 8/1995 -- 8/1996: Network Manager / *CollegeNET*
* Rebuilt the corporate network as the company tripled in staff; included building out the new site, connecting the network to the internet via a bastion host firewall, and implementing NIS and NFS.
* Managed the conversion from a homegrown groupware to Lotus Notes, became Lotus Notes certified and managed the Notes infrastructure, including email.
* Migrated all Wintel boxes to Windows95 (to get them reliably on the network) and standardized equipment specs and purchasing procedures.
* Customer technical support
* Internal technical support -- always looking for ways to help colleagues, wrote many scripts to streamline Marketing and Administration tasks.

## 3/1995 -- 7/1995: Systems Engineer / *CollegeNET*
* Responsible for maintaining diverse Unix, VAX, and Wintel hosts.
* Internal technical support -- regularly interviewed staff to elicit requirements, discover frustrations. Then worked on designing and implementing solutions to those problems.
* Worked on the company's nascent website, www.collegenet.com -- configured and operated the web server, also wrote the site's first CGI scripts to transform flat static pages into user-interactive dynamic content, including a simple search engine of college stats.

## 8/1992 -- 2/1995: Technical Support/Network Administrator / *Electronic Technical Publishing*
* Designed, installed, and maintained network interconnecting Unix, Macintosh, and Windows systems.
* Installed and maintained software and hardware; performed incremental and full backups and recoveries.
* Supported users, trained new and established employees in Unix, TeX, and vi (wrote training materials and documentation, taught in-house classes).
* Wrote and maintained TeX, LaTex, and troff macro libraries.
* Coded and updated TeX source files.

# Education

Reed College, Portland, Oregon  
B.A. Biology, May 1989  
Thesis: Attempted Isolation of Two Arginine Catabolism Genes from the Pathogenic Yeast Candida albicans

Portland State University, Portland Oregon  
CS161 and CS162, Introduction to Computer Science (Fall 1993)  
CS163, Data Structures (Fall 2004)  
CS399J, Advanced Java Programming (Spring 2005)

# Interests

* Homebrewing beer and mead, and making fruit wine
* Gardening and making jellies, jams, and pickles
* Reading science fiction and history
* Keeping abreast of advances in science and technology
* Playing Settlers of Catan, Carcassonne, and Dominion with my sons and friends
* TV: Doctor Who, Dark Matter, Orphan Black, Foyle's War, Vice News

# Patents

* Universal Forms Engine, United States Patent 6,345,278 (filed 1999-06-03, issued 2002-02-05); International Patent WO9963454 (publication date 1999-12-09)
* Universal Forms Engine, United States Patent 6,460,042 (filed 2001-11-09, issued 2002-10-01; European Patent EP1522947 (publication date 2005-04-13)
* Method for paperless attachment of supplementary forms to a world wide web application, United States Patent 7,231,594 (filed 2000-02-09, issued 2007-06-12); International Patent WO0048087  (publication date 2000-08-17)

