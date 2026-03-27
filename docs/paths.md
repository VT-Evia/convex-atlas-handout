# Suggested Paths

Not all organizations are at the same point on the map. Use these paths as starting points for finding your route.

---

## Path A: "We're a DITA shop. Where does AI fit?"

**Starting point:** Established DITA or component CMS (CCMS) environment, professional technical writers, existing governance.

**Recommended route:**

1. **Audit your metadata.** AI systems work best with content that has explicit, consistent metadata. DITA's architecture supports this, but only if your metadata is actually populated and governed.
2. **Evaluate your output architecture for AI readiness.** Is your content published in formats that AI retrieval systems can parse (HTML, chunked topics, structured JSON)? If output is PDF-first, AI integration will be limited.
3. **Introduce LwDITA MDITA for contributor onboarding.** Subject matter experts and developers who resist XML authoring can contribute via MDITA with tooling (VS Code + DITA-OT) that maintains DITA compatibility.
4. **Define your *intentio algorithmi* policy.** What should AI systems do with your content? Summarize? Answer questions? Generate variants? Define this before choosing tooling.

**Watch out for:** assuming that "structured content = AI-ready content." Structure is necessary but not sufficient — consistent metadata and deliberate output architecture matter equally.

---

## Path B: "We're docs-as-code in Markdown. How do we scale?"

**Starting point:** Developer documentation, Git-based workflow, static site generator, small-to-medium team.

**Recommended route:**

1. **Introduce MDITA conventions before you need them.** Adding DITA-compatible YAML front matter and topic-type conventions to your Markdown now costs almost nothing and enables DITA-OT processing later.
2. **Define your reuse strategy.** Markdown's native reuse mechanisms (includes, snippets) vary by static site generator and are not portable. Consider whether LwDITA's map-based reuse is worth adopting.
3. **Build governance into your pipeline.** Linting, style checking, and metadata validation can be added to CI/CD workflows (GitHub Actions, etc.) to enforce structure without changing authoring tools.
4. **Treat AI as a pipeline stage.** AI-assisted authoring, review, and summarization can be integrated into your existing docs-as-code pipeline as steps in a workflow, not as replacements for the workflow.

**Watch out for:** Markdown fragmentation. Every SSG has a different Markdown flavor, shortcode syntax, and front matter schema. Standardize early.

---

## Path C: "We're starting from scratch. What should we build?"

**Starting point:** New content operation, greenfield toolchain decision, or significant migration/modernization.

**Recommended route:**

1. **Start with ContentOps, not tools.** Identify your content types, reuse requirements, delivery channels, and governance model before selecting authoring tools or formats.
2. **Choose your format based on your contributor profile.** If contributors are professional technical writers at scale: DITA. If contributors are developers or mixed: MDITA or Markdown with LwDITA conventions. If contributors are non-technical: HDITA or a headless CMS with structured content modeling.
3. **Design for AI from the start.** Build metadata schemas, topic typing, and output formats with AI legibility in mind. This is significantly easier to do at the start than to retrofit.
4. **Build a CI/CD pipeline from day one.** Even a simple GitHub Actions workflow that builds and validates your content on every commit establishes the operational discipline that scales.

**Watch out for:** over-engineering for scale you don't have yet. Start with the simplest toolchain that meets your current needs and has a clear upgrade path.

---

## Path D: "We need to make the case for structured authoring to leadership."

**Starting point:** Individual contributor or team lead who understands the value of structure but needs to build organizational support.

**Recommended route:**

1. **Use AI as the bridge argument.** Leadership conversations about DITA and structured authoring are easier when framed around AI readiness. "Our content needs to be structured so AI systems can use it reliably" lands differently than "we need XML."
2. **Start with a pilot.** A single content type (release notes, API docs, onboarding guides) migrated to a structured format with measurable outcomes is more persuasive than a comprehensive proposal.
3. **Quantify the cost of unstructured content.** Translation costs, search failure rates, duplicate content, and inconsistent AI outputs are all measurable costs of unstructured content operations.
4. **Connect to existing initiatives.** ContentOps arguments land better when connected to ongoing programs: AI adoption, accessibility compliance, product localization, or developer experience.

**Watch out for:** making the argument on tool features rather than business outcomes.
