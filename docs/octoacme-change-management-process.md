# OctoAcme Change Management Process

## Purpose
Establish a structured approach for evaluating, approving, and implementing changes to project scope, schedule, or resources. This process ensures controlled changes while maintaining project stability.

---

## When to Use This Process

Use this change management process when:
- Changes to agreed-upon project scope or deliverables are proposed
- Significant schedule adjustments are needed
- Resource allocation changes impact project commitments
- Requirements changes affect multiple teams or dependencies
- Changes have budget or contract implications

**Note**: Minor clarifications, bug fixes, and small implementation details typically don't require formal change management.

---

## Change Impact Levels

### Level 1: Minor Changes
- **Definition**: Limited scope, minimal timeline impact (< 1 week), no additional resources needed
- **Examples**: Minor UI adjustments, documentation updates, small feature refinements
- **Approval**: Project Manager + Product Manager (informal)
- **Documentation**: Update in project backlog or decision log

### Level 2: Moderate Changes
- **Definition**: Moderate scope impact, timeline impact (1-4 weeks), may require resource adjustment
- **Examples**: New features within current project, significant requirement changes, dependency shifts
- **Approval**: Change Control Board review (if applicable) or formal PM/PdM approval
- **Documentation**: Change request form required

### Level 3: Major Changes
- **Definition**: Significant scope change, major timeline impact (> 4 weeks), resource or budget changes
- **Examples**: Major feature additions, project pivot, significant schedule extension
- **Approval**: Sponsor/Executive approval required
- **Documentation**: Full impact assessment and revised project charter

---

## Change Request Process

### Step 1: Submit Change Request

**Requester completes**:
- [ ] Change request form (template below)
- [ ] Business justification
- [ ] Preliminary impact assessment

**Submitted to**: Change Manager or Project Manager

---

### Step 2: Initial Review & Assessment

**Change Manager evaluates**:
- [ ] Completeness of request
- [ ] Alignment with project goals
- [ ] Urgency and priority
- [ ] Initial categorization (Level 1/2/3)

**Timeline**: Within 2 business days

---

### Step 3: Impact Analysis

**Relevant stakeholders assess**:
- [ ] **Business Analyst**: Requirements impact, stakeholder alignment
- [ ] **Developers**: Technical feasibility, effort estimate, risks
- [ ] **QA Lead**: Testing impact, quality implications
- [ ] **Project Manager**: Schedule impact, resource needs, dependencies
- [ ] **Product Manager**: Product strategy alignment, priority trade-offs
- [ ] **Release Coordinator**: Release timing impact (if applicable)

**Timeline**: 2-5 business days depending on complexity

---

### Step 4: Decision & Approval

**Change Control Board (or approval authority)**:
- [ ] Review impact assessment
- [ ] Evaluate alternatives
- [ ] Consider project health and risk
- [ ] Make approval decision

**Possible Outcomes**:
- **Approved**: Proceed with implementation
- **Approved with Modifications**: Implement with specified adjustments
- **Deferred**: Postpone to future release or phase
- **Rejected**: Do not proceed

**Timeline**: Within 3-5 business days of completed impact analysis

---

### Step 5: Implementation & Communication

**If approved, Change Manager coordinates**:
- [ ] Update project documentation (scope, schedule, requirements)
- [ ] Communicate decision and impacts to all stakeholders
- [ ] Update risk register with new or modified risks
- [ ] Ensure team is briefed on changes
- [ ] Track change in change log

**Timeline**: Within 1-2 business days of approval

---

### Step 6: Monitor & Track

**Project Manager and Change Manager**:
- [ ] Track change through implementation
- [ ] Monitor for secondary impacts
- [ ] Update stakeholders on progress
- [ ] Validate change was implemented as intended

**Ongoing throughout implementation**

---

## Change Request Template

### Change Request Form

**Change ID**: CR-[Project]-[Number] (e.g., CR-OCTOACME-001)  
**Date Submitted**: _______________  
**Submitted By**: _______________  
**Project Name**: _______________

---

#### 1. Change Description
**Brief description of proposed change**:


**Category** (select one):
- [ ] Scope change (features/deliverables)
- [ ] Schedule change (timeline/milestones)
- [ ] Resource change (team/budget)
- [ ] Requirements change
- [ ] Technical approach change
- [ ] Other: _______________

---

#### 2. Business Justification
**Why is this change needed?**


**What happens if we don't make this change?**


**Priority** (select one):
- [ ] Critical (project cannot succeed without this)
- [ ] High (significant value or risk mitigation)
- [ ] Medium (valuable but not essential)
- [ ] Low (nice to have)

---

#### 3. Impact Assessment

**Scope Impact**:
- What deliverables are affected?
- What new work is required?


**Schedule Impact**:
- Estimated delay or acceleration: _____ weeks
- Which milestones are affected?


**Resource Impact**:
- Additional team members needed?
- Budget impact: $______
- Tools or infrastructure needs?


**Quality Impact**:
- Testing requirements:
- Risk considerations:


**Dependency Impact**:
- Which teams or projects are affected?
- External dependencies impacted?


---

#### 4. Alternatives Considered

**What alternatives were evaluated?**


**Why was this approach selected?**


---

#### 5. Risk Assessment

**Risks of implementing this change**:


**Mitigation strategies**:


---

#### 6. Approvals

| Role | Name | Decision | Date | Signature |
|------|------|----------|------|-----------|
| Change Manager | | ☐ Approve ☐ Reject ☐ Defer | | |
| Project Manager | | ☐ Approve ☐ Reject ☐ Defer | | |
| Product Manager | | ☐ Approve ☐ Reject ☐ Defer | | |
| Sponsor (if Level 3) | | ☐ Approve ☐ Reject ☐ Defer | | |

**Final Decision**: ☐ Approved  ☐ Approved with Modifications  ☐ Deferred  ☐ Rejected

**Decision Notes**:


---

#### 7. Implementation Plan (if approved)

**Implementation start date**: _______________  
**Expected completion date**: _______________  
**Owner**: _______________

**Key implementation steps**:
1. 
2. 
3. 

**Communication plan**:


---

## Change Log Template

Track all changes in a centralized change log for the project:

| Change ID | Date | Description | Impact Level | Status | Decision | Implementation Date |
|-----------|------|-------------|--------------|--------|----------|-------------------|
| CR-001 | 2026-01-15 | Add mobile responsiveness | Level 2 | Approved | Implement in Sprint 3 | 2026-01-25 |
| CR-002 | 2026-01-18 | Change authentication method | Level 3 | Deferred | Move to Phase 2 | TBD |

---

## Best Practices

1. **Be proactive**: Identify potential changes early before they become crises
2. **Assess honestly**: Provide realistic impact assessments, not optimistic estimates
3. **Communicate widely**: Ensure all affected parties are informed
4. **Document everything**: Maintain clear records of decisions and rationales
5. **Learn from changes**: Review change patterns in retrospectives to improve planning
6. **Balance stability and flexibility**: Enable necessary changes while protecting team focus

---

## Escalation Process

If change decisions are contested or urgent decisions are needed:

1. **Standard escalation**: Project Manager → Product Manager → Sponsor
2. **Timeline**: Emergency decisions within 24 hours; standard within 3-5 days
3. **Documentation**: All escalated decisions must be documented with rationale

---

**Related Documents**:
- [Roles and Personas](octoacme-roles-and-personas.md) - Role definitions including Change Manager
- [Stakeholder Responsibility Matrix](octoacme-stakeholder-responsibility-matrix.md) - Decision authority
- [Risk Management and Communication](octoacme-risks-and-communication.md) - Communication protocols
- [Project Planning](octoacme-project-planning.md) - Planning process
