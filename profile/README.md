## Welcome to UC3's Product Development Space 👋

🙋‍♀️ The University of California Curation Center (UC3) helps researchers and the UC libraries manage, preserve, and provide access to their important digital assets.


# UC3 Development Practices

This page outlines shared development practices across UC3 repositories. These guidelines establish a consistent baseline for how we build, review, deploy, and operate our services.

For broader context, see our [UC3 Product Development Approach](https://uc3.cdlib.org/our-work/uc3-product-development-approach/).

---

## Development Workflow

### Work Tracking
- All work must be tracked in GitHub issues
- Issues should include:
  - Clear description
  - Acceptance criteria
  - Relevant context and dependencies
- Work is prioritized through the Product Manager

### Branching & Pull Requests
- All changes must be submitted via pull request
- PRs require at least one review before merging
- PRs should include:
  - Summary of changes
  - Testing instructions
  - Related issue(s)

### Code Review
- Reviews should validate:
  - Functionality
  - Code quality
  - Security considerations
- Feedback should be clear, constructive, and actionable

---

## Testing & Quality

- Automated tests are expected where feasible
- Changes should be validated before merging
- Accessibility and performance should be considered as part of development

---

## Deployment & Releases

### General Guidelines
- Keep releases small and incremental
- Avoid deployments late in the day, on Fridays, or before holidays
- Monitor systems after deployment
- Communicate releases to relevant stakeholders

### Release Template

Use the standard release template: https://github.com/CDLUC3/.github/blob/main/ISSUE_TEMPLATE/release.md

---

## Infrastructure & DevOps

* Infrastructure should be managed as code wherever possible
* Services should include:
  * Logging
  * Monitoring
  * Alerting
* Use shared AWS patterns and tooling when available

---

## ECS Migration Guidance

When migrating EC2-based services to ECS:

### Architecture

* Containerize applications and reduce host dependencies
* Design for stateless services where possible

### Configuration & Secrets

* Externalize configuration using environment variables
* Store secrets in AWS SSM or Secrets Manager

### Storage

* Use managed services for persistence (S3, RDS, EFS)
* Avoid reliance on local disk

### CI/CD

* Build and deploy container images through pipelines
* Use versioned image tags

### Monitoring & Logging

* Ensure centralized logging (CloudWatch, OpenSearch)
* Monitor service and container health

### Deployment & Rollback

* Use rolling or blue/green deployments where possible
* Ensure rollback via previous task definitions

### Cost Awareness

* Monitor utilization and right-size services
* Evaluate ECS vs EC2 tradeoffs

---

## Shared Responsibility

* At least two developers should be familiar with each service
* Document architecture and operational processes
* Raise blockers and risks early
* Share knowledge across teams

---

## Related Resources

* [UC3 Product Development Approach](https://uc3.cdlib.org/our-work/uc3-product-development-approach/)




