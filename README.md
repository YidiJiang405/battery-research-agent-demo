# Battery Research Agent Demo

This repository presents a demo workflow for AI-assisted lithium-ion battery cathode materials research, focusing on Li-rich Mn-based layered oxide cathodes.

## Project Overview

I am developing an AI-assisted research workflow for battery materials science. The workflow is designed to support literature analysis, experimental data processing, mechanism reasoning, and manuscript/figure preparation for Li-rich Mn-based cathode materials.

The project is not a general chatbot. It is a vertical research Agent workflow built around real materials science problems, especially the analysis of electrochemical behavior, structural evolution, surface/interface chemistry, oxygen redox, and advanced characterization data.

## Core Pain Points

Battery materials research involves highly heterogeneous data. A single research project may include:

- Charge/discharge curves
- dQ/dV analysis
- GITT analysis
- Variable-rate CV and b-value analysis
- In situ XRD lattice evolution
- PDF/NPD experiment planning and refinement support
- XPS O 1s and Mn 3s interpretation
- Solid-state 7Li NMR peak shift and broadening analysis
- DEMS gas evolution analysis
- Literature evidence from high-level journals

Manually connecting these data into a consistent scientific mechanism is time-consuming and error-prone. The main pain point is not only data processing, but also building a self-consistent link between structure, electrochemistry, surface chemistry, oxygen redox behavior, and material performance.

## Agent Workflow

The current workflow contains four main Agent modules.

### 1. Literature Agent

The Literature Agent reads and summarizes papers from journals such as Advanced Materials, Nature Communications, JACS, Angewandte Chemie, Energy & Environmental Science, and Advanced Energy Materials.

It extracts:

- Core scientific question
- Experimental design
- Characterization strategy
- Figure logic
- Mechanistic conclusion
- Writing strategy for high-level papers

### 2. Data Agent

The Data Agent assists with experimental data processing and summary generation. It works with Python scripts, semi-automated analysis workflows, and manual verification.

Typical tasks include:

- dQ/dV peak extraction
- GITT data organization
- Variable-rate CV kinetic analysis
- In situ XRD lattice parameter evolution
- PDF/NPD testing requirement organization
- XPS peak component summary
- Solid-state NMR peak position and broadening analysis

### 3. Mechanism Critic Agent

The Mechanism Critic Agent performs long-chain reasoning and cross-checking. It evaluates whether the proposed mechanism is consistent with experimental data and literature evidence.

It checks questions such as:

- Whether structural evolution agrees with electrochemical behavior
- Whether oxygen redox interpretation is overclaimed
- Whether surface/interface chemistry can explain performance improvement
- Whether alternative explanations or experimental artifacts exist
- Whether additional control experiments are needed

### 4. Writing and Figure Agent

The Writing and Figure Agent converts analyzed results into research outputs, including:

- Figure captions
- Result and discussion paragraphs
- Supplementary information structure
- Beamtime proposal text
- Experimental requirement documents
- Manuscript logic and story line

## Example Research Scenarios

This workflow has been used in several real PhD research scenarios, including:

- Surface/interface modification of Li-rich Mn-based cathode materials
- First-cycle lattice evolution analysis from in situ XRD
- PDF/NPD experiment planning and refinement requirement preparation
- Solid-state 7Li NMR peak shift and broadening analysis
- ICP sample digestion and elemental quantification planning
- XPS O 1s and Mn 3s interpretation across electrochemical states
- DEMS oxygen release analysis during high-voltage charging
- Manuscript introduction and mechanism narrative development

## Core Logic Flow

The workflow follows a long-chain research reasoning process:

```text
Literature Input
    ↓
Literature Agent
    ↓
Experimental Data Input
    ↓
Data Agent
    ↓
Mechanism Critic Agent
    ↓
Writing and Figure Agent
    ↓
Output:
Figures / Tables / Discussion / SI Framework / Beamtime Proposal / Experimental Plan
