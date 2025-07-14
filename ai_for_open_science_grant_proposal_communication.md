**AI-Powered Science Translation for Multi-Stakeholder Epidemic Communication**

**Project Team**

**Chris Fonnesbeck** (PyMC Labs) - Lead developer of PyMC probabilistic programming framework. **Katriona Shea** (Penn State) - Professor of Biology, expert in multi-model decision frameworks. **Cecile Viboud** (NIH Fogarty) - Senior Staff Scientist, architect of COVID-19 Scenario Modeling Hub. **Emily Howerton** (Princeton) - Postdoctoral Research Fellow, lead developer COVID-19 Scenario Modeling Hub. **Michael Runge** (USGS) - Research Ecologist, expert in structured decision making. Partnership with established US Scenario Modeling Hubs (scenariomodelinghub.org).

**Executive Summary**

We propose developing an AI system that automatically translates complex epidemic model outputs into actionable insights for public health professionals—epidemiologists and health officers who need to understand model implications without technical training—while enabling natural language exploration of model scenarios. By fine-tuning Large Language Models on successful science communication examples and integrating conversational interfaces, our system will bridge the critical gap between sophisticated modeling outputs and actionable insights for decision-makers. This tool will transform how epidemic projections are communicated, enabling non-technical users to design meaningful scenarios, explore uncertainty, and extract decision-relevant information. Building on infrastructure from the US Scenario Modeling Hub and leveraging our team's expertise in epidemic modeling and decision science, we will create an open-source platform that democratizes access to complex model insights. All software and outputs will be released under open-source licenses (MIT/Apache 2.0).

**Critical Challenges**

Epidemic modeling faces a fundamental communication crisis: sophisticated models produce outputs that remain inaccessible to those who need them most. Current challenges include:

* **Technical Language Barriers**: Model outputs use statistical terminology and uncertainty representations that non-experts cannot interpret, leading to misunderstandings and suboptimal decisions

* **One-Size-Fits-None Communication**: Current outputs fail to address the distinct needs of policymakers (who need decision points), healthcare providers (who need operational guidance), and the public (who need actionable behaviors)

* **Scenario Design Inefficiency**: Non-technical stakeholders waste effort designing redundant scenarios that fail to reveal decision-relevant differences, missing opportunities to explore meaningful alternatives

* **Static Reporting**: Traditional reports cannot adapt to user questions or provide interactive exploration of uncertainty and trade-offs

* **Lost Value of Information**: Current approaches fail to identify which scenarios would actually change decisions, limiting the practical impact of modeling efforts

**Community Impact**

This project will primarily serve **public health professionals**—epidemiologists, health officers, and program managers at state and local health departments who possess deep domain expertise but limited technical modeling background. These professionals need to:

* **Understand model assumptions** without reading code or mathematical formulations
* **Compare scenarios** to inform policy decisions without statistical training
* **Communicate findings** to leadership and communities in their jurisdictions
* **Design meaningful scenarios** that address local conditions and constraints
* **Access model insights quickly** during rapidly evolving outbreaks

Secondary beneficiaries include **epidemic modelers** who will gain clearer understanding of how public health professionals interpret and use their outputs, enabling more effective model design and communication.

**Technical Approach**

Our system architecture addresses each key deliverable through specific technical components:

**1. Automated Model Output Translation Pipeline**
We will develop a multi-stage processing system that ingests standardized model outputs from the Scenario Modeling Hub format (quantile-based projections across time horizons). The pipeline will: extract key metrics (peak timing, magnitude, uncertainty bounds); identify scenario differences using structured comparison algorithms; generate audience-specific narratives using LLMs fine-tuned on science communication corpora. Fine-tuning will use a curated dataset combining: peer-reviewed epidemiology papers with lay summaries; CDC communications matched with technical reports; successful public health messaging examples annotated by communication experts.

**2. Natural Language Query Interface**
Users will interact with model outputs through conversational interfaces built on open-source LLM frameworks. The system will: parse natural language questions ("What happens if we increase vaccination by 20%?"); map queries to available model scenarios or identify gaps requiring new runs; generate responses grounded in actual model outputs using retrieval-augmented generation (RAG); maintain conversation context to handle follow-up questions. The RAG implementation will index all model metadata, scenario definitions, and outputs to ensure responses are factually grounded.

**3. Interactive Visualization Generation**
We will create an AI-powered visualization system that: analyzes user expertise level through interaction patterns; adjusts visualization complexity accordingly (technical users see confidence intervals, public sees risk levels); generates accompanying text explanations calibrated to audience; produces multiple visualization options for A/B testing effectiveness. Visualizations will be built using Plotly for interactivity and will follow established best practices for uncertainty communication.

**4. Value of Information Analysis for Scenario Design**
To prevent redundant scenario exploration, we will implement: sensitivity analysis algorithms to identify parameters that most affect outcomes; decision-theoretic frameworks to quantify which scenarios would change decisions; AI-assisted scenario suggestion based on maximizing expected information gain; automated detection of scenario sets that are too similar to provide new insights. This component will help users design scenario comparisons that actually inform decisions rather than confirming existing beliefs.

**5. Public Health Professional Communication Framework**
The system will be optimized for public health professionals' specific needs: **Decision support summaries** that translate statistical outputs into policy-relevant thresholds (e.g., "Hospital capacity likely exceeded if no action taken within 2 weeks"); **Assumption explanations** in epidemiological terms rather than mathematical notation; **Uncertainty communication** using familiar public health concepts (e.g., "similar confidence to seasonal flu forecasts" rather than "95% prediction interval"); **Scenario comparison tools** that highlight practically meaningful differences rather than all parameter variations. Templates will be developed through iterative co-design with state and local health department staff.

**6. Quality Assurance and Validation**
All AI-generated content will pass through validation layers: factual accuracy checks against source model outputs; readability scoring for target audience level; expert review sampling for technical correctness; A/B testing framework for communication effectiveness. The system will log all transformations for audit trails and continuous improvement.

**Current Progress**

We build upon established infrastructure from the Scenario Modeling Hubs (SMH), which coordinates projections from multiple modeling teams and provided COVID-19 scenario projections to the CDC and White House throughout the pandemic. SMH has since expanded to provide real-time multi-model scenario projections for influenza and RSV. Available resources include: standardized model outputs and metadata from multiple respiratory disease modeling rounds; established data infrastructure for model comparison; documented scenario specifications and model assumptions. Our team brings combined expertise in epidemic modeling, probabilistic programming, decision science, and multi-model coordination. The proposed communication platform would address a documented gap in translating technical modeling outputs for diverse stakeholder audiences.

**Funding Request**

We request $350,000 for an 18-month development grant to create a production-ready AI communication system:

**AI Development and Training (50%)**: $175,000 - LLM fine-tuning, interface development, visualization tools
**Stakeholder Engagement and Testing (30%)**: $105,000 - User studies, CSTE collaboration, iterative design
**Platform Integration and Deployment (20%)**: $70,000 - Hub integration, API development, documentation

**Milestones**:

* Months 1-6: LLM fine-tuning, prototype interfaces, initial stakeholder feedback

* Months 7-12: Conversational agent development, visualization tools, CSTE pilot testing

* Months 13-18: Platform deployment, training materials, open-source release

**Open Science Commitment**: All software (MIT license), fine-tuned models, communication templates, and training data will be openly available via GitHub and HuggingFace. Success metrics include stakeholder comprehension scores, scenario design efficiency, decision quality improvements, and adoption by state health departments. Post-grant sustainability through integration with CDC/NIH communication infrastructure and continued CSTE partnership.