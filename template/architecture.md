
## Architecture
The architecture is a composition of  three different perspectives providing a common understanding to different point of view of the product:
- Business analysts look to the **functional view**
- Data engineers look to the **data view**
- Developers look to the **component  view**

As overview  of the architecture section you should add a system context view using the [C4 model diagrams](https://c4model.com/). For diagrams,  consider using a textual based tool like PlantUML or mermaid. For example (with plantUML)

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


### Functional view
The functional view looks at your project with the user eyes; it defines the features realized by the components designed in the technical view grounding by the data semantic defined in the data view.

The functional view  consists in a hierarchies of modulese, feature sheets, features and functionalities. A module is a composition of feature sheets that is a document that describe a set of related features. Features can depends from other features; the features with no dependencies are called functionalities.

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

You should also define  your feature life cycle, for example according ITIL best practices.


### Technical view
The technical view looks at the interaction of physical components that build your system. The components realize the features defined in the functional view by recognizing the data semantic defined in the data view.

In this section you should address:
- the application focus
- principles (e.g. Twelve-Factor Application)
- Layer breakdown
- Style guides and naming conventions

You can use the C4 component diagrams or UML


### Data view
The data view captures the semantic behind your application; it demonstrates the feasibility of the features defined in the functional view allowing the design of in the technical components.

In this section you should address:
- the application focus
- principles (e.g. Privacy by Design, KEES compliance, Data-Driven architecture)
- the data model abstraction (e.g. wuth UML class diagrams)
- The data representation (e.g., RDF, openApi, AsyncAPI)
- Style guides and naming conventions
