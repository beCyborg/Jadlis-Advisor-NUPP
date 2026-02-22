# NUP6: Use Repeatable Elements

## Context

Read this file when the NUP Scan flags NUP6 as Yellow or Red, or when the user's situation involves any of the following:

- Every task or deliverable is being approached from scratch, with no templates, checklists, or standard workflows
- The team cannot describe what "done" means for a given deliverable type
- Quality problems are inconsistent: some deliverables are done well, others miss obvious criteria, with no clear pattern
- The project has recurring activities but no defined way to perform them consistently
- There is no regular meeting cadence, review cycle, or sprint structure — planning and coordination happen ad hoc
- The team is adopting a methodology but applying it without any tailoring to their context
- People describe the project's processes as "bureaucratic" or as obstacles rather than supports
- Lessons from past projects are not informing current work

This reference gives Claude the NUPP-specific framework for diagnosing repeatability gaps and recommending appropriate interventions. Claude's general training includes general knowledge of checklists, workflows, and Agile methodologies but does not include the NUPP hierarchy of repeatable elements or the specific diagnostic logic for identifying which layer of repeatability to introduce in a given project situation.

---

## The Principle

NUP6 states: **Use repeatable elements, preferably in repeatable cycles.**

Ad hoc execution is expensive in two ways. First, energy cost: every time a team approaches a task from scratch, they spend energy reconstructing context and reinventing structure that has already been worked out — or that could be worked out once and reused. Second, inconsistency: when every deliverable is assembled differently, quality depends on who happened to be involved and what they happened to remember. Some items come out well; others miss obvious criteria. The failure mode is not negligence — it is the predictable result of relying on improvisation rather than systematized knowledge.

Repeatable elements — checklists, workflows, cycles, methodologies — are crystallizations of prior judgment that can be applied again without reconstructing that judgment each time. The team spends energy once (designing the element) and much less energy on every subsequent application.

The order of preference in NUP6 is specific: repeatable elements placed inside repeatable cycles are better than elements applied ad hoc. Cycles make elements self-triggering. A team that runs a weekly review does not decide each week whether to run it — the cycle decides.

---

## The Checklist Hierarchy

Checklists are the most accessible entry point into repeatability. They require minimal process overhead, are easy to build incrementally, and provide immediate quality assurance benefits. NUPP describes a four-level hierarchy that allows checklists to grow in scope and reusability.

### Level 1: Individual Checklist

A quality checklist for a single deliverable. Before work begins — on a requirements document, a software module, a stakeholder presentation — the team lists what "done" means for that specific item.

This is a planning act, not just a quality act. Writing "the presentation must include a clear recommendation and three supporting data points" before starting forces clarity at the moment when changing course is cheap. Individual checklists are not yet repeatable — they are specific. But they establish the habit of explicit quality criteria that the higher levels build on.

### Level 2: Category Checklist

When a project contains multiple similar deliverables, individual checklists start to converge. The team generalizes: instead of writing a separate checklist for each requirements document, they write one requirements-document checklist and apply it to all instances of that type. The checklist is now repeatable within the project.

When a specific deliverable has unique criteria beyond the category standard, those are added as supplemental items — but the generic list forms the base. The practical test: can a new team member pick up any deliverable of that type and immediately know what done looks like?

### Level 3: Parent Checklist

Once a project has category checklists for several deliverable types, common items emerge across categories: "Has the deliverable been reviewed by a relevant stakeholder?" "Is the source of key decisions documented?" These are not requirements-document questions or design-document questions — they are project-wide quality criteria.

Extracting these common items produces a parent checklist: a single project-wide generic list that applies to all deliverables regardless of category. Each deliverable must satisfy the parent checklist, plus its category checklist, plus any individual supplemental items. Scrum's Definition of Done operates at this level — every increment must satisfy it, regardless of which features it contains.

The hierarchy prevents both under-specification (no criteria at all) and over-specification (an impossibly long checklist for every deliverable). Each level adds scope incrementally.

### Level 4: Cross-Project Reuse

A well-built set of checklists from one project becomes the starting point for the next. At Level 4, the team takes checklists from a prior project, identifies what is generic enough to carry over, and tailors those items to the new context. Each project refines the checklists; the refinements accumulate across projects rather than disappearing.

Tailoring is the critical discipline at this level. Carrying checklists over without review defeats the purpose — different projects have different priorities and risk profiles. The starting point is inherited; the content must be examined and adapted.

---

## Processes and Workflows

Some categories of work are not well captured by a checklist alone. When producing a deliverable requires a defined sequence of steps involving multiple people, a workflow is more appropriate.

A workflow makes explicit: what happens first, what happens next, who is responsible at each step, and approximately how long each step takes. It is the right tool when the question is not just "is this done correctly?" but "how does this move through the team?" A common example: deliverables requiring individual design, stakeholder review, revision, and formal approval. Without a defined workflow, handoffs rely on informal communication that is easily missed or delayed. With one, delays become visible rather than invisible.

The balance point on workflow complexity is critical. When a workflow requires more effort to follow than it saves, people stop following it — they route around it and maintain the official process as a compliance fiction. The test: do people describe the workflow as something that helps them, or as something they have to comply with? The answer is diagnostic information about whether the workflow is appropriately scoped.

---

## Cycles

The second part of NUP6 — "preferably in repeatable cycles" — is not a decoration on the principle. It is an amplifier. A checklist applied when someone remembers to apply it is less reliable than one embedded in a regular cycle. The cycle makes the repeatable element self-executing and removes the overhead of deciding each time whether and when to run it.

Major PM methodologies all use cycles, with instructive variation in how they do so:

- **Scrum** uses a single cycle type — the Sprint, typically two weeks — with defined events inside it. One cycle type, consistently applied, is simple to understand and adopt.
- **DSDM** uses two cycle types: short timeboxes for tactical execution and longer iteration cycles for phased delivery. Different work rhythms for different activity types within the same project.
- **P3.express** uses three cycle types: daily, weekly, and monthly. Each type handles activities at the frequency appropriate to its scope — immediate coordination, progress review, and strategic assessment respectively.
- **PRINCE2** structures projects into stages, with daily and weekly cycles nested inside each stage.
- **PMBOK** describes process groups that repeat across multiple project phases, creating a cycle at the phase level.

Shorter cycles are easier to adopt, but very short cycles may not suit all project types. A project with deliverables requiring months of preparation cannot usefully be reviewed in two-week increments. When one cycle length does not fit, the solution is multiple cycle types operating in parallel — not a single longer cycle.

---

## Methods as Repeatable Elements

Using an established methodology is itself an application of NUP6. A methodology is a comprehensive repeatable element: an integrated system of checklists, workflows, roles, cycles, and decision criteria refined across many projects. Starting with an existing methodology rather than building custom processes from scratch means beginning with tested knowledge rather than an empty page.

The repeatable elements exist on a spectrum of abstraction and tailoring demand:

1. **Quality checklists**: Concrete, minimal tailoring required. A checklist for a deliverable type needs little adjustment to be immediately useful.
2. **Workflows**: Moderate abstraction. Tailoring for the team's specific roles and communication patterns is needed.
3. **Cycles**: Moderate tailoring. Cycle length and events must be calibrated to project type and team size.
4. **Methodologies**: Highest abstraction, highest tailoring requirement. PRINCE2 or Scrum provide a complete system but must be substantially adapted to the specific context.

NUP6 applies the same discipline at every level: tailoring is not optional. It is the mechanism by which a generic repeatable element is made to fit the real situation. Whenever adopting any repeatable element, explicitly identify what tailoring is needed and do it before deployment.

---

## Diagnostic Questions

During a NUP Scan, the following questions assess NUP6 health:

- What proportion of project work is done ad hoc versus using defined repeatable elements?
- Do quality checklists exist? At which level of the hierarchy (individual, category, parent, cross-project)?
- Are there defined workflows for recurring activities such as review, approval, or escalation?
- Is there a regular cadence — daily, weekly, sprint — and does the team reliably use it?
- Is a methodology in use? Has it been explicitly tailored for this project's context?
- Are lessons from this project being systematically captured in a form usable for future projects?
- When team members describe the project's processes, do they use the language of support or the language of compliance?

The last question is particularly diagnostic. "We use the workflow to make sure nothing falls through" signals NUP6 health. "We have to fill out the template before we can move forward" signals a tailoring failure — the element exists but is experienced as an obstacle rather than a tool.

---

## Methodology Cross-References

| Methodology | Repeatable Element | NUP6 Layer |
|---|---|---|
| Scrum | Sprint | Cycle |
| Scrum | Sprint events (Planning, Review, Retrospective, Daily) | Repeatable ceremonies within cycle |
| Scrum | Definition of Done | Parent checklist |
| PRINCE2 | Seven processes | Repeatable process workflow |
| PRINCE2 | Stage structure | Cycle |
| PRINCE2 | Quality theme, Product Description | Category/individual checklist |
| PMBOK | Process groups (Initiating, Planning, Executing, Monitoring, Closing) | Repeatable across phases |
| PMBOK | Organizational Process Assets (OPAs) | Cross-project Level 4 reuse |
| P3.express | Daily, weekly, monthly activities | Multiple cycle types |
| DSDM | Timeboxes + iteration cycles | Dual cycle types |
| XP | Daily routine (pair up, pick item, design, test, code, integrate) | Cycle with embedded workflow |

---

## Anti-patterns

### Reinventing the Wheel

The baseline failure mode for NUP6 is the absence of any repeatable elements. Every task is approached as a unique problem. Every deliverable is assembled without reference to how similar deliverables were built before. Every decision about how to do the work is made fresh.

The costs are distributed and invisible. The time spent each time to reconstruct structure, establish criteria, and coordinate the work does not appear as a line item — it appears as general project slowness and as meetings that feel unproductive because the team is spending half the time agreeing on process before addressing substance.

The inconsistency cost is equally invisible until quality problems surface. When there are no shared criteria for done, individual team members apply their own implicit standards. Some items meet a high bar. Others miss obvious criteria. The variation looks random from the outside, which makes it harder to diagnose — but it maps directly to the absence of any category or parent checklist.

### Bureaucratic Over-engineering

The opposite failure mode is creating repeatable elements so detailed and documentation-intensive that they become obstacles. The checklist has 47 items. The workflow requires five approval signatures. The methodology template demands a 20-page document before any execution can begin.

People respond predictably: they route around it. They do the informal work first, then backfill the documentation. The element exists in a zombie state — officially present, practically absent. The organization pays the overhead without receiving the benefit.

The diagnostic signal is the compliance language described above. When team members say they "have to" follow a process rather than that they "use" it, the element has crossed from support to bureaucracy. The intervention is not to eliminate the element but to trim it: identify what is genuinely useful and strip out the overhead that serves no practical purpose.

### Copy-Paste Methodology

Adopting a methodology and applying it without tailoring is a failure mode specific to the highest abstraction level of NUP6. The team identifies Scrum or PRINCE2 or DSDM as appropriate, reads about how it works, and implements it exactly as described — Sprint length, ceremonies, artifacts, roles — without examining whether those specifics fit the project context.

The book says two-week Sprints. The project has deliverables with a six-week design cycle. The team runs nine Sprints with nothing to show before the first deliverable is complete. The book says the product owner is a single person. The project has five stakeholder groups with conflicting authority. The assigned product owner gets overridden in every Sprint Review.

Any methodology is a generalization designed for a range of contexts, not for a specific project. Tailoring is the mechanism for moving from the general to the specific. Without it, the methodology's structure is present but its value is not. The intervention: for each component of the methodology, ask whether it fits this project's context and what adjustment is needed. Document the tailoring decisions so they can be revisited as the project evolves.

### Cycle Rigidity

Adopting a single cycle length and refusing to adjust it, despite evidence that it does not fit the project, is a specific form of copy-paste methodology applied to the cycle dimension.

The evidence usually takes one of two forms: either the cycle is too short (the team is constantly cutting off work-in-progress to hit the cycle boundary, and reviews feel premature) or too long (the cycle is long enough that problems accumulate undetected for extended periods before a review surface them).

The rigidity often comes from treating the cycle length as a methodology requirement rather than a design choice. "Scrum says two-week Sprints" becomes a constraint rather than a starting point. The team adjusts its work to the cycle instead of adjusting the cycle to the work.

The solution is multiple cycle types calibrated to different types of activity. Immediate coordination needs a short cycle — daily or near-daily. Progress review needs a medium cycle — weekly or bi-weekly. Strategic assessment needs a longer cycle — monthly or stage-based. These can coexist in the same project. Choosing one cycle length for everything is a simplification that works only when one type of activity dominates the project, which is rarely the case.
