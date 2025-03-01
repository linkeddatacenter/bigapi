## Typographic conventions
This section defines legends and typographic convention in diagrams. 
For example:


	### Agents
	[Agents](https://w3id.org/itsmo/Agent) are represented using UML actors notation as in use cases.

	The <<Bot>> agents may be represented as dashed actor or with the `<<Bot>>` stereotype.
	```plantuml
	actor bot #line.dashed
	actor bot <<Bot>> as b1
	```


	### Features 
	_Features_ can be represented in UML use cases, are packaged in feature sheets and are composed in a taxonomy where the leaf nodes are called  functionalities. _Functionalities_ can be represented with a check sign (☑) or  with the `<<Functionality>>` stereotype.

	```plantuml
	package "feature sheet X" <<Module>>  {
		usecase "feature 1" as UC1  
		usecase "feature 2" as UC2
		usecase "functionality 1" as F1.1 <<☑>>
		usecase "functionality 2" as F1.2 <<☑>>
		usecase "functionality 3" as F2.1 <<functionality>>

		UC1 *-- F1.1
		UC1 *-- F1.2
		UC2 *-- F2.1
	}
	```


	### Context diagrams
	The [System Context Diagram](https://c4model.com/diagrams/system-context) notation from the  C4 Model is used

	![C1 example](https://static.structurizr.com/workspace/76748/diagrams/SystemContext.png)


	### Container diagrams as deploy diagrams
	The UML _deployment diagram_ in cloud native application context is similar to the _Container diagram_ in the C4 model container. The UML _deployment diagram_ is to be preferred because it allows more freedom degree in describing how [System components](https://w3id.org/itsmo/SystemComponent) interacts, for example you can say that a components is a customization of a standard component. 

	System components are represented as nodes in a UML deploy diagram and they may conform to one or more _stereotypes_. Each stereotype may also be indicated with an Icon on a node image.
	a  line represents a logic dependency relation as in the C4 container diagram semantic. 


	Nodes in this abstraction are treated as logical execution units (not just physical machines)

	```plantuml
	skinparam Rectangle {
		BorderStyle Dashed
	}
	node "system component 2" as n2 <<API>>
	actor client
	rectangle "System A" {
		node "system component 1" as n1 <<MsgProducer>>
		node "custom component" as n2custom <<API>>
	}

	client - n2custom
	n2custom -> n1 : calls
	n2 <|-- n2custom
	```



	### Relations
	The following UML relation types are supported in diagrams:
	```plantuml
	(A) -( (B) : attaches to interface
	(A) -> (B) : dependency relation / structural dependency / generic relation
	(A) -|> (B) : specializes / it is a fork of / derived from
	(A) - (B) : generic association ?link
	(A) *- (B) : composed by
	(A) o- (B) : aggregates
	(A) .|> (B) : implement/ run time dependency
	```

	The exact meaning depends from the scope of the diagram.


	### Conventional notation for requirements
	Requirements are expressed with a combination of descriptive assertions and [RFC 2119](https://tools.ietf.org/html/rfc2119) terminology. The key words **MUST**, **MUST NOT**, **REQUIRED**, **SHALL**, **SHALL NOT**, **SHOULD**, **SHOULD NOT**, **RECOMMENDED**, **MAY**, and **OPTIONAL** in the normative parts of this document are to be interpreted as described in RFC 2119.  However, for readability, these words may not always appear in uppercase letters in this specification.

