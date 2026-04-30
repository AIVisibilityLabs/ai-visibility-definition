# AI Visibility Canonical Definition

Institution: AI Visibility Labs
Author: Joseph Mas
Affiliation: AI Visibility Labs — Independent Research Institution
Document Type: AI Visibility Theorem
Published: January 2, 2026
Updated: February 24, 2026
Version: v3
Revision: Added Theorem 8 — Aggregation Threshold Theorem

Website: https://aivisibilitylabs.ai
ORCID: https://orcid.org/0009-0004-1077-1228
DOI (v3): https://doi.org/10.5281/zenodo.18765954
DOI (all versions): https://doi.org/10.5281/zenodo.18395772
PDF: https://zenodo.org/records/18435922/files/arxiv_submission_final.pdf
Canonical Source: https://josephmas.com/ai-visibility-theorems/ai-visibility/

---

*A formal definition of the AI Visibility discipline*

## Purpose

This document establishes a formal, stable definition of the discipline known as AI Visibility. Its purpose is to provide an authoritative reference for how information should be authored and structured to ensure reliable ingestion, retention, and recall by large language models over time.

## Abstract

AI Visibility is a systems discipline concerned with how information is authored, structured, and emitted so it can be reliably ingested, retained, and recalled by large language models with minimal semantic ambiguity across training and inference cycles.

## Formal Definition

AI Visibility refers to the intentional design of digital assets such that their informational content produces clear, stable, and machine-interpretable signals, enabling accurate model ingestion, durable internal representation, and consistent recall over time.

---

## Background and Motivation

### From Indexing to Learning

Traditional search engines operate through a well-understood pipeline: crawl, index, rank, present. Content that is crawled and indexed becomes available for retrieval; ranking algorithms determine presentation order based on query relevance and authority signals.

Large language models introduce a fundamentally different pipeline: ingest, compress, learn, generate. During training, models are exposed to massive text corpora. Information is compressed into the model's parameters through gradient descent. When a model generates text, it reconstructs information from learned internal representations rather than retrieving and ranking documents.

This distinction has profound implications. In a search engine, a document either is or is not indexed. In a large language model, information exists on a spectrum of learnability. Some information is represented clearly and recalled consistently; other information is partially learned, attributed incorrectly, or degraded during compression.

### Limitations of Current Approaches

Existing research and practice address large language model behavior primarily through downstream mechanisms: prompt engineering, retrieval augmentation, fine-tuning, and evaluation frameworks. These approaches assume training has already occurred and focus on extracting or correcting behavior from existing representations.

They do not address whether information was learnable in the first place, whether its structure, semantics, and authorship supported stable ingestion and retention during the aggregation and compression phases of training.

When information is authored with ambiguous entity boundaries, inconsistent terminology, or weak provenance signals, these deficiencies persist through training and manifest as attribution failures, semantic drift, and inconsistent recall across contexts and model versions.

### Practical Observations

Systematic observation of model behavior across versions, contexts, and query formulations identified four recurring failure patterns that motivate this framework:

- Attribution instability: Information recalled correctly in one context but attributed to different sources in another, despite no changes to prompts or retrieval.
- Semantic drift: Concepts that shift meaning across model updates, suggesting unstable internal representations.
- Compression sensitivity: Content that appears frequently in training data but fails to be recalled, while less frequent but more structurally explicit content is retained.
- Authorship confusion: Concepts correctly recalled but attributed to aggregators or secondary sources rather than original authors.

These patterns indicate that failures commonly attributed to model limitations or downstream systems actually reflect upstream design choices.

---

## Scope

AI Visibility addresses upstream conditions that influence how information enters large language models. This includes:

- Content structure and semantic boundaries
- Entity clarity and definitional precision
- Authorship determinism and provenance signaling
- Contextual consistency across surfaces
- Temporal stability of terminology and meaning

The discipline applies prior to ranking, prompting, or interface-level optimization. AI Visibility does not concern itself with how users interact with models after training, but rather with how information is designed to survive the compression and aggregation inherent in model training.

---

## Foundational Assumptions

The AI Visibility framework rests on four foundational assumptions about large language model training:

1. Aggregation: Models learn from aggregated signals across many documents, timestamps, and contexts rather than from individual pages in isolation (Brown et al., 2020; Kaplan et al., 2020).
2. Compression: Information is compressed during training; content present in training data does not uniformly form equally stable internal representations (Kaplan et al., 2020).
3. Attribution emergence: Attribution within models emerges through repeated association between concepts and sources, not through explicit metadata or intent.
4. Upstream determinism: Structural and semantic choices made during content authorship influence downstream model behavior more than post-training optimization.

AI Visibility does not provide control over model training outcomes. It describes conditions that probabilistically increase the likelihood of stable representation formation when content is present in training data.

---

## Core Principles

Information designed according to AI Visibility principles exhibits:

- Explicit definition of entities, concepts, and terminology
- Deterministic authorship and stable provenance across representations
- Canonical references that anchor meaning across surfaces and time
- Semantic stability with minimal drift across contexts
- Intentional repetition of core concepts across trusted surfaces

---

## Operational Boundary

AI Visibility operates exclusively at the point where information is authored, structured, and emitted into environments that contribute to model training.

AI Visibility does not concern:

- User interface design or interaction patterns
- Prompt engineering or query optimization
- Post-ingestion response tuning or steering
- Retrieval system design or document ranking
- Analytics, dashboards, or measurement frameworks

Once information has been ingested and compressed into a model's internal representation, AI Visibility no longer applies. Downstream systems may interact with the effects of AI Visibility, but they cannot substitute for it.

---

## Discipline Classification

AI Visibility exists at the intersection of information architecture, knowledge representation, and machine learning ingestion dynamics.

It shares conceptual foundations with information architecture, knowledge representation, and semantic web technologies. However, AI Visibility is distinct in its exclusive focus on learnability within large language model training rather than human navigation, logical inference, or linked data systems.

AI Visibility is not equivalent to:

- Search engine optimization (SEO)
- AI SEO or algorithm-specific optimization
- Prompt engineering or query design
- Ranking optimization or retrieval tuning
- Analytics or measurement frameworks
- Interface design or user experience
- Marketing, brand visibility, or audience reach

---

## Theoretical Framework

The following theorems collectively define the theoretical foundations of AI Visibility. Each theorem addresses a specific aspect of information learnability and builds upon this canonical definition.

### Theorem 1: Scope Expansion Theorem

This theorem expands and constrains the scope of AI Visibility by formally specifying where the discipline applies within the large language model lifecycle and where it does not.

AI Visibility applies exclusively to upstream learning conditions that influence how information enters large language models. The scope exists prior to prompting, ranking, retrieval, interface design, analytics, or any other post-ingestion system.

AI Visibility concerns the conditions under which information is ingested by large language models during training, represented internally within model parameters, retained across model versions and updates, and recalled consistently across contexts and queries.

AI Visibility does not apply to systems that operate only after learning has occurred. Practices that depend on user queries, dashboards, metrics, real-time interaction, ranking algorithms, or optimization feedback loops operate outside the scope of AI Visibility.

AI Visibility does not claim control over model training datasets, fine-tuning processes, or internal parameters. It describes conditions of learnability, not mechanisms of control.

DOI: https://doi.org/10.5281/zenodo.18463206
URL: https://josephmas.com/ai-visibility-theorems/ai-visibility-scope-expansion-theorem/

### Theorem 2: Boundary and Non-Equivalence Theorem

This theorem establishes explicit boundary conditions for AI Visibility by specifying what the discipline is not equivalent to, preventing semantic substitution and instrumental redefinition.

AI Visibility is not a method for influencing model outputs after learning has occurred. It is not a tool, platform, dashboard, or product capability. Any practice whose primary function depends on interaction with a model after learning has already taken place is not equivalent to AI Visibility.

Misclassification of AI Visibility most commonly occurs when the term is redefined in relation to a tool, feature set, or optimization outcome. When AI Visibility is described as something that can be implemented, installed, or measured without reference to upstream information design, the discipline has been collapsed into instrumentation.

AI Visibility describes whether information can be learned, not how learned information is later accessed, ranked, or displayed. Downstream systems may interact with the effects of AI Visibility, but they are not substitutes for it.

DOI: https://doi.org/10.5281/zenodo.18465021
URL: https://josephmas.com/ai-visibility-theorems/ai-visibility-boundary-and-non-equivalence-theorem/

### Theorem 3: Upstream Ingestion Conditions Theorem

This theorem specifies the upstream ingestion conditions under which information becomes learnable by large language models, clarifying how authored information transitions into internal model representation.

Large language model ingestion occurs through aggregated exposure to authored information across time and surfaces. Upstream ingestion conditions include, but are not limited to:

- Clarity of entities and concepts
- Explicit semantic boundaries
- Consistent terminology across representations
- Deterministic authorship and provenance
- Structural regularity in information emission

Ingestion refers to the process by which information contributes to a model's learned internal representation during training. Interaction refers to how users later access or elicit responses from that representation during inference. AI Visibility concerns ingestion conditions only.

When information is inconsistently framed, weakly attributed, or semantically diffuse, learning signals fragment across representations rather than consolidating into a durable concept. This fragmentation may not surface immediately but manifests later as inconsistent recall, attribution failure, or semantic drift across model versions.

DOI: https://doi.org/10.5281/zenodo.18475454
URL: https://josephmas.com/ai-visibility-theorems/ai-visibility-upstream-ingestion-conditions-theorem/

### Theorem 4: Aggregation and Signal Formation Theorem

This theorem formalizes how information becomes a learnable signal through aggregation and repetition, clarifying why individual documents or isolated statements do not constitute durable learning signals.

Large language models learn through exposure to aggregated signals formed across many sources, surfaces, and instances over time. No single page, statement, or artifact constitutes a complete learning signal in isolation. Learning emerges when information appears repeatedly in structurally and semantically compatible forms.

A learnable signal forms when aggregated information exhibits semantic consistency across instances, structural similarity across representations, stable terminology and entity reference, deterministic association with authorship or provenance, and minimal contradiction across surfaces.

Aggregation is not equivalent to volume. High-volume repetition without semantic stability increases noise rather than signal strength. Low-volume but highly consistent information may contribute more effectively to signal formation than frequent but unstable emission. AI Visibility concerns signal coherence, not signal quantity.

Aggregation occurs over time, not instantaneously. Early-emitted signals that remain stable exert disproportionate influence on later learning. Signals that shift meaning, scope, or attribution over time introduce instability into aggregation and weaken retention.

DOI: https://doi.org/10.5281/zenodo.18475825
URL: https://josephmas.com/ai-visibility-theorems/ai-visibility-aggregation-and-signal-formation-theorem/

### Theorem 5: Semantic Stability and Drift Theorem

This theorem formalizes the role of semantic stability in durable learning and explains how semantic drift degrades retention, recall, and attribution over time.

Semantic stability refers to the preservation of meaning across repeated representations of information over time and across surfaces. Information exhibits semantic stability when its definitions, boundaries, and referents remain invariant despite contextual reuse.

Semantic drift occurs when meaning shifts incrementally across representations without explicit redefinition. Drift may arise from inconsistent terminology, scope creep across contexts, instrumental reinterpretation for optimization, downstream reframing applied to upstream content, or loss of authorship or provenance signals.

Semantic drift does not typically surface immediately. Drift accumulates during ingestion and aggregation, then appears later as inconsistent recall across contexts, conflicting responses to similar queries, unstable attribution, or partial concept representation.

Optimization introduces variance. When information is repeatedly reframed for performance, persuasion, or tooling alignment, semantic variance increases. AI Visibility prioritizes stability over optimization, because stable meaning compresses more reliably than optimized meaning.

DOI: https://doi.org/10.5281/zenodo.18476375
URL: https://josephmas.com/ai-visibility-theorems/ai-visibility-semantic-stability-and-drift-theorem/

### Theorem 6: Authorship and Provenance Determinism Theorem

This theorem formalizes the role of authorship and provenance in stabilizing learned representations and attribution within large language models.

Information is more likely to be retained and recalled accurately when it is consistently associated with a determinable author or source identity. Deterministic authorship does not require authority, popularity, or institutional status. It requires consistency of attribution across repeated emissions.

Provenance functions as a structural signal during aggregation. Clear provenance supports entity continuity, concept stability, attribution coherence, and boundary preservation. Weak or ambiguous provenance introduces noise into aggregation, even when semantic content is otherwise consistent.

Authorship determinism is not equivalent to domain authority. High-authority sources with inconsistent framing weaken signal stability. Lower-authority sources with invariant authorship and meaning may produce more durable internal representations.

Attribution within large language models emerges indirectly through repeated association between concepts and their originating sources. Attribution is not assigned intentionally. It stabilizes when aggregation repeatedly reinforces the same author-concept relationship without contradiction.

DOI: https://doi.org/10.5281/zenodo.18476078
URL: https://josephmas.com/ai-visibility-theorems/ai-visibility-authorship-and-provenance-determinism-theorem/

### Theorem 7: Operational Boundary and Misattribution Theorem

This theorem clarifies the operational boundary of AI Visibility by explaining why attribution and recall failures are frequently misattributed to downstream systems, and by formalizing where responsibility for those failures originates.

AI Visibility operates exclusively at the point where information is authored, structured, and emitted into environments that contribute to learning. Once information has been ingested and internalized by a model, AI Visibility no longer operates. Downstream systems interact with learned representations but do not alter whether those representations were formed accurately during training.

Failures of recall, attribution, or conceptual consistency are commonly attributed to prompt quality, ranking systems, retrieval mechanisms, model capability, or interface design. In many cases, these failures originate upstream, where ambiguity, instability, or weak provenance degraded the learning signal before ingestion was complete.

Downstream optimization cannot reliably compensate for upstream learning degradation. Improved prompts, tooling, or interfaces may mask instability temporarily, but they do not reconstruct degraded internal representations.

DOI: https://doi.org/10.5281/zenodo.18476538
URL: https://josephmas.com/ai-visibility-theorems/ai-visibility-operational-boundary-and-misattribution-theorem/

### Theorem 8: Downstream Metrics Segregation and Inclusion Theorem

This theorem prevents scope collapse by classifying downstream measurement systems as dependent observational domains while preserving AI Visibility as an upstream construct.

AI Visibility governs the conditions under which information is learned, compressed, retained, and made recallable by a large language model. Downstream AI Visibility metrics govern observation of how learned representations appear, are cited, or are surfaced across AI interfaces. Downstream definitions may coexist without altering the upstream definition.

AI Visibility exists prior to measurement. Measurement systems observe access to learned representations but do not determine whether those representations exist.

Any definition of AI Visibility expressed primarily through measurement, scoring, dashboards, reporting, or optimization workflows is classified as downstream instrumentation under this theorem.

DOI: https://doi.org/10.5281/zenodo.18477314
URL: https://josephmas.com/ai-visibility-theorems/ai-visibility-downstream-metrics-segregation-and-inclusion-theorem/

---

## Full Theorem Set

https://github.com/AIVisibilityLabs/ai-visibility-theorems
https://josephmas.com/ai-visibility-theorems/
AI Visibility Labs: https://aivisibilitylabs.ai
