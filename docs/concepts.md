# The Atlas: Key Concepts

This page maps the core conceptual territory covered in the session.

---

## Territory 1: Structured Authoring and the DITA Ecosystem

DITA has been the dominant framework for structured technical content for 20 years (2005–2026). Its core contributions:

- **Typed topics** (task, concept, reference) that enforce rhetorical purpose at the structural level
- **Content reuse** via conref, keyref, and map-based assembly
- **Conditional processing** for variant output from a single source
- **Metadata-forward architecture** that makes content legible to downstream systems, including AI

**What DITA does well:** enterprise-scale, multi-channel, heavily governed content with significant reuse requirements.

**Where DITA struggles:** low-barrier adoption, small teams, agile content workflows, and contributors who aren't professional technical writers.

---

## Territory 2: Markdown and the Docs-as-Code Landscape

Markdown's ascendance in the 2010s was driven by developer adoption, not content strategy. Its strengths:

- Near-zero authoring barrier
- Native integration with version control (Git)
- Ecosystem of static site generators (MkDocs, Jekyll, Hugo, Docusaurus)
- Strong fit for docs-as-code CI/CD pipelines

**What Markdown does well:** developer documentation, open-source projects, small-to-medium content operations, rapid iteration.

**Where Markdown struggles:** semantic richness, enforced structure, complex reuse, and large-scale governance without additional tooling.

---

## Territory 3: Lightweight DITA as Border Crossing

LwDITA (OASIS standard, 2023) is frequently misread as "DITA made easier." It is more precisely a **bridge specification** — a formally defined interface between the DITA ecosystem and simpler serializations.

LwDITA's three serializations:

| Serialization | Format | Use Case |
|---|---|---|
| **XDITA** | XML | Structured authoring with DITA tooling (DITA-OT) |
| **HDITA** | HTML5 | Web-native authoring and CMS integration |
| **MDITA** | Markdown | Docs-as-code workflows with semantic DITA structure |

MDITA in particular enables content teams to author in Markdown while preserving DITA-compatible topic typing and map-based assembly — a genuine border crossing, not a downgrade.

---

## Territory 4: AI and the Emergence of Intentio Algorithmi

AI systems in content workflows are not passive processors. They exert an interpretive force on content — selecting, transforming, summarizing, and generating based on patterns learned from training data and shaped by system prompts and retrieval architectures.

We propose extending Umberto Eco's tripartite model of textual intentionality:

| Intentio | Source | Description |
|---|---|---|
| *Intentio auctoris* | Author | What the author meant to communicate |
| *Intentio operis* | Text | What the text itself communicates independent of authorial intent |
| *Intentio lectoris* | Reader | What the reader brings to the text |
| ***Intentio algorithmi*** | **AI system** | **What the AI system "reads into" content based on its architecture, training, and task** |

**Implications for ContentOps:** structured content with explicit semantics (typed topics, metadata, clear hierarchy) is more legible to AI systems and produces more predictable *intentio algorithmi* outcomes. Unstructured or ambiguous content increases the variance of AI interpretation.

---

## Territory 5: ContentOps as Infrastructure

ContentOps is the discipline that makes all other territories sustainable at scale. Key components:

- **Governance:** who owns content, how it is approved, how it is retired
- **Pipeline architecture:** how content moves from source to delivery channel
- **Metadata strategy:** what information travels with content to make it findable and reusable
- **Toolchain decisions:** how authoring, review, build, and publish systems are connected

ContentOps decisions made early constrain (or enable) what is possible when AI systems, new formats, or scale requirements emerge later.
