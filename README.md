<p align="center">
  <img alt="ncm" src="https://raw.githubusercontent.com/opbi/logo/master/opbi/opbi.svg?sanitize=true" width="160">
</p>

<h3 align="center">OPBI - Open Business Institute</h3>
<p align="center" style="margin-bottom: 2em;">opinionated business agnostic open source solutions</p>

---

### Missions

#### Sharing Best Practices
With the power brought by the open-source community and Sass tools, it is much easier to curate an idea into a business than 2008. OPBI is founded with a mission to share the common technology decisions validated as best practices so that entrepreneurs can better focus on explore business logics. It is initialised with solution patterns found in various companies in different scales, and it is always more forward-looking to fix problems perceived in those organisations. It would stay open-source, so that it can be kept updated to set the technology structure models.

#### Reusable and Integrated Solutions
It often comes down to choose tools and services, integrate them with automations and process to achieve efficiency and technology-organisation fit. Common decisions on infrastructure, development process, pipeline, release pattern, data tracking and analytics can firstly be shared, discussed, updated. Secondly, architect and certain services can be made reusable as well, e.g. an image upload service, payment-accounting integration, etc. OPBI will be sharing here a list of technology choices and automations to integrate them into one system with a fitting organisation structure.


### Principles
```
"Those who want to do their job well must first sharpen their tools." -- Ban Lu
```

#### Open-Source and Business Agnostic
#### Zero-Configuration By Default
#### While Always Configurable
#### Consistency over Variety
#### Repeatable and Automatable


### Practices

#### Technology Choices

OPBI will be sharing automation tooling based on common technology choices to create a well-integrated solution. We aim to use best-of-kind services while also would like to provide more flexibilities to support different options. As change of the fundamental technology options would largely impact the toolchain, we would like to keep the solutions more future proof by clear separation of layers and lock some of the choices initially.

Here we assume a list of choices as below [in different layers]:
- *Cloud Infrastructure*: [Google Cloud Platform](https://cloud.google.com/), [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/), [Terraform](https://www.terraform.io/)
- *Container Orchestration*: [Kubernetes](https://github.com/kubernetes/kubernetes), [Helm](https://github.com/helm/helm)
- *Continuous Integration*: [GitLab](https://gitlab.com), [GitHub](https://github.com/), [CircleCI](circleci.com), [Coveralls](http://coveralls.io), [Snyk](http://snyk.io), [Hashicorp/Vault](https://github.com/hashicorp/vault), etc.
- *Build Toolchain*: Language specific best-practice build toolchain managed in centralised repos
  - JavaScript: [@opbi/ncm](github.com/opbi/ncm) - package an updated best-practices build toolchain for multiple repos
- *Services & Programming Languages*
  - JavaScript(Applications): React, React-Native, Node, Fastify
  - Python(Data Services)
  - Golang(DevOps Services)
- *Operation*:
  - @opbi/toolbox: Packaged Log, Metrics, Tracing Decorator
  - Prometheus, Grafana, ELK, etc.
- *Behaviour Analytics*: Segment
- *Marketing Automation*
- *Business Intelligence*

#### Organisation Structure

<p align="center">
  <img alt="ncm" src="https://raw.githubusercontent.com/opbi/graffle/master/organisation-structure.png">
</p>

#### Technology Architecture

<p align="center">
  <img alt="ncm" src="https://raw.githubusercontent.com/opbi/graffle/master/architecture-graph.png">
</p>

#### Component Lifecycle Standard

<p align="center">
  <img alt="component" src="https://raw.githubusercontent.com/opbi/graffle/master/component-lifecycle.png">
</p>

#### Service Lifecycle Standard

<p align="center">
  <img alt="service" src="https://raw.githubusercontent.com/opbi/graffle/master/service-lifecycle.png">
</p>

#### Application Lifecycle Standard

<p align="center">
  <img alt="app" src="https://raw.githubusercontent.com/opbi/graffle/master/app-lifecycle.png">
</p>

#### Glossary

We choose to use a set of distinctive and friendly terms to describe high-level elements in organisation structure and technology architecture. These terms are chosen to avoid confusion with any lower-level elements in technology and organisation while ideally integrate them, e.g. `package` is used in Node.js to describe codebase unit. Those terms will essentially be used to form the schema of the technology resource management system.

[Product] <- [User Journeys, Business Capabilities] <- [Team(Squad)]

[System] <- [Component] -> [Team(Tribe)]

[Organisation] <- [Team] <- [People]

- System: the operating architecture constructed with components, which serves a set of user journeys or business capabilities managed by different business slice teams [Squads]
- Component: a codebase unit that can be developed, ran or deployed or published or used to config infrastructure. It be in one of the types [infra, data store, app, service, job, package], and for each type there should be a template to define its quality and workflow standard, to model how it would be planned, developed, tested, deployed, shared, used, monitored, and administrated.
- Team: can be a skill based community [Tribe] or a business capability slice group [Squad]. Each Tribe should have a common standard of distinctive responsibilities and technology choices, e.g. commonly can be product, data engineering, devops Tribes. Each Squad should have a set of key metrics to define their missions, a product Squad should take the first touch point of a particular set of user journeys to its very end, and how they would be formed would be aligned to the Product User Experience Architect.
- User Journey: user-product interaction path to complete certain tasks in order to fulfil users' requirement from time to time as well as the organisation's mission. A selected set of journeys are arranged to form the product according to Product User Experience Architect based on priorities. There should be one single source of truth of those journeys to thread user research, design, user stories planning, development, test, product release and performance monitor, aligning to business missions.
