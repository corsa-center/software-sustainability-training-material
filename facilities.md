# Working with facilities

## Questions asked to US computing facilities

We're trying to outline and develop some material for open source software projects as part of [CORSA](https\://corsa.center/) / [CASS](https\://cass.community/).

Currently, we're working with DOE-funded projects, most of which were part of ECP.

We're wondering what we should say about how these projects could work with facilities, such as computing facilities.

We're thinking that they might want to consider things like: How do I get my software mentioned in the facility's docs? How do I get my software installed on the facility's systems? How do I get the facility to talk about my software when they have users who could benefit from it? How do I coordinate support for people who have problems with my software on the facility's system?

Maybe not all of these are reasonable, and maybe there are other questions that would be more reasonable.

What do you think?

Do you have any advice on what we should be telling the projects about this in general, and about \[FACILITY\] specifically?  Is there a part of your website that helps?  Are there any \[FACILITY\] talks that include anything about this?

## Answers

The answers that follow are anonymized. Updates from these facilities or additions from others are welcome.

### Answer from ALCF

I think the best way to frame this is to say that facilities exist to serve their users' needs.  To have the facility provide support for a software package as you describe, there needs to be a demonstrated need from multiple facility users.  So my advice to these projects would be to develop a user community that includes users of the facilities you are targeting.  I think for developers to come to a facility without use cases or users would be unlikely to be fruitful.

At ALCF, we are traditionally focused on large scale capability computing (although we may see some evolution in this requirement from DOE with the Genesis mission).  About 60 per cent of the time on ALCF systems are allocated to projects that demonstrate a need for 20 per cent (or more) of our systems for compute jobs.  So the libraries, software, and tools we as a facility focus on are for these users who have to meet this requirement as part of the technical assessment of their proposals.

### Answer from OLCF

Happy to help. Your four questions are all reasonable and map well to how projects actually engage facilities. I'd frame them roughly in this order of effort:

1. Get installed on the system: At OLCF that usually means working with the User Assistance / software team to get it into the software stack (module or container), or providing a clean install recipe (Spack helps a lot here).
2. Get into the facility docs: Once it's installed and supported, documentation is the next step. See the workflows example for the level of detail that works well: https\://docs.olcf.ornl.gov/software/workflows/index.html\#workflow-systems
3. Support coordination: Define who owns what. Facilities handle first-tier user contact, but they need a clear escalation path back to the project team. Agreeing on this up front is what makes a facility comfortable recommending your software. For example, for each workflow system we have a direct line to someone in their development team.
4. Facility promotion: This tends to come last and follows naturally from the first three. Facilities point users to software they've installed, documented, and can support. It's less about asking them to promote you and more about being an easy thing to recommend.

The through-line for all of these: facilities champion software that reduces their support burden and demonstrably helps their users. Reliable installs, good docs, and a responsive project team are what earn the mentions.

On resources: the OLCF docs site is the main lever, and the workflows page above is a good model. I'm not aware of any OLCF talks that cover this topic specifically.

### Answer from NERSC

How do I get my software mentioned in the facility's docs?   
  * Our docs source is publicly available and we allow users to add MRs which can be reviewed by staff and added to the docs. One issue we face is having software on the docs that we don’t have staff to support. At least one of our sections in the docs, our workflow tools, does have a section we call “Community Supported Tools” these would be tools verified by the author or community work at NERSC but we can’t offer full support and we may rely on the developers to keep the software working at NERSC.  

How do I get my software installed on the facility's systems?   
  * Usually software is installed on a per user or project basis. We have docs on some best practices for installing and sharing software. So in general we would expect someone who wants to share software to place it in a location that is accessible and create their own module file to share it. If there is a large user base for a particular software library it’s probably best to open a ticket for our staff to understand the user base and how we may be able to help support the software.  

How do I get the facility to talk about my software when they have users who could benefit from it?   
  * For staff directly talking about a software tool this would probably be more of a training event. Our NERSC User Group (NUG) community calls are a good place to allow users to present on their work and would probably be a good place to present on it. We also have our NERSC User Slack space which can be a good place to communicate on different software tools.   

How do I coordinate support for people who have problems with my software on the facility's system?  
  * Our NERSC User Slack can be a good place to coordinate on issues specific to running software at NERSC. While some staff may be there and could help, our general strategy is to have users open tickets for specific issues. In our ticketing system users can add others onto a ticket, even non-nersc users, as the ticketing system works with emails. So we can work with the NERSC user and software developer to understand the issue and work to try and find a solution.


Some general tips about working at NERSC:

* Our docs are a great first place to start with many questions, and a good resource to point people to who want to use NERSC.  
* The NERSC User Slack can be a great place to collaborate with other NERSC users and get help from others who use NERSC.  
* For system level issues or specific questions, our ticketing system can direct you to the right member of staff to get questions answered and support if there are issues with the systems.

### Answer from ACCESS

How do I get my software mentioned in the facility's docs?
  * ACCESS only mentions software already installed on integrated systems/resources  
  * Researchers can discover installed software using https\://sds.access-ci.org/, or the Q\&A chatbot  
    
How do I get my software installed on the facility's systems?
  * Convince the resource providers to install the software on their resource  
  * Request that the resource provider create a community software area on their resource, where the software provider can install and maintain their software  
  * In both of these cases, the software provider needs to make a case that there is researcher interest in having the software pre-installed  
    
How do I get the facility to talk about my software when they have users who could benefit from it?
  * Primarily by getting the software installed on systems/resources  
    
How do I coordinate support for people who have problems with my software on the facility's system?  
  * If the software provider convinced the resource provider to install the software, support will happen through standard ACCESS channels via the resource provider  
  * If the software was installed in a community software area, the support mechanism is registered along with the software  
    
How ACCESS supports software developers  
  * Once a developer has gotten their software on at least one ACCESS resource, the ACCESS Software Documentation Service ([https\://sds.access-ci.org/](https://sds.access-ci.org/)) contains researcher-facing documentation that the software developer can help us develop/improve. We help developers by publishing this federation-wide documentation that will be found by researchers across all resources that have their software.  
  * The ability to create Community Software Areas is an ACCESS ability operationalized by the resource provider. It provides developers a common approach to installing their software on resource provider resources in a way designed to share with other researchers on those resources.
