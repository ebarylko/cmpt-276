```mermaid
stateDiagram-v2
    [*] --> UNPLANNED: create issue
    UNPLANNED --> TODO: planned for next iteration
     UNPLANNED --> IN_PROGRESS: started work
     TODO --> IN_PROGRESS: started work
     IN_PROGRESS --> REVIEW: work finished
     REVIEW --> [*]: successful review
     REVIEW --> IN_PROGRESS: more work required
     IN_PROGRESS --> TODO: delayed
     TODO --> REVIEW: work finished
     TODO --> UNPLANNED: revision required
     UNPLANNED --> REVIEW: 
     IN_PROGRESS --> UNPLANNED: 
     ```
