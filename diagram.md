flowchart TD
    U["👤 Professional<br/>starts a deliverable"] --> G0

    subgraph G0S["G0 — Framing"]
        G0["Domain + reference framework?"] --> Q{"Confirmed by<br/>professional?"}
        Q -- "Yes" --> LOCK["Source registry<br/>locked"]
        Q -- "Uncertain" --> FLAG["AI suggests leads,<br/>flagged 'unconfirmed'"]
        FLAG --> Q
    end

    LOCK --> G1["G1 — Design<br/>architecture & method documented"]
    G1 --> G2["G2 — Execution<br/>AI-assisted production, tests"]
    G2 --> G3S

    subgraph G3S["G3 — Technical Validation"]
        G3["Reference cases,<br/>sources validated"] --> C{"Criticality<br/>level?"}
        C -- "N1 / N2 / N3" --> G3OK["Professional review"]
        C -- "N4" --> G3IND["+ Independent<br/>qualified reviewer<br/>required"]
    end

    G3OK --> G4["G4 — Client Deliverable<br/>reviewed, archived"]
    G3IND --> G4
    G4 --> G5["G5 — Production<br/>release, decision log"]
    G5 --> OUT["✅ Delivered under<br/>professional responsibility"]

    classDef gate fill:#1F3864,stroke:#D9782D,stroke-width:2px,color:#FFFFFF
    classDef decision fill:#D9782D,stroke:#1F3864,stroke-width:2px,color:#FFFFFF
    classDef terminal fill:#0F1E38,stroke:#D9782D,stroke-width:2px,color:#FFFFFF
    classDef flag fill:#8A97AC,stroke:#1F3864,stroke-width:1px,color:#0F1E38

    class G0,G1,G2,G3,G3OK,G3IND,G4,G5 gate
    class Q,C decision
    class U,OUT terminal
    class LOCK,FLAG flag
