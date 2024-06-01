```mermaid
stateDiagram-v2
    [*] --> UNPLANNED: create issue
    UNPLANNED --> TODO: planned for next iteration
     TODO --> IN_PROGRESS: started work
     IN_PROGRESS --> REVIEW: work finished
     REVIEW --> DONE: successful review
     REVIEW --> IN_PROGRESS: more work required
     IN_PROGRESS --> TODO: issue became sidelined
     TODO --> DONE: issue closed in previous iteration
     TODO --> UNPLANNED: revision required
     DONE --> IN_PROGRESS: requirements not fully satisfied

     UNPLANNED --> UNPLANNED: updated issue
     TODO --> TODO: updated issue
     IN_PROGRESS --> IN_PROGRESS: updated issue
     REVIEW --> REVIEW: updated issue

