# Tracker Feedback Analysis — JTBD + UX Audit

Source file: `tracker_feedback_codex.json` (107 qualitative responses, Russian language).

## 1) Executive summary

Users see Tracker as a **flexible but hard-to-scale work management system**. Core value exists (task tracking, comments, workflows), but advanced teams hit recurring friction in:

1. **Configuration complexity** (projects, workflows, fields, board setup).
2. **Planning visualization gaps** (roadmap/tree/Gantt/dependency views).
3. **Search and discoverability** (finding tasks, filters, recent items, cross-project navigation).
4. **Collaboration signal quality** (discussion clarity, notifications, docs/wiki context).
5. **Weak reporting and management visibility** (dashboards/metrics for leads).

Net: Tracker works for execution, but users need better support for **planning, alignment, and system-level clarity**.

---

## 2) JTBD extraction

### Functional JTBD

1. **When I plan initiatives across teams, I want hierarchy + timeline views, so I can see roadmap dependencies and delivery risk early.**
2. **When I configure a project, I want reusable templates/constructors, so I can launch and adapt workflows without admin overhead.**
3. **When I search for work, I want fast contextual discovery (recently viewed, smart filters, linked work), so I can update tasks without losing time.**
4. **When we collaborate on tasks, I want structured discussion + clear notifications, so decisions are not lost in long comment threads.**
5. **When I report status to management, I want actionable dashboards and progress metrics, so I can communicate outcomes without manual exports.**

### Emotional / social JTBD

1. **Reduce cognitive load:** “I don’t want to feel lost in settings and custom fields.”
2. **Increase confidence:** “I need to trust planning artifacts reflect reality.”
3. **Protect team credibility:** “I need to present clean progress views for stakeholders.”

### Main competing alternatives users mentally compare against

- Jira (flexibility/ecosystem expectations)
- Asana (Gantt/timeline ease)
- Notion/Confluence-like docs collaboration

---

## 3) Theme prevalence (signal-level, keyword-assisted)

Out of 107 responses:

- **Customization & setup friction:** 42 mentions (~39%)
- **Search/navigation/discovery friction:** 39 mentions (~36%)
- **Collaboration/docs/notification friction:** 28 mentions (~26%)
- **Planning visualization gaps:** 18 mentions (~17%)
- **Reporting/analytics gaps:** 14 mentions (~13%)
- **UX simplicity concerns:** 12 mentions (~11%)
- **Integrations/API requests:** 12 mentions (~11%)
- **Performance/stability complaints:** 5 mentions (~5%)

Interpretation: The strongest opportunities are **information architecture + workflow ergonomics**, then **planning visibility** and **management reporting**.

---

## 4) UX audit (heuristic + evidence-aligned)

## A. Information architecture & discoverability

**Observed issues**
- Hard to find tasks quickly (especially across boards/projects).
- Limited or rigid filter behavior in key views.
- Need for “recently opened” context when linking tasks.

**UX impact**
- High interaction cost for simple actions.
- Frequent context switching and manual lookup by task ID.

**Severity:** High

**Audit verdict**
- Current discovery model appears optimized for known-item retrieval, not exploratory navigation.

## B. Configuration complexity / system ergonomics

**Observed issues**
- Setup of projects, task types, statuses/transitions feels overly complex.
- Desire for board/card constructors and dynamic layouts.

**UX impact**
- Adoption risk for non-admin users.
- Inconsistent workspace quality between teams.

**Severity:** High

**Audit verdict**
- Flexibility is a strength, but progressive disclosure is insufficient.

## C. Planning and portfolio visibility

**Observed issues**
- Repeated demand for Gantt-like timeline, dependency links, tree hierarchy, swimlanes.

**UX impact**
- Teams cannot easily map delivery sequence and cross-initiative dependency risk.

**Severity:** High for managers/program owners; Medium for ICs.

**Audit verdict**
- Tracker under-serves strategic planning workflows compared with user expectations.

## D. Collaboration quality

**Observed issues**
- Comment-heavy workflows become noisy; decisions can be hard to extract.
- Need for stronger notification targeting and embedded docs context.

**UX impact**
- Decision latency and repeated clarification loops.

**Severity:** Medium-High

## E. Reporting and stakeholder communication

**Observed issues**
- Need for better dashboards/analytics views and less manual reporting labor.

**UX impact**
- Extra overhead for leads/PMs and weaker executive visibility.

**Severity:** Medium-High

## F. Performance / reliability

**Observed issues**
- Some mentions of lag/instability.

**UX impact**
- Trust erosion and reduced willingness to use advanced views.

**Severity:** Medium (based on lower mention count, but high consequence when present).

---

## 5) Opportunity sizing and prioritization

## Priority 1 (Now): reduce friction in core workflows

1. **Universal command/search bar** (tasks, projects, people, recent entities, saved filters).
2. **Board/card view constructor v1** with presets (Team Scrum, Kanban Ops, Product Roadmap).
3. **Guided workflow setup** with templates + “advanced mode” split.

Expected outcome: lower time-to-task-update, lower onboarding friction, improved perceived simplicity.

## Priority 2 (Next): planning confidence layer

1. **Roadmap hierarchy view** (Initiative → Epic → Task).
2. **Timeline/Gantt with dependencies** and critical path warnings.
3. **Cross-project dependency map**.

Expected outcome: stronger program-level planning; higher management adoption.

## Priority 3 (Then): communication and insight loop

1. **Decision summaries inside tasks** (pin resolution, owner, due date).
2. **Role-aware notifications** (reduce noise; increase relevance).
3. **Executive dashboard pack** (delivery status, blockers, forecast).

Expected outcome: faster decision cycles and clearer stakeholder reporting.

---

## 6) Suggested UX metrics (to validate improvements)

1. **Median time to find + open correct task**.
2. **Median time to create configured board/workflow**.
3. **% tasks with unresolved dependency conflicts**.
4. **Notification relevance score** (opened/acted vs ignored).
5. **Weekly reporting prep time (self-reported) for leads**.
6. **SUS or UMUX-Lite trend by role (IC, PM, Manager, Admin)**.

---

## 7) Risks and caveats

- This is qualitative feedback and likely over-represents engaged/power users.
- Keyword-assisted prevalence is directional, not exact coding.
- No segmentation metadata (role/company size/use-case maturity) was provided; prioritization should be validated with role-based slices.

---

## 8) Recommended next research step

Run a **role-segmented follow-up** with 12–15 interviews:
- 5 ICs, 5 PM/Leads, 2–5 Admins.
- Script around three journeys: setup, planning, status reporting.
- Convert top pain points into prototype tests (search, setup wizard, roadmap view).

This will de-risk feature investment and sharpen rollout sequencing.
