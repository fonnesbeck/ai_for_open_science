# AI-Driven Model Divergence Analysis for Epidemic Projections

## Executive Summary

We propose developing an AI system that automatically identifies and explains sources of disagreement between epidemic models, addressing a critical gap in public health decision-making. By providing Large Language Models (LLMs) with comprehensive access to model code, metadata, abstracts, and outputs from established modeling hubs, our system will generate testable hypotheses about why different models produce divergent projections. This tool will transform how modelers and decision-makers understand multi-model ensembles, initially focusing on seasonal respiratory disease waves before expanding to other infectious diseases. The project leverages existing infrastructure from the MIDAS Network's scenario modeling hubs while introducing novel AI capabilities for model interpretation and comparison.

## Critical Challenges

Epidemic modeling faces a fundamental communication problem: when multiple models produce different projections for the same scenario, decision-makers lack clear explanations for these divergences. Current challenges include:

- **Information Overload**: Each model contains thousands of lines of code, complex parameter sets, and nuanced assumptions about disease dynamics, making manual comparison infeasible
- **Hidden Assumptions**: Critical modeling decisions about immune landscapes, waning immunity, and behavioral dynamics are often buried in code or inadequately documented
- **Time Constraints**: During active outbreaks, the urgency of decision-making prevents thorough investigation of model differences
- **Technical Barriers**: Decision-makers often lack the technical expertise to parse model code and identify meaningful differences

Traditional approaches have failed because the volume and complexity of information exceeds human analytical capacity. Manual model comparison typically focuses on easily quantifiable differences (e.g., parameter values) while missing conceptual divergences in how models handle uncertainty, population heterogeneity, or intervention effects.

## Community Impact

This project will serve three critical communities:

**Epidemic Modelers** will gain automated insights into how their models differ from others, enabling more targeted model improvements and clearer communication of assumptions. The AI system will highlight overlooked modeling choices and suggest areas for sensitivity analysis.

**Public Health Decision-Makers** will receive plain-language explanations of why models disagree, transforming incomprehensible technical differences into actionable insights. Instead of choosing between conflicting projections without understanding why they differ, officials can make informed decisions based on which assumptions best match their local context.

**The Open Science Community** will benefit from a reusable framework for AI-driven model comparison applicable across scientific domains. Our open-source tools, benchmarks, and methodologies will accelerate similar efforts in climate modeling, economic forecasting, and other fields relying on multi-model ensembles.

## Current Progress and Context

We build upon substantial existing infrastructure:

- **MIDAS Network Scenario Modeling Hubs**: Established repositories containing standardized model outputs, metadata, and scenario specifications from 7+ modeling teams
- **Proven Collaboration Framework**: Existing relationships with modeling teams who regularly contribute projections and engage in model comparison exercises
- **Initial Pilot Data**: COVID-19 and influenza projection data spanning multiple seasons, providing rich test cases for AI analysis

Preliminary explorations have shown that LLMs can successfully identify basic parameter differences between models when provided with structured metadata. However, developing systems that can parse model code, understand complex epidemiological concepts, and generate meaningful hypotheses requires dedicated development.

Our team combines expertise in:
- Infectious disease modeling and ensemble projection systems
- Natural language processing and prompt engineering
- Science communication and decision support tools
- Open-source software development and reproducible research

## Funding Request

We request $350,000 for an 18-month development grant to create a production-ready AI system for model divergence analysis:

**Technical Development (60%)**: $210,000
- LLM integration and prompt engineering framework
- Model code parsing and preprocessing pipelines  
- Hypothesis generation and validation systems
- User interface for querying model differences

**Evaluation and Testing (25%)**: $87,500
- Retrospective analysis of COVID-19 model divergences
- Prospective testing on seasonal influenza projections
- User studies with modelers and decision-makers
- Accuracy assessment of AI-generated hypotheses

**Dissemination and Training (15%)**: $52,500
- Open-source tool release and documentation
- Training workshops for modeling teams
- Integration with existing modeling hub infrastructure
- Development of reusable benchmarks and datasets

This investment will transform how the scientific community understands and communicates model uncertainty, with immediate applications in epidemic preparedness and broad potential across computational science domains.