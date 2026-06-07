## output-3-mermaid-selection

# Gray-scale Mermaid diagram set for H. R. 9510 v4.0

*Independent research draft. Every diagram below is gray-scale Mermaid (no color,
no images, Rule 5). Each renders directly in GitHub; in the compiled LaTeX bill the
same diagram is reproduced as a matching gray-scale TikZ figure (Overleaf does not
render Mermaid and no raster image is permitted).*

The source families are the colored Mermaid diagrams in
`Clinical-AI-Demos/tree/main/ai-outputs/output-01/ChatGPT.md` (original workflow,
PlantUML component and sequence, D2 declarative map, Excalidraw sketch board,
Graphviz/DOT clustered flow, Structurizr/C4 architecture, BPMN workflow, draw.io
swimlane, hybrid). Each is converted to gray-scale and re-themed from the
software-publication workflow to this bill's subject. **Different and most relevant
diagram types are used throughout, so no figure repeats another's pattern.**

## Shared gray-scale palette

All diagrams use Mermaid's `neutral` theme plus five explicit gray fills, black
strokes, and black text:

- `g1` `#f5f5f5` (lightest) - inputs / context
- `g2` `#e0e0e0` - process steps
- `g3` `#cfcfcf` - decisions / gates
- `g4` `#bdbdbd` - law / statute
- `g5` `#9e9e9e` (darkest) - end goals / the bill

## Figure-slot map

| Fig. | Diagram type (source family) | Bill location | Gray-scale subject |
|:--|:--|:--|:--|
| 1 | Flowchart LR (original workflow) | SEC. 2 | Four-work evidence-to-law lineage |
| 2 | Flowchart TB, paired columns (D2 map) | SEC. 2 | Accelerated timeline vs conventional |
| 3 | BPMN flowchart (BPMN workflow) | SEC. 3 | Ten-gate decision rule and funnel |
| 4 | Component/clustered (Graphviz/DOT) | SEC. 3 | Statutory layering through Title 21 |
| 5 | Flowchart LR (PlantUML component) | SEC. 4 | Comparative-print section order |
| 6 | Swimlane (draw.io) | App. C / App. J | Pre-introduction path by actor |
| 7 | Sequence (PlantUML sequence) | App. L | Evidence to introduction handoff |
| 8 | C4 architecture (Structurizr/C4) | App. C | The verification gate as a system |
| 9 | Flowchart TB (hybrid) | App. K | Prompt and bill-version evolution |

---

## Figure 1 - Four-work evidence-to-law lineage (flowchart LR)

```mermaid
%%{init: {'theme':'neutral','themeVariables':{'fontSize':'13px'}}}%%
flowchart LR
    V1["VVUQ-01<br/>method + 51-test pipeline"]:::g1
    V2["VVUQ-02<br/>10-gate humanoid, 172 tests"]:::g1
    V3["VVUQ-03<br/>standalone bill (v1.0)"]:::g2
    V4["VVUQ-04<br/>FD&C Act amendment (v2.0)"]:::g4
    B["H. R. 9510 v4.0<br/>visual amendment + 12 LaTeX deliverables"]:::g5
    V1 --> V2 --> V3 --> V4 --> B
    classDef g1 fill:#f5f5f5,stroke:#333,stroke-width:1px,color:#000
    classDef g2 fill:#e0e0e0,stroke:#333,stroke-width:1px,color:#000
    classDef g4 fill:#bdbdbd,stroke:#000,stroke-width:1.4px,color:#000
    classDef g5 fill:#9e9e9e,stroke:#000,stroke-width:1.6px,color:#000
```

## Figure 2 - Accelerated timeline versus conventional methods (paired flowchart)

```mermaid
%%{init: {'theme':'neutral'}}%%
flowchart TB
    subgraph CONV["Conventional path (months to years)"]
      C1["Method paper ~ months"]:::g1
      C2["Verified robotics code 6-18 mo"]:::g1
      C3["Manuscript ~ months"]:::g1
      C4["Federal bill + counsel mo-years"]:::g1
      C1 --> C2 --> C3 --> C4
    end
    subgraph THIS["This work (about 11 days)"]
      T1["VVUQ-01 ~ 5 days"]:::g2
      T2["VVUQ-02 ~ 2 days"]:::g2
      T3["VVUQ-03 ~ 1 day"]:::g2
      T4["VVUQ-04 ~ 2 days"]:::g2
      T1 --> T2 --> T3 --> T4
    end
    classDef g1 fill:#f5f5f5,stroke:#333,stroke-width:1px,color:#000
    classDef g2 fill:#cfcfcf,stroke:#000,stroke-width:1.2px,color:#000
```

## Figure 3 - Ten-gate decision rule and funnel (BPMN flowchart)

```mermaid
%%{init: {'theme':'neutral'}}%%
flowchart TB
    S((Start)):::ev
    G["Candidate robot-patient<br/>interaction code"]:::g1
    Q{"Clears all 10<br/>standards-bound gates?"}:::g3
    A["ACCEPT<br/>code may be generated"]:::g5
    B["BLOCK<br/>code withheld"]:::g4
    E{"Borderline?"}:::g3
    ESC["ESCALATE<br/>human review"]:::g2
    S --> G --> Q
    Q -- "yes" --> A
    Q -- "no" --> E
    E -- "no" --> B
    E -- "yes" --> ESC
    ESC --> Q
    classDef ev fill:#ffffff,stroke:#000,stroke-width:1.4px,color:#000
    classDef g1 fill:#f5f5f5,stroke:#333,stroke-width:1px,color:#000
    classDef g2 fill:#e0e0e0,stroke:#333,stroke-width:1px,color:#000
    classDef g3 fill:#cfcfcf,stroke:#000,stroke-width:1.2px,color:#000
    classDef g4 fill:#bdbdbd,stroke:#000,stroke-width:1.4px,color:#000
    classDef g5 fill:#9e9e9e,stroke:#000,stroke-width:1.6px,color:#000
```

## Figure 4 - Statutory layering through Title 21 (clustered component)

```mermaid
%%{init: {'theme':'neutral'}}%%
flowchart LR
    subgraph EX["Existing Title 21 device pathway"]
      D["Device<br/>(§ 321)"]:::g1
      C["Classification<br/>(§ 360c)"]:::g1
      P["510(k) / PMA<br/>(§ 360 / § 360e)"]:::g2
      PC["PCCP<br/>§ 515C / § 360e-4"]:::g2
      D --> C --> P --> PC
    end
    subgraph NEW["This amendment"]
      N["New § 515D / § 360e-5<br/>verify before generation"]:::g5
    end
    PC --> N
    classDef g1 fill:#f5f5f5,stroke:#333,stroke-width:1px,color:#000
    classDef g2 fill:#e0e0e0,stroke:#333,stroke-width:1px,color:#000
    classDef g5 fill:#9e9e9e,stroke:#000,stroke-width:1.6px,color:#000
```

## Figure 5 - Comparative-print section order (component flowchart)

```mermaid
%%{init: {'theme':'neutral'}}%%
flowchart LR
    A["§ 321<br/>definitions"]:::g1
    B["§ 360c<br/>classification"]:::g1
    C["§ 360e<br/>PMA"]:::g2
    D["§ 360e-4<br/>PCCP"]:::g2
    E["§ 360e-5<br/>NEW"]:::g5
    F["§ 360j, 374, 360i<br/>conforming"]:::g1
    A --> B --> C --> D --> E --> F
    classDef g1 fill:#f5f5f5,stroke:#333,stroke-width:1px,color:#000
    classDef g2 fill:#e0e0e0,stroke:#333,stroke-width:1px,color:#000
    classDef g5 fill:#9e9e9e,stroke:#000,stroke-width:1.6px,color:#000
```

## Figure 6 - Pre-introduction path by actor (swimlane)

```mermaid
%%{init: {'theme':'neutral'}}%%
flowchart TB
    subgraph SPON["Sponsoring office"]
      A["Consolidate one text"]:::g2
      B["Recruit cosponsors"]:::g2
      F["Introduce via eHopper"]:::g5
    end
    subgraph EXP["Experts / counsel"]
      C["Human + legal review"]:::g1
      D["Currency check"]:::g1
    end
    subgraph HOLC["HOLC + Clerk"]
      E["Legislative form;<br/>attach CAS + PAYGO"]:::g2
      G["Clerk assigns number;<br/>refer to E&C"]:::g4
    end
    A --> C --> D --> E --> B --> F --> G
    classDef g1 fill:#f5f5f5,stroke:#333,stroke-width:1px,color:#000
    classDef g2 fill:#e0e0e0,stroke:#333,stroke-width:1px,color:#000
    classDef g4 fill:#bdbdbd,stroke:#000,stroke-width:1.4px,color:#000
    classDef g5 fill:#9e9e9e,stroke:#000,stroke-width:1.6px,color:#000
```

## Figure 7 - Evidence to introduction handoff (sequence)

```mermaid
%%{init: {'theme':'neutral'}}%%
sequenceDiagram
    autonumber
    actor K as Author (human)
    participant AI as Claude Code Opus 4.8
    participant T as VVUQ gates / tests
    participant L as Legislative Counsel
    participant H as House (eHopper)
    K->>AI: Requirements (verify before generation)
    AI->>T: Generate + run assurance suite
    T-->>AI: 172/172 tests; 10 gates clear
    AI->>K: Draft -> full -> final bill + deliverables
    K->>L: Route final text for legislative form
    L-->>K: Introduction-ready measure
    K->>H: Sponsor introduces; Clerk assigns number
```

## Figure 8 - The verification gate as a system (C4 architecture)

```mermaid
%%{init: {'theme':'neutral'}}%%
flowchart TB
    Person(["Person<br/>trial sponsor / investigator"]):::g1
    subgraph SYS["System: verify-before-generate gate (new § 360e-5)"]
      Gate{{"Component<br/>automated VVUQ gate"}}:::g3
      Std[("Component<br/>standards bindings<br/>ASME V&V 40, ISO/TS 15066")]:::g2
      Rec[("Component<br/>immutable record<br/>part 11")]:::g2
    end
    FDA["External<br/>FDA review (PMA / PCCP)"]:::g4
    Person -->|submits code| Gate
    Gate -->|checks against| Std
    Gate -->|writes| Rec
    Gate -->|ACCEPT artifact| FDA
    classDef g1 fill:#f5f5f5,stroke:#333,stroke-width:1px,color:#000
    classDef g2 fill:#e0e0e0,stroke:#333,stroke-width:1px,color:#000
    classDef g3 fill:#cfcfcf,stroke:#000,stroke-width:1.2px,color:#000
    classDef g4 fill:#bdbdbd,stroke:#000,stroke-width:1.4px,color:#000
```

## Figure 9 - Prompt and bill-version evolution (hybrid flowchart)

```mermaid
%%{init: {'theme':'neutral'}}%%
flowchart TB
    subgraph PR["Prompt evolution"]
      P1["next-steps"]:::g1
      P2["figures-bill"]:::g1
      P3["draft-bill"]:::g2
      P4["full-bill"]:::g2
      P5["final-bill"]:::g2
      P1 --> P2 --> P3 --> P4 --> P5
    end
    subgraph BV["Bill version evolution"]
      B1["v1.0 VVUQ-03"]:::g1
      B2["v2.0 VVUQ-04"]:::g2
      B3["v3.0 VVUQ-05"]:::g3
      B4["v4.0 this build"]:::g5
      B1 --> B2 --> B3 --> B4
    end
    P5 -.-> B4
    classDef g1 fill:#f5f5f5,stroke:#333,stroke-width:1px,color:#000
    classDef g2 fill:#e0e0e0,stroke:#333,stroke-width:1px,color:#000
    classDef g3 fill:#cfcfcf,stroke:#000,stroke-width:1.2px,color:#000
    classDef g5 fill:#9e9e9e,stroke:#000,stroke-width:1.6px,color:#000
```

---

## Conversion notes for the LaTeX bill

- Each diagram maps to one `mermaidfig` slot in the bill. The LaTeX `usctitle.sty`
  defines TikZ node styles `mmg1`..`mmg5` matching the five gray fills, plus a
  `mermaidfig` environment that centers the diagram on a white background with a
  thin black frame and a figure caption, exactly as the prior bill's `asciifig`
  centered its ASCII art.
- Node shapes follow the Mermaid source: rounded rectangles for steps, diamonds for
  decisions (BPMN/decision diagrams), stadiums for persons, hexagons/cylinders for
  components (C4), and lanes for swimlanes.
- Gray-scale only: no color survives the conversion; emphasis is by gray level and
  stroke weight, matching the palette above.
