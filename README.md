# A Software Development Life Cycle for Research Software Engineering
A toolkit for documentation and processes for software development in a research setting. 

This repository was established by [King's Digital Lab](https://www.kdl.kcl.ac.uk)  (KDL) on Aug 22 2018 and it is intended to be an evolving piece of work, enriched with community contributions.

The documentation found here represents the KDL's implementation of an Agile software development lifecycle, pragmatically adapted to suit the particular requirements and peculiarities of Research Software Development. 

## How to use this resource
*Document guidance and templates have been written in simple Markdown. They can be copied and pasted into most desktop word processing software or converted via a variety of third party tools into formats that can be easily used offline.*

### 1. Getting started
The core component of this toolkit is the [document templates](/sdlc-for-rse/document_template_index) that underpin the various stages of the SDLC.  In addition to the document templates, there are guidance documents which offer advice on how to populate the documents and what factors to consider when planning a RSE project.

Documents are prefixed alphabetically in expected order of use. The alphabetic character is followed by a number which will denotes whether the document is 1, a template or 2, an accompanying guidance document.

#### 1.1 Document templates
All branding and commercially sensitive information has been removed from the original KDL templates. The layout of the templates continues to evolve over several iterations and is geared towards achieving:

 - clarity of the project aims
 - clarity of the responsibilities of participating parties
 - a logical structure for peer review (internally)
 - the considered use of **boilerplate** text where applicable
 - transparency of the development process
 - direct reuse of text in funding applications

It is recommended that these completed templates be stored as project governance records in secure storage with access shared by the RSE team. Some of these documents are intended for internal audiences only, and these will be identified clearly with the header **"For internal use only"**

#### 1.2 Document guidance
Each document template has a [guidance document]()/sdlc-for-rse/document_guidance_index which explains the purpose of the document and offers useful direction for ensuring that the right information is gathered at the right time.

Each guidance document may contain one or more matrices of prompts and questions to help ensure productive meetings and minimise misunderstandings in the later stages of development. These prompts are not intended to be exhaustive and each research project will have complex and individual aspects, but it is hoped that these suggestions will stimulate productive communication.

Links within these documents may direct the user to:

 - RSE team role descriptions
 - SDLC process documentation
 - terms in a glossary
 - additional documentation

### 2. SDLC Stages and Processes
The SDLC can represented in a flow diagram thus:

<div class="mermaid">
graph LR
A[Square Rect] -- Link text --> B((Circle))
A --> C(Round Rect)
B - -> D{Rhombus}
C --> D
</div>

```mermaid 
graph TB
Pre["<b>Pre-project stage</b><br/><small><b>Products: </b> Terms of reference (Internal document)<br/><b>Goals: </b>Understand business case<br/><b>Roles: </b>Analyst, Project Manager, Director</small>"] --Go?--> 
Feas("<b>Feasibility</b><br/><small><b>Products: </b>Feasibility (Internal for peer review),<br/>High Level Cost --> Product Quote (if feasible)<br/><b>Goals: </b> Assess technical feasibility, clarify roles and responsibilities<br/> and make final GO/NO GO assessment.<br/><b>Roles: </b>Analyst, Project Manager, Developer, UI/UX, Systems Manager</small>")
Pre--No go?-->endPre[Do not proceed]
Feas--Feasible?-->Found("<b>Foundations</b><br/><small><b>Products: </b></small>")
Feas--Not feasible?-->endPre
Found-->Evo(Evolutionary development)
Evo-->Dep(Deployment)
Dep--Review-->Evo
Dep-->Post[Post project]




{% include js/js.md %}
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQwNjE5OTYzMywyMDc5MDU4NTk0LC0xOT
E5NDY0MTMzLC0xMTcyMDEyNjQ1LC0xMjE3MjU1NTk5LC0xNjU0
NzcxMDUzXX0=
-->