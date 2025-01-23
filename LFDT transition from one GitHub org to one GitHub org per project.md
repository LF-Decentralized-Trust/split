# LFDT transition from one GitHub org to one GitHub org per project

Historically, LFDT has had two active orgs; one for the main projects, and one for labs. With the introduction of CLOWarden, and being approved for an Open Source enterprise plan, staff is working with project maintainers to transition to one org per project, as well as an org for labs.

Why do this? Cost management, governance, and security.

* The primary challenge is the inability to manage costs on a per-project basis, particularly when using GitHub Actions and large runners. This has led to budget overruns affecting all projects.
  * New GitHub Enterprise features, introduced last year, provide improved mechanisms for cost control.
* Previously, repositories within the Hyperledger organization were readable by anyone with access to the organization, even if they should have been restricted. 
* Distinct orgs allow us to address [east-west](https://en.wikipedia.org/wiki/East-west_traffic) security concerns, where a security incident in one org does not instantly compromise all projects.

Transition to Independent Organizations

* There is a strategic move to transition projects into their own GitHub organizations to provide better governance, cost control, and project independence. This change is part of an overarching plan to phase out the centralized Hyperledger GitHub organization.
* The expected timeline for this transition spans the first half of the year, with a final deadline potentially extending to the end of the following year.

Project-Specific Challenges

* Firefly, along with other projects like Fabric and Indy, faces significant administrative and engineering challenges during this transition, including renaming repositories, managing workflows, and ensuring seamless integration with existing clients and infrastructure.
* Pushback from maintainers was noted, particularly around the effort required to adapt to the new organizational structure and naming conventions.

Benefits to projects

* Projects will have better stats in LFX Insights, as each org will be one project
* Delegation of repo creation to the project maintainers

Action Items and Next Steps

1. Documentation: Formal documentation of the transition requirements and benefits will be created and submitted to the LFDT Technical Advisory Council (TAC) for discussion and formal acknowledgment.
1. Maintainer Discussions: Project maintainers will review the proposed organizational changes, their benefits, and their impacts on governance and cost management.
1. Technical Adjustments: Efforts will be made to streamline workflows, test repository changes, and explore options for cost optimization, such as using AWS runners.
