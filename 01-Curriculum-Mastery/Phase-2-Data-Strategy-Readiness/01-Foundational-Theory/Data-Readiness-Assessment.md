# Data Readiness Assessment (DRA)

The Data Readiness Assessment (DRA) is a systematic evaluation conducted by Business Analysts to determine if an organization's data infrastructure can support specific AI objectives.

## The Five Dimensions of Data Readiness

1.  **Availability (Can we access it?)**:
    *   **Metric**: Is the data siloed? Are there APIs or connectors to retrieve it?
    *   **Concern**: Data accessibility for training or inference.
2.  **Quality (Is it accurate?)**:
    *   **Metric**: Completeness, consistency, timeliness, and uniqueness of data.
    *   **Concern**: "Garbage in, Garbage out" (GIGO).
3.  **Volume (Is there enough?)**:
    *   **Metric**: Historical depth and diversity of samples.
    *   **Concern**: Statistical significance for predictive models.
4.  **Labeling (Is it annotated?)**:
    *   **Metric**: Availability of ground-truth labels for supervised learning.
    *   **Concern**: High cost of human-in-the-loop (HITL) labeling.
5.  **Lineage (Do we know where it comes from?)**:
    *   **Metric**: Tracking data from source to model.
    *   **Concern**: Compliance, auditability, and debugging.

## Assessment Matrix

| Dimension | Critical | Adequate | Poor |
| :--- | :--- | :--- | :--- |
| **Availability** | Real-time APIs | Batch exports | Manual spreadsheets |
| **Quality** | Cleansed & Validated | Some duplicates | Inconsistent formats |
| **Lineage** | Fully documented | Partially tracked | Unknown origin |

## Outcome: The Data Roadmap
Based on the DRA, the BA recommends data cleaning, ingestion pipelines, or third-party data acquisition before model development begins.
