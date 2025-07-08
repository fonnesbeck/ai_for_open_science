# AI-Driven Model Divergence Analysis for Epidemic Projections

## Project Team

**Chris Fonnesbeck** (PyMC Labs) - Lead developer of PyMC probabilistic programming framework. **Katriona Shea** (Penn State) - Professor of Biology, expertise in multi-model decision frameworks. **Cecile Viboud** (NIH Fogarty) - Senior Staff Scientist, architect of COVID-19 Forecast Hub. **Emily Howerton** (Princeton) - C3.ai Fellow, lead developer COVID-19 Scenario Modeling Hub. **Michael Runge** (USGS) - Research Ecologist, expert in structured decision making. Partnership with established MIDAS Network Scenario Modeling Hubs (covid19scenariomodelinghub.org).

## Executive Summary

We propose developing an AI system that automates the identification and explanation of sources of disagreement between epidemic models, addressing a critical gap in public health decision-making. By providing Large Language Models (LLMs) with comprehensive access to model code, metadata, and outputs from established modeling hubs, our system will generate testable hypotheses about why different models produce divergent projections. This tool will transform how modelers and decision-makers understand multi-model ensembles, initially focusing on seasonal respiratory disease waves before expanding to other infectious diseases. The project leverages existing infrastructure from the MIDAS Network's scenario modeling hubs while introducing novel AI capabilities for model interpretation and comparison. All software and outputs will be released under open-source licenses (MIT/Apache 2.0).

## Critical Challenges

Epidemic modeling faces a fundamental communication problem: when multiple models produce different projections for the same scenario, decision-makers lack clear explanations for these divergences. Current challenges include:

- **Information Overload**: Complex parameter sets and nuanced assumptions about disease dynamics make manual comparison infeasible
- **Hidden Assumptions**: Critical modeling decisions about immunity and behavioral dynamics are often buried in code or inadequately documented
- **Time Constraints**: During active outbreaks, urgency prevents thorough investigation of model differences
- **Technical Barriers**: Decision-makers lack the expertise to parse model code and identify meaningful differences

Manual comparison misses conceptual divergences in how models handle uncertainty, population heterogeneity, and intervention effects.

## Community Impact

This project will serve three critical communities:

**Epidemic Modelers** will gain automated insights into how their models differ from others, enabling targeted improvements and clearer communication of assumptions.

**Public Health Decision-Makers** will receive plain-language explanations of why models disagree, helping officials make informed decisions based on which assumptions best match their local context.

**The Open Science Community** will benefit from a reusable framework for AI-driven model comparison applicable across scientific domains including climate and economic modeling.

## Technical Approach

Our AI system will employ a multi-stage pipeline: (1) parse epidemic model code and documentation using automated tools, (2) apply LLMs to identify structural and conceptual differences between models, (3) generate testable hypotheses about why projections diverge, and (4) create open benchmarks for evaluating model comparison tools. The system will leverage retrieval-augmented generation (RAG) to ground hypotheses in epidemiological literature and validate outputs against known model behaviors.

## Current Progress

We build upon established infrastructure from the MIDAS Network Scenario Modeling Hubs, which coordinate projections from multiple modeling teams. Available resources include standardized model outputs, metadata, and scenario specifications for COVID-19 and influenza. Preliminary explorations show LLMs can identify parameter differences when provided structured metadata. Our team's combined expertise spans infectious disease modeling, AI/ML systems, and decision support tools.

## Funding Request

We request $350,000 for an 18-month development grant to create a production-ready AI system for model divergence analysis:

**Technical Development (60%)**: $210,000 - LLM integration, model parsing pipelines, hypothesis generation
**Evaluation and Testing (25%)**: $87,500 - COVID-19 retrospective analysis, user studies, validation
**Dissemination and Training (15%)**: $52,500 - Open-source release, workshops, benchmark development

**Milestones**: 
- Months 1-6: Prototype system, initial model comparisons
- Months 7-12: Expanded testing, user feedback, benchmark v1.0
- Months 13-18: Public API, hub integration, documentation

**Open Science Commitment**: All software (MIT license), benchmarks, and documentation will be openly available via GitHub. Success metrics include adoption by modeling teams, validated hypothesis quality, and reduced time to understand model differences. Post-grant sustainability through integration with NIH/CDC infrastructure.