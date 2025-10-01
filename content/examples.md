---
title: "Examples & Use Cases"
date: 2025-09-17
draft: false
layout: "topic"
hero: /images/copan_lpjml_examples.png
---

<div style="display: flex; align-items: center; gap: 10px; flex-wrap: wrap; margin-top: -30px; margin-bottom: -20px;">
  <div style="flex: 1; min-width: 300px;">
    <h3 style="margin: 2;"><em>Get inspired and start drafting your own social-ecological World-Earth models.</em></h3>
  </div>
  <div style="flex-shrink: 0;">
    <img src="/images/logo_med.svg" alt="pycopanlpjml" style="width: 250px; height: auto;">
  </div>
</div>

## Model Gallery

So far copan:LPJmL is still in its early stages of deployment. 
Currently we have three main example applications that have been developed.
They are part of the corresponding description paper that is currently under
review at the Journal of Geoscientific Model Development (GMD). These are:

1. **🤖 InSEEDS** - an agent-based model for social-ecological transitions
2. **📅 Crop Calendar** - a rule-based model for adaptive growing seasons
3. **🧠 LLM Fertilization** - an AI-enhanced decision-making approach

### 🤖 InSEEDS

**InSEEDS** simulates how farmers adopt conservation tillage practices through social networks and environmental feedback. It's the first model to simulate coevolutionary social-ecological dynamics through closed feedback loops.

**What it does:** Individual farmer agents decide whether to switch from conventional to conservation tillage based on social interactions, environmental observations, and performance evaluation. Their decisions are based on the Theory of Planned Behavior.

**How it works:** Each farmer belongs to one of two agent-functional types - "traditionalists" who stick to conventional methods, or "pioneers" who are more likely to try new practices. They observe soil carbon levels and crop yields from their fields and learn from nearby farmers through social networks.

**Key features:**
- Closed feedback loops between social and ecological processes
- Bidirectional coupling - farmer decisions affect environment, environmental feedback influences decisions
- Social networks influence adoption patterns  
- Spatial spreading emerges from local interactions
- Global patterns show irreversible coevolutionary transitions

<div style="text-align: center; margin: 1rem 0;">
  <img src="/images/inseeds_scheme.png" alt="InSEEDS Scheme" style="max-width: 80%; height: auto; max-height: 400px;">
</div>

**Results:** Conservation tillage spreads geographically through social learning, creating synergistic effects between soil health and productivity. In Kazakhstan, adoption started in the south and spread northeastward, demonstrating how local decisions drive large-scale coevolutionary transformations.


### 📅 Crop Calendar

**Crop Calendar** adapts farming schedules to climate change in real-time using rule-based logic.

**What it does:** Automatically adjusts when farmers should plant and harvest crops based on changing temperature and precipitation patterns.

**How it works:** Uses a 10-year rolling window of climate data to determine optimal sowing and harvest dates. Rules respond to temperature and precipitation thresholds to switch crop varieties or adjust timing. This enables runtime adaptation without requiring pre-computed scenarios.

**Key features:**
- No pre-computed scenarios needed - adapts during simulation
- Handles multiple crop types (maize, spring/winter cereals)
- Global implementation using efficient vectorized operations
- Climate-responsive decision rules

<div style="text-align: center; margin: 1rem 0;">
  <img src="/images/crop_calendar_scheme.png" alt="Crop Calendar Scheme" style="max-width: 80%; height: auto; max-height: 350px;">
</div>

**Results:** Earlier planting in temperate regions, variety switching in response to warming, and region-specific adaptation patterns. Successfully reproduces established methods while integrating with other models.


### 🧠 LLM Fertilization

**LLM Fertilization** tests whether AI can make realistic farming decisions by using Large Language Models as virtual farmers.

**What it does:** LLM-based agents decide how much nitrogen fertilizer to apply to their crops based on location, crop type, historical performance, and current conditions.

**How it works:** Each AI farmer receives detailed information about their land, crops, and past fertilizer use. They make decisions using natural language reasoning and explain their choices.

**Key features:**
- AI agents reason about farming decisions like humans
- Each agent responds differently based on local conditions
- Agents explain their reasoning in natural language
- Adaptive responses to changing yields and conditions

<div style="text-align: center; margin: 1rem 0;">
  <img src="/images/llm_fertilization_scheme.png" alt="LLM Fertilization Scheme" style="max-width: 80%; height: auto; max-height: 320px;">
</div>

**Results:** AI farmers show realistic behavior - they increase fertilizer when yields are low, stabilize applications when conditions improve, and adapt to local needs. This proves LLMs can capture complex decision-making in agricultural systems.


## Modelling Capabilities

copan:LPJmL supports **six core modeling paradigms** that can be combined and adapted to address diverse research questions:

| **Paradigm** | **Application Domain(s)** | **Representative Examples** |
|--------------|-------------------------|----------------------------|
| **🤖 Agent-Based Models (ABMs)** | Socio-ecological systems, land-use change and adaptation, household and farmer decision-making, socio-hydrological systems | InSEEDS: heterogeneous farmer agents with LPJmL feedback; household-level farming responses; social-hydrological studies |
| **📋 Rule-Based Models (RBMs)** | Systems following rule-based logic, agricultural management and land use, institutional guidelines | Crop Calendar: climate-responsive adaptation; land use allocation; crop rotation and fallow scheduling |
| **⚡ Optimization Models** | Economic land and resource optimization, yield and input efficiency, food security and environmental trade-offs | MAgPIE, GLOBIOM, IMAGE: water and nutrient optimization; land-based mitigation strategies |
| **🔄 Dynamical System Models** | System-level feedbacks and tipping dynamics, coupled socio-environmental processes, bioeconomic models | Tipping point and regime shift models; socio-epidemic models; human-climate interaction models |
| **📊 Data-Driven Models** | Emulators, pattern discovery, scenario validation and calibration, remote-sensing based approaches | Statistical crop yield emulators; surrogate models; remote-sensing integration |
| **🧠 LLM-Enhanced Models** | Decision emulation, stakeholder reasoning, adaptive behavior | LLM-based farmer management decisions; LLM agents as institutional policy-makers |

## Research Applications

copan:LPJmL can model complex interactions between people and land systems across multiple scales.

**Main research areas:**
- 🌱 Land-use change and farming practices
- 🌡️ Climate adaptation strategies
- ⚡ Food-water-energy systems
- 🏛️ Policy and governance scenarios
- 🔄 Social-ecological system transitions

**Multi-layer systems** can be modeled - for example, supply chains where farmers interact directly with land, while food processors and consumers are connected through social networks.

## Key Advantages

**Modular design** allows researchers to:
- Combine different modeling approaches in one framework
- Scale from local to global perspectives
- Integrate multiple disciplines and stakeholder views
- Adapt to new research challenges

This makes copan:LPJmL well-suited for modeling human-nature interactions across scales.

## Getting Started

Ready to explore these applications? 

📚 **Documentation**: Visit our [comprehensive documentation](https://copanlpjml.pik-potsdam.de) for detailed guides, tutorials, and API references.

🔧 **Code Examples**: Browse our [GitHub repository](https://github.com/pik-copan/pycopanlpjml) for implementation examples and sample models.

🤝 **Community**: Join our user community for support, collaboration, and sharing your own applications.
