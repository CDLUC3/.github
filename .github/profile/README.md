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
- Work is prioritized through the Product Manager as part of our development process

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

## Testing & Quality

- Automated tests are expected where feasible
- Changes should be validated before merging
- Accessibility and performance should be considered as part of development

## Deployment & Releases

### General Guidelines
- Keep releases small and incremental
- Avoid deployments late in the day, on Fridays, or before holidays
- Monitor systems after deployment
- Communicate releases to relevant stakeholders

