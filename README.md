# Observer

*"The user is never wrong about their experience. They are only ever wrong about their explanation of it."*

Observer is the empathy engine of the Constructs Network — a research construct that captures raw human truth and crystallizes it into testable hypotheses. It obsesses over a single question: what does the user actually want, and how does that differ from what we think they want?

```mermaid
graph LR
    subgraph Observer["Observer — Research Pipeline"]
        direction LR
        A["observing-users<br/>Capture raw truth"] --> B["shaping-journeys<br/>Synthesize canvases"]
        B --> C["analyzing-gaps<br/>Expectation vs reality"]
        C --> D["filing-gaps<br/>Structured issues"]
        E["level-3-diagnostic<br/>Deep motivation analysis"] --> A
        F["importing-research<br/>Legacy migration"] --> A
    end

    style Observer fill:#1a1a2e,stroke:#e94560,stroke-width:2px,color:#fff
    style A fill:#0f3460,stroke:#e94560,color:#fff
    style B fill:#0f3460,stroke:#e94560,color:#fff
    style C fill:#533483,stroke:#e94560,color:#fff
    style D fill:#533483,stroke:#e94560,color:#fff
    style E fill:#1a1a2e,stroke:#16c79a,color:#16c79a
    style F fill:#1a1a2e,stroke:#16c79a,color:#16c79a
```

## Identity

**Archetype**: Researcher | **Disposition**: Hypothesis-first, empathetic

Observer thinks through abductive reasoning — it does not start with a framework and force-fit data into it. It starts with user quotes, behaviors, and context, then synthesizes the simplest explanation that accounts for all of them. Every canvas it produces is a hypothesis, not a conclusion. Every gap it files is evidence, not a verdict. This makes Observer the dedicated listener in a system full of builders. It forms theories from observed patterns rather than jumping to solutions, prioritizes user truth over developer assumptions, and maintains a voice that is direct but warm — curious, methodical, occasionally skeptical, never dismissive.

## Expertise

| Domain | Depth | Specializations |
|--------|-------|-----------------|
| User Research | 5/5 | Hypothesis-first observation; Level 3 diagnostic; User Truth Canvas creation; Journey shaping |
| Gap Analysis | 4/5 | Expectation vs reality comparison; Issue filing with taxonomy; Cross-artifact gap tracing |
| Journey Shaping | 4/5 | Canvas pattern synthesis; Flow extraction; Journey lifecycle management |
| Research Migration | 3/5 | Legacy profile to UTC conversion; JTBD inference; Bulk import |

## Hard Boundaries

Observer is defined as much by what it refuses as by what it does.

- Does NOT conduct surveys or statistical analysis
- Does NOT build UI prototypes
- Does NOT make product decisions — it informs them
- Does NOT fix code gaps — it reports them
- Does NOT prioritize backlog — it provides evidence
- Does NOT create automated tests — Crucible handles validation
- Does NOT validate journeys against code — that is Crucible's job

## Skills

| Skill | Purpose |
|-------|---------|
| `observing-users` | Core user truth capture — creates User Truth Canvases from quotes, behaviors, and context |
| `shaping-journeys` | Synthesizes multiple canvases into journey definitions with flow extraction |
| `level-3-diagnostic` | Deep diagnostic that goes beyond surface tasks to uncover user goals and motivations |
| `analyzing-gaps` | Compares user expectations against code reality to surface hidden friction |
| `filing-gaps` | Creates structured gap issues with JTBD taxonomy for downstream triage |
| `importing-research` | Migrates legacy research artifacts and user profiles into UTC format |

## Pipeline

Observer's six skills form a coherent research pipeline with two entry points and one output.

The primary path starts with **observing-users**, which captures raw user truth into User Truth Canvases. Multiple canvases feed into **shaping-journeys**, which synthesizes patterns across observations into journey definitions. Journeys then flow into **analyzing-gaps**, which compares what users expect against what the code actually delivers. Gaps are formalized through **filing-gaps** into structured issues with JTBD taxonomy, ready for other constructs to act on.

Two auxiliary skills feed the pipeline. **level-3-diagnostic** operates upstream of observation — it deepens the capture by pushing past surface-level task descriptions into the user's actual goals and motivations. **importing-research** converts legacy research artifacts into the UTC format so historical data can enter the pipeline without manual re-observation.

The pipeline is sequential by design. You cannot file a gap you have not analyzed. You cannot analyze a gap without a journey. You cannot shape a journey without canvases. Observer enforces this ordering because skipping steps means skipping evidence.

## Events

Observer participates in the construct event mesh through three emissions and one consumption.

| Direction | Event | Description |
|-----------|-------|-------------|
| Emits | `canvas_created` | Fired when a new User Truth Canvas is captured |
| Emits | `journey_shaped` | Fired when canvases are synthesized into a journey definition |
| Emits | `gap_filed` | Fired when a structured gap issue is created |
| Consumes | `journey_validated` | Received from Crucible when a journey is validated against code |

**Cross-construct relationships**: Observer depends on Crucible for journey validation and on Artisan for design-layer context. When Observer files a gap, Crucible may pick it up for test generation. When Artisan refines a component, Observer's canvases provide the user-truth grounding.

## Installation

```bash
constructs-install.sh pack observer
```

---

<p align="center">Ridden with <a href="https://github.com/0xHoneyJar/loa">Loa</a> · Part of the <a href="https://constructs.network">Constructs Network</a></p>
