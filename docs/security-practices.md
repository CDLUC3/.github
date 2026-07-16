# UC3 Software Security and Vulnerability Management Practices

UC3 maintains the security of its services through a structured vulnerability management process that combines automated patching, regular reviews, and lifecycle management of third-party software.

UC3 employs a risk-based vulnerability management program that combines automated monthly operating system patching with recurring reviews of third-party software, application dependencies, and cloud infrastructure. We maintain an inventory of deployed software versions, monitor security advisories and end-of-life notices, review dependency health for each application, and use automated security scanning to identify vulnerabilities across EC2 instances and containers. Findings are tracked to resolution through our engineering workflow, with critical vulnerabilities prioritized for expedited remediation while routine updates are addressed during scheduled maintenance cycles.

**Key practices include:**

## Monthly operating system patching
- Linux (Amazon Linux) packages installed through the distribution repositories are updated as part of a recurring monthly operating system patch cycle.
- Standard operating system packages are automatically maintained through the distribution package manager (dnf).
## Comprehensive third-party software inventory
- UC3 maintains an inventory of third-party software deployed across its services, including:
  - operating system packages
  - language-specific packages (Ruby gems, npm, pip, Maven)
  - Docker images
  - tarball installations
- For each component, the team tracks:
  - deployed version
  - latest available release
  - end-of-life date
  - last update date
  - security advisory sources
  - release notification sources
  - upgrade notes
## Regular vulnerability reviews
- Software dependencies and infrastructure components are reviewed on a monthly basis to identify:
  - newly released versions
  - known security vulnerabilities
  - approaching end-of-life software
  - opportunities for planned upgrades.
## Application dependency management
- Each UC3 application maintains dependency manifests appropriate to its technology stack.
- Development teams periodically review these dependencies to ensure:
  - no known security vulnerabilities remain
  - dependencies remain reasonably current rather than falling behind supported versions.
## Security scanning and findings management
- UC3 reviews results from AWS IAS SecUnit security scans covering:
  - EC2 instances
  - containers
  - BitSight notifications
    
Findings are assigned to responsible service teams, tracked, acknowledged, and given revisit dates until remediation is complete.
## Monthly infrastructure health reviews
- AWS HouseKeeper reports are reviewed each month, with findings distributed to the appropriate service teams for remediation.
## Planned modernization and lifecycle management
- Rather than only reacting to vulnerabilities, UC3 proactively tracks software lifecycle information, including end-of-life dates and major version upgrades.
- Modernization work (for example, framework migrations or major platform upgrades) is planned and tracked to reduce long-term security and maintenance risk.
