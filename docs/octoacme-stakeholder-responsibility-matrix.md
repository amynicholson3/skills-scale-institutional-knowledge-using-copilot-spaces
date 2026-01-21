# OctoAcme Stakeholder Responsibility Matrix

## Purpose
Define clear accountability across project roles to minimize gaps and duplication of effort. This matrix uses the RACI model: Responsible (does the work), Accountable (owns the outcome), Consulted (provides input), Informed (kept updated).

---

## Project Lifecycle Activities

| Activity | Project Manager | Product Manager | Developer | Business Analyst | QA Lead | Change Manager | Release Coordinator |
|----------|----------------|-----------------|-----------|------------------|---------|----------------|---------------------|
| **Initiation Phase** |
| Define problem statement | C | A/R | I | C | I | I | I |
| Identify stakeholders | A/R | C | I | C | I | I | I |
| Create project charter | A/R | R | I | C | I | I | I |
| Initial risk assessment | A/R | C | C | I | I | C | I |
| **Planning Phase** |
| Kickoff meeting facilitation | A/R | R | R | R | R | I | I |
| Gather requirements | C | R | C | A/R | C | I | I |
| Define acceptance criteria | C | R | C | R | A/R | I | I |
| Estimate effort | C | I | A/R | C | C | I | I |
| Create release plan | A/R | R | C | I | I | I | C |
| Identify dependencies | A/R | C | R | C | I | I | C |
| **Execution Phase** |
| Implement features | I | I | A/R | C | C | I | I |
| Code reviews | I | I | A/R | I | C | I | I |
| Write tests | I | I | R | I | A/R | I | I |
| Defect triage | C | C | R | I | A/R | I | I |
| Daily standups | R | C | R | R | R | I | I |
| Update project status | A/R | C | C | I | C | I | I |
| Risk management | A/R | C | C | C | C | R | I |
| **Change Management** |
| Evaluate change requests | C | C | C | C | C | A/R | I |
| Impact assessment | R | C | R | C | C | A/R | C |
| Communicate changes | R | C | I | I | I | A/R | I |
| Update documentation | R | C | C | R | I | A/R | I |
| **Quality Assurance** |
| Define test strategy | I | C | C | I | A/R | I | I |
| Execute test plans | I | I | C | I | A/R | I | I |
| Track defects | I | I | R | I | A/R | I | I |
| Sign-off on quality | I | C | I | I | A/R | I | C |
| **Release Phase** |
| Verify pre-release requirements | R | C | C | I | R | I | A/R |
| Schedule deployment window | C | C | I | I | I | I | A/R |
| Execute deployment | I | I | R | I | I | I | A/R |
| Post-deployment verification | C | C | R | I | R | I | A/R |
| Release communications | R | R | I | I | I | I | A/R |
| **Retrospective Phase** |
| Facilitate retrospective | A/R | R | R | R | R | R | R |
| Capture action items | A/R | C | C | C | C | C | C |
| Follow up on improvements | A/R | C | C | C | C | C | C |

---

## Decision Authority Matrix

| Decision Type | Primary Decision Maker | Must Consult | Must Inform |
|---------------|----------------------|--------------|-------------|
| Feature prioritization | Product Manager | Project Manager, Business Analyst | Development Team |
| Scope changes | Product Manager, Project Manager | Business Analyst, Change Manager | All stakeholders |
| Technical approach | Developers | Product Manager, Project Manager | Business Analyst |
| Quality standards | QA Lead | Product Manager, Developers | Project Manager |
| Release timing | Product Manager, Project Manager | Release Coordinator, QA Lead | All stakeholders |
| Resource allocation | Project Manager | Product Manager | Development Team |
| Change approval (low impact) | Project Manager | Change Manager | Product Manager |
| Change approval (high impact) | Product Manager, Sponsor | Project Manager, Change Manager | All stakeholders |

---

## Escalation Paths

| Issue Type | First Level | Second Level | Final Level |
|------------|-------------|--------------|-------------|
| Technical blockers | Developer → Tech Lead | Project Manager | Product Manager/Sponsor |
| Requirements clarity | Business Analyst | Product Manager | Sponsor |
| Quality concerns | QA Lead | Project Manager | Product Manager/Sponsor |
| Schedule risks | Project Manager | Product Manager | Sponsor |
| Scope change requests | Change Manager | Project Manager + Product Manager | Sponsor |
| Release issues | Release Coordinator | Project Manager + DevOps Lead | Product Manager/Sponsor |

---

## Notes on Using This Matrix

- **Accountable (A)**: Only one person should be accountable for each activity
- **Responsible (R)**: Multiple people can be responsible for execution
- **Consulted (C)**: Provide input before decisions or actions
- **Informed (I)**: Kept updated on progress or decisions

This matrix should be reviewed and customized for each project based on team size, complexity, and organizational structure.

---

**Related Documents**:
- [Roles and Personas](octoacme-roles-and-personas.md) - Detailed role definitions
- [Project Management Overview](octoacme-project-management-overview.md) - Process overview
- [Risk Management and Communication](octoacme-risks-and-communication.md) - Communication protocols
