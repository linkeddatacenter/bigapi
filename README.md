![logo](http://linkeddata.center/resources/v4/logo/Logo-colori-trasp_oriz-640x220.png)

Perceive Its Beauty, Acknowledge Its Grace
==========================================

**BIGAPI** is an architectural design pattern and template designed for effective communication and documentation of software architectures. It addresses modern data-centered, cloud-native applications based on the best practices promoted by the W3C consortium. BIGAPI assists software development teams in describing and communicating software architecture during both initial design sessions and retrospective documentation of existing codebases. It facilitates the creation of "maps of your code" at various levels of detail, considering different points of view.

BIGAPI streamlines the process of documenting and communicating software architecture, making it more manageable and efficient. By leveraging proven practices and supporting a wide range of technologies and development methodologies, BIGAPI serves as a valuable tool for teams developing modern applications.


## Purpose
BIGAPI pragmatically answers two fundamental questions and can be tailored to meet specific needs:

- **What should you document/communicate about your architecture?**
- **How should you document/communicate it?**

## Key Features
- **Documentation structure:** Provides everything you need to construct, communicate, and document your software architecture, making the process practical and less burdensome.
- **Inspirations and Foundations:** Draws inspiration from the W3C architecture, ARC42 architectural template, and the C4 model, built upon practical experience from numerous systems across various domains.
- **Technology Agnostic:** Supports arbitrary technologies and tools, ensuring versatility across different projects and platforms.
- **Process-Agnostic:** Completely independent of specific processes, making it well-suited for lean and agile development approaches.
- **Open Source:** Available with  open-source license and free to use in non-commercial situations. Refer to our license page for more details.


## Philosophy Behind the Name
The name **BIGAPI** is a scrambled acronym for "**Perceive Its Beauty, Acknowledge Its Grace**": **B**eauty, **I**ts, **G**race, **A**cknowledge, **P**erceive, **I**ts.

The idea is to highlight how elegance and beauty can manifest in software architecture, much like patterns in nature. By creating systems with recognizable structures and balanced, lightweight components, aesthetic principles guide the design even before functional requirements. Graceful and well-proportioned architecture leads to software that is not only efficient but also intuitively understandable.

## Benefits

- **Enhanced Communication:** Offers a structured template for documenting and communicating software and system architectures, promoting better understanding among team members and stakeholders.

- **Flexible Detailing:** Allows the creation of architectural documentation at various levels of detail, accommodating different perspectives and requirements.

## Template
We provide you with the **BIGAPI template** for architectural documentation — a comprehensive index designed to simplify your documentation process. This template serves as a structured framework where you can seamlessly **fill in your architecture decisions**, capturing every critical aspect of your system's design. By using BIGAPI, the once daunting task of documenting your architecture becomes **simple, effective, and painless**, allowing you to focus more on developing robust solutions rather than getting bogged down by complex documentation procedures.

### Architectural documentation organization
The architectural documentation shoud be organized in 10 sections:
1) **Getting Started**: What do you need to know about the project
2) **Conformance**: Regulatory compliance and industry standards adopted by Argento.
3) **Glossary**: The main terms used in the project jargon
4) **Architecture**: The system big picture according different points of view
5) **Features**: The feature sheets that catalogues all the features implemented by the system
6) **Components**: TShe catalog of the technical components and configuration items that buildsup the project
7) **Stereotypes**: The source of truth for shared pieces of component documentation.
8) **Skills**: Competence required in  roles
9) **Roles**: Mission and skills required in the project operations
10) **Processes**: The ways to make things done

### Getting Started
Information in this section helps your user understand your project by themselves.

* What do your users need to do to start using your project? This could include downloading/installation instructions, including any prerequisites or system requirements.

* Introductory road map

Consider using the headings below for your getting started page. You can delete any that are not applicable to your project.:

```markdown
## What is <your project name>?
Please refer to:
- the [<your project name> web site]() 
- the [<your project name> value proposition]()

## What is the <your project name> architecture?
The <your project name> architecture is the foundational technology and environment on which the <your project name> applications run. It provides a base layer of processes, services, tools, and frameworks that allow developers to build, deploy, and manage applications. Essentially, **it is the design document of <your project name>**.

## What is it good for?
The <your project name> platform serves as an entry point for understanding the broader context of <your project name>. It is useful for:

- Understanding <your project name>'s  from different points of view
- Identifying the *skills* required for development and *management roles*
- Setting up the *development environment* and managing *day-to-day operations*.

## What is it not good for?
This is not a place to find detailed component documentation. 
About this, refer to the README files in the repositories in the [Component catalog]().

It is not a tool for business things.

## Where should I go next?
1) read the definition of some [terms]() used inside the <your project name> jargon
2) read the [standards]() to which <your project name> conforms
3) read the [architecture overview]()
4) self-assess your [skills]() 
5) find the [roles]() best match your competences
6) join a [process]()
```


### Conformance
This section covers the reference standards and normative guidelines that apply to your project.

For example:
```markdown
### Ethics
The <your project name> platform is designed for compliance with [EU AI  regulations](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) as minimal risk application. 

### Privacy
The <your project name> platform is designed for compliance with [GDPR privacy guidelines](https://gdpr.eu/), and cybersecurity best practices. This ensures that sensitive data is handled securely, and user privacy is protected. 

### W3C standards
The <your project name> platform conforms to the [W3C Web Architecture](https://www.w3.org/TR/webarch/) adopting the [Resource Description Framework (RDF)](https://www.w3.org/RDF/) for data representation and interoperability,  and [Solid specifications](https://github.com/solid/specification?tab=readme-ov-file)  to provide secure and decentralised data management.  

### Processes
<your project name> relies on  [DevOps](https://about.gitlab.com/topics/devops/) best practices. It  also considers [ITIL](https://www.ibm.com/topics/it-infrastructure-library) processes to create a long term corporate approach to IT service management.
```

### Glossary
This section defines the main temrs used in the architecture. For example:

```markdown
### Application
This term must be interpreted in multiple way in <your project name> platform:
- From development POV is a set of components that are seen by developers as a single product;
- From product management POV is  group of features that is made available to the customer with their functional requirements.
- From data semantic POV, an application profile  (also known as language profile) is a trimmed-down version or an extension of a set of recognized ontologies that trades some expressive power for the efficiency of reasoning.

### Architectural Element  
An architectural element is a sign (icon) for something referred in the <your project name> architecture (e.g. "component", "feature", "module", etc. etc.).

### Architecture
According to [KEES definition](https://linkeddatacenter.github.io/kees/#architecture-and-application):
- An architecture is the shared understanding that developers have about the design of the system. 
- The design decisions that must be made at the beginning of a project. 
- Architecture is about the important things. Whatever they are. 

### Artificial Intelligence  
A software program that is able to mimic the interaction with a human using its native language (i.e., a Turing test passing machine).

### Component
An architectural element representing a releasable software component. A component is modular, encapsulated unit of <your project name> system that performs a specific functions and may  concur to implement features. Components interact with each other through well-defined interfaces and can be independently developed, tested, and deployed. They are fundamental building blocks of the software architecture, enabling the system to be organized into manageable and reusable parts.  They are configuration items derived by the development process defined in a git repository.

### Explainable A.I.
A property of an AI algorithm to trace its result from the original input data. For example: *Neural Networks* and *Deep Learning* are not explainable (i.e., black box), *Logic Inference* is explainable.

### Feature  
An architectural element representing a distinct capability of <your project name> that delivers value to users or stakeholders. A feature can contain other feature in a tree structure (i.e a taxonomy) defined by a module

### Feature sheet
An architectural element representing a document that groups a set of related features.

### Functionality  
An architectural element representing an atomic testable feature. It cant' be composed by other features (i.e. it is a leaf in a feature taxonomy)

### Layer
a container of related technical module

### Machine Learning  
An algorithm that makes predictions based on examples, can be discriminative (e.g., classifier) or generative.

### Module
An architectural element representing a logical group of _feature sheets_.

### Platform  
The foundational framework that supports the requirements, development, deployment, and execution of software applications.

```

### Architecture
The architecture is a composition of  three different perspectives providing a common understanding to different point of view of the product:
- Business analyst looks to the **functional view**
- Data engineer looks to the **data view**
- Developer looks to the **component  view**

Ath the home of the architecture you can add a system view using [C4 model diagrams](https://c4model.com/). For picture consider using a textual based tool like PlantUML or mermaid. For example (with plantUML)

```plantuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Container.puml

Person(user, "User", "An user")
System(system, "your System", ) 
System(solid, "SOLID POD", "personal data storage and authentication")
System(billing, "Billing system", "accounting")

Rel(user, system, "Uses", )
Rel(system, solid, "HTTPS", "SOLID OIDC, LDP")
Rel(system, billing, "HTTPS", "accounting info")
```
#### Functional view
The functional view looks at the your project with the user eyes; it define the features realized by the components designed in the technical view grounding by the data semantic defined in the data view.

The functional view of your project  consists in a hierarchies of modulese, feature sheets, features and functionalities. A module is a composition of feature sheets that is a document that describe a set of related features. Features can depends from other features; the features with no dependencies are called functionalities.


```plantuml
folder "Modules" as Module
file "Feature Sheets" as FeatureSheet
collections "Features" as Feature
card "Functionalities" as Functionality
Module *-- FeatureSheet
FeatureSheet *-- Feature
Feature ..> Feature
Feature <|-- Functionality
```

You should also define  your feature life cycle according ITIL best practices.


#### Technical view
The technical view looks at the interaction of physical components that build your system. The components realize the features defined in the functional view by recognizing the data semantic defined in the data view.

In this section you should address:
- the application focus
- principles (e.g. Twelve-Factor Application)
- Layer breakdown
- Style guides and naming conventions


You can use the C4 component diagrams or UML


#### Data view
The data view captures the semantic behind your application; it demonstrates the feasibility of the features defined in the functional view allowing the design of in the technical components.

In this section you should address:
- the application focus
- principles (e.g. Privacy by Design, KEES compliance, Data-Driven architecture)
- the data model abstraction (e.g. wuth UML class diagrams)
- The data representation (e.g., RDF, openApi, AsyncAPI)
- Style guides and naming conventions


### Features
This section contains or refers to the catalog of all the project features.


### Components
This section refers to the repositories where technical component resides. Each technical componet should be rdeveloped inside its own repository. 
Its documentation is written in its README file and by reference one or more stereotype


### Stereotypes
The objective of the  stereotypes is to avoid duplication in technical component documentation; you can think a stereotype as a _README include_

A stereotype should be immutable, it must not be deleted if there is at least an active component that refer it.


### Skills
A skill is the ability to perform a task with proficiency and expertise through knowledge and practice. Skills are required to play a role in your project development.


### Roles
In your project organization some role should be defined. A people can play more than a role. Each role should be granted by a mission and some required skills.


### Processes
Here is where you document process and task in your project. For example:
- **Agile development**: Process to develop and release product
- **Service management**: Management of the runtime Argento service
- **Dev workstation**: Setup of a developer workstation
- **Dev workstation**: Setup of a tester workstation


## License
BIGAPI is a research project by [LinkedData.Center](https://linkeddata.center) it is released open-source and can be used free of charge, for non-commercial and private situations. See our [license](LICENSE) page for details.


## Contributing to this site
A great way to contribute to the site is to create an [issue](https://github.com/linkeddatacenter/bigapi/issues) on GitHub when you encounter a problem or something. We always appreciate it. You can also edit the code by yourself and create a pull request.

