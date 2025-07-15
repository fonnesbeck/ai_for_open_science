**AI-Driven Model Divergence Analysis for Epidemic Projections**

**Project Team**

**Chris Fonnesbeck** (PyMC Labs) - Lead developer of PyMC probabilistic programming framework; **Katriona Shea** (Penn State) - Professor of Biology, expert in multi-model decision frameworks; **Cecile Viboud** (NIH Fogarty) - Senior Staff Scientist, architect of COVID-19 Scenario Modeling Hub; **Emily Howerton** (Princeton) - Postdoctoral Research Fellow, lead developer COVID-19 Scenario Modeling Hub; **Michael Runge** (USGS) - Research Ecologist, expert in structured decision making. Partnership with established US Scenario Modeling Hub (scenariomodelinghub.org).

**Executive Summary**

We propose developing an AI system that automates the identification and explanation of divergences between epidemic models, addressing a critical gap in public health decision-making. By providing Large Language Models (LLMs) with comprehensive access to model code, documentation, metadata, and outputs from established modeling hubs, our system will generate testable hypotheses about projection differences. This tool will transform how modelers and decision-makers understand multi-model ensembles, initially focusing on seasonal respiratory viruses where training data are rich. The project leverages existing infrastructure from the US Scenario Modeling Hub while introducing novel AI capabilities for model interpretation. All software will be released under open-source licenses (MIT/Apache 2.0).

**Critical Challenges**

Epidemic modeling faces a fundamental communication problem: when multiple models produce different projections for the same scenario, decision-makers lack clear explanations for these divergences, which hampers decision-making. Current challenges include:

* **Information Overload**: Complex parameter sets and nuanced assumptions about disease dynamics make manual comparison infeasible.

* **Hidden Assumptions**: Critical modeling decisions about immunity and behavioral dynamics are often buried in code or inadequately documented.

* **Time Constraints**: During active outbreaks, urgency prevents thorough investigation of model differences.

* **Technical Barriers**: Decision-makers lack the expertise to parse model code and isolate meaningful differences.

Manual comparison misses conceptual divergences in how models handle uncertainty, population heterogeneity, and intervention effects.

**Community Impact**

This project will serve three critical communities:

**Epidemic Modelers** will gain automated insights into model differences, enabling targeted improvements and clearer communication of assumptions.

**Public Health Decision-Makers** will receive plain-language explanations of model disagreements, supporting informed decisions based on context-appropriate assumptions.

**The Open Science Community** will benefit from a reusable framework for AI-driven model comparison applicable across scientific domains.

**Technical Approach**

Our AI system will employ a multi-stage pipeline with human-in-the-loop validation:

1. **Automated Model Analysis**: Parse epidemic model code and documentation using static analysis tools and LLM-powered code understanding. Extract model structure, parameters, and assumptions.

2. **AI-Driven Difference Detection**: Apply LLMs to identify structural and conceptual differences between models - from mathematical formulations to implementation choices. The system will categorize differences by type (e.g., population structure, transmission dynamics, intervention modeling).

3. **Hypothesis Generation**: Generate testable hypotheses about why projections diverge, grounded in epidemiological literature through retrieval-augmented generation (RAG). Hypotheses will be ranked by likely impact on projections.

4. **Community Validation Loop**: A critical advantage of this project is our direct connection to the Scenario Modeling Hub (SMH), an active community that meets regularly. We will:
   - Present LLM-generated summaries and hypotheses to modeling teams during SMH meetings
   - Collect structured feedback on accuracy and completeness of AI analysis
   - Use team validation to refine LLM prompts and improve output quality
   - Facilitate cross-team discussions about modeling choices and assumptions

5. **Iterative Improvement**: The feedback loop will enable:
   - Fine-tuning of LLM outputs based on expert validation
   - Creation of domain-specific evaluation metrics
   - Development of a curated dataset of validated model comparisons
   - Identification of common modeling patterns and divergence points

6. **Benchmark Development**: Create open benchmarks for evaluating model comparison tools, incorporating both automated metrics and human expert ratings from the SMH community.

This human-AI collaboration ensures reliable, actionable insights while fostering community trust. The AI analyzes complex code and identifies differences, while domain experts validate findings and provide context to improve analysis quality. This creates a virtuous cycle: modelers learn from each other's approaches through AI-generated comparisons, while the AI system continuously improves through expert feedback.

**Current Progress**

We build upon established infrastructure from the Scenario Modeling Hub (SMH), which coordinates projections from multiple modeling teams. SMH provided COVID-19 scenario projections to the CDC and White House throughout the pandemic and has expanded to provide real-time multi-model projections for flu and RSV.

Available resources include:
- Standardized model outputs from modeling teams
- Detailed metadata on model structure and assumptions
- Scenario specifications for COVID-19, influenza, and RSV
- Retrospective observations and model evaluations comparing projections to actual outcomes

While our primary focus is real-time decision-making, historical evaluation data presents additional opportunities to:
- Validate which model differences actually impact predictive performance
- Train the AI system to identify characteristics associated with accurate projections
- Create a "lessons learned" knowledge base for future outbreaks

This dual approach - real-time hypothesis generation for decision support and retrospective analysis for scientific understanding - positions our tool to serve both immediate public health needs and longer-term model improvement. The retrospective component could reveal which modeling choices (e.g., age structure, behavioral assumptions, spatial resolution) correlate with better performance under different epidemic conditions.

Our team's combined expertise spans infectious disease modeling (Shea, Viboud, Howerton), AI/ML systems (Fonnesbeck), and decision support tools (Runge), ensuring both technical excellence and practical utility.

**Funding Request**

We request $430,000 for an 18-month development grant to create a production-ready AI system for model divergence analysis:

**Technical Development (60%)**: \$260,000 - LLM integration, model parsing pipelines, hypothesis generation 
**Evaluation and Testing (25%)**: \$100,000 - COVID-19 retrospective analysis, user studies, validation 
**Dissemination and Training (15%)**: \$70,000 - Open-source release, workshops, benchmark development

**Milestones**:

* Months 1-6: Prototype system, initial model comparisons

* Months 7-12: Expanded testing, user feedback, benchmark v1.0

* Months 13-18: Public API, hub integration, documentation

**Open Science Commitment**: All software (MIT license), benchmarks, and documentation will be openly available via GitHub. Success metrics include adoption by modeling teams, validated hypothesis quality, and reduced time to understand model differences. Post-grant sustainability through integration with NIH/CDC infrastructure.
