# Wallarm

Wallarm provides advanced API security and protection solutions for APIs, web applications, and microservices. The platform includes API discovery, real-time attack protection, vulnerability testing, and an open-source API Firewall that enforces OpenAPI specifications as a positive security model. Wallarm supports deployment on Kubernetes, cloud environments, and as an NGINX-based proxy.

- **Website:** [https://www.wallarm.com/](https://www.wallarm.com/)
- **Documentation:** [https://docs.wallarm.com/](https://docs.wallarm.com/)
- **API Reference:** [https://docs.wallarm.com/api/overview/](https://docs.wallarm.com/api/overview/)
- **GitHub:** [https://github.com/wallarm](https://github.com/wallarm)

## APIs

### Wallarm API

Programmatic access to the Wallarm API Security Platform for managing attacks, vulnerabilities, security rules, IP lists, filter nodes, users, integrations, and triggers.

- **Base URL:** `https://us1.api.wallarm.com` (US Cloud), `https://api.wallarm.com` (EU Cloud)
- **Authentication:** API Token (`X-WallarmApi-Token` header)
- **Console:** [US Cloud](https://apiconsole.us1.wallarm.com/) | [EU Cloud](https://apiconsole.eu1.wallarm.com/)

## Artifacts

### OpenAPI Specifications

| Spec | Description |
|------|-------------|
| [wallarm-openapi.yml](openapi/wallarm-openapi.yml) | Wallarm API — attacks, vulnerabilities, rules, IP lists, nodes, integrations, triggers |

### Spectral Rules

| Ruleset | Description |
|---------|-------------|
| [wallarm-rules.yml](rules/wallarm-rules.yml) | Spectral ruleset enforcing Wallarm API conventions |

### Naftiko Capabilities

#### Shared Per-API Definitions

| File | Description |
|------|-------------|
| [capabilities/shared/wallarm-api.yaml](capabilities/shared/wallarm-api.yaml) | Wallarm API consumed definition |

#### Workflow Capabilities

| Workflow | Description | Tools |
|----------|-------------|-------|
| [api-security-operations.yaml](capabilities/api-security-operations.yaml) | Unified API security monitoring, attack response, vulnerability management, IP list management | 10 tools |

### JSON Schemas

| Schema | Description |
|--------|-------------|
| [wallarm-attack-schema.json](json-schema/wallarm-attack-schema.json) | Schema for Wallarm attack objects |
| [wallarm-vulnerability-schema.json](json-schema/wallarm-vulnerability-schema.json) | Schema for Wallarm vulnerability objects |

### JSON Structures

| Structure | Description |
|-----------|-------------|
| [wallarm-attack-structure.json](json-structure/wallarm-attack-structure.json) | Attack data structure documentation |

### JSON-LD Contexts

| Context | Description |
|---------|-------------|
| [wallarm-context.jsonld](json-ld/wallarm-context.jsonld) | JSON-LD context for Wallarm security entities |

### Examples

| Example | Description |
|---------|-------------|
| [wallarm-listAttacks-example.json](examples/wallarm-listAttacks-example.json) | List attacks request/response example |
| [wallarm-listVulnerabilities-example.json](examples/wallarm-listVulnerabilities-example.json) | List vulnerabilities request/response example |
| [wallarm-addIpRule-example.json](examples/wallarm-addIpRule-example.json) | Add IP denylist rule request/response example |

### Vocabulary

| File | Description |
|------|-------------|
| [wallarm-vocabulary.yml](vocabulary/wallarm-vocabulary.yml) | Wallarm API security vocabulary and taxonomy |

## SDKs and Tools

- **Go SDK:** [github.com/wallarm/wallarm-go](https://github.com/wallarm/wallarm-go)
- **Terraform Provider:** [github.com/wallarm/terraform-provider-wallarm](https://github.com/wallarm/terraform-provider-wallarm)
- **Terraform AWS Module:** [github.com/wallarm/terraform-aws-wallarm](https://github.com/wallarm/terraform-aws-wallarm)
- **Kubernetes Ingress:** [github.com/wallarm/ingress](https://github.com/wallarm/ingress)
- **Helm Charts:** [github.com/wallarm/helm-charts](https://github.com/wallarm/helm-charts)
- **API Firewall:** [github.com/wallarm/api-firewall](https://github.com/wallarm/api-firewall)
- **GoTestWAF:** [github.com/wallarm/gotestwaf](https://github.com/wallarm/gotestwaf)

## Maintainers

**Kin Lane** — [kin@apievangelist.com](mailto:kin@apievangelist.com)
