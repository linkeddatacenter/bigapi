## Glossary
This section defines the main terms used in the architecture. 


For example:

	This project conforms to the [IT Service Management Ontology v2](https://w3id.org/itsmo) and to [schema.org](https://schema.org/) vocabularies, mainly for terms derived from [GoodRelation](https://www.heppnetz.de/ontologies/goodrelations/v1.html#classes). Beside those, some specific terms are used:

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

