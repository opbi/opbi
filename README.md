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
#### Code of Conduct

- Open-Source and Business Agnostic
- Zero-Configuration By Default
- While Always Configurable
- Consistency over Variety
- Repeatable and Automatable


### Opinions

#### Technology Choices

OPBI will be sharing automation tooling based on common technology choices to create a well-integrated solution. We aim to use best-of-kind services while also would like to provide more flexibilities to support different options. As change of the fundamental technology options would largely impact the toolchain, we would like to keep the solutions more future proof by clear separation of layers and lock some of the choices initially.

Here we assume a list of choices as below [in different layers]:
- *Cloud Infrastructure*: [Google Cloud Platform](https://cloud.google.com/), [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/), [Terraform](https://www.terraform.io/)
- *Container Orchestration*: [Kubernetes](https://github.com/kubernetes/kubernetes), [Helm](https://github.com/helm/helm)
- *Continuous Integration*: [GitHub](https://github.com/), [CircleCI](circleci.com), [Coveralls](http://coveralls.io), [Snyk](http://snyk.io), [Hashicorp/Vault](https://github.com/hashicorp/vault), etc.
- *Build Toolchain*: Language specific best-practice build toolchain managed in centralised repos
  - JavaScript: [@opbi/ncm](github.com/opbi/ncm) - package an updated best-practices build toolchain for multiple repos
- *Services & Programming Languages*
  - JavaScript(Applications): React, React-Native, Node
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
