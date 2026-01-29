# Goal Kick Tactical Analysis in Professional Football

## Overview

This project analyzes goal kick situations in professional football using **StatsBomb event data**.  
The analysis focuses on **tactical decision-making**, combining contextual variables, player positioning, and execution outcomes. All matches analyzed correspond to **Bayer Leverkusen during the 2023/2024 season**.  

The project was developed as part of a **Bachelor’s Thesis in Sports Science and Data Analysis**. Its aim is to provide a **systematic and data-driven approach** to evaluate goal kick effectiveness and support tactical decision-making.

---

## Objectives

- Design an automated tool to detect goal kick events and extract contextual data.
- Evaluate tactical decisions using a **rule-based model** combining WHEN (context) and HOW (execution) criteria.
- Generate actionable insights on team positioning, player interactions, and decision quality.
- Explore patterns influencing goal kick outcomes to support coaching interventions.

---

## Data

- **Source:** StatsBomb Open Data  
- **Team:** Bayer Leverkusen  
- **Season:** 2023/2024  

> **Note:** Raw event data is not included in this repository due to licensing restrictions. Processed datasets and results are shared to illustrate the analysis workflow.

---

## Methodology

1. **Event Filtering & Feature Engineering**
   - Identify goal kick events.
   - Extract contextual variables: pressure, player positioning, distance, pass type, teammate proximity.

2. **Rule-Based Tactical Model**
   - **WHEN:** Define contextual conditions for the goal kick (e.g., space, opponent pressure, teammate configuration).  
   - **HOW:** Specify execution type (short, medium, long).  
   - **Scoring Function:** Quantitatively evaluates the tactical quality of each goal kick.

3. **Exploratory & Visual Analysis**
   - Descriptive statistics for goal kick distribution, execution types, and outcomes.
   - Visualizations of player positioning and relationships between teammates’ proximity and tactical scores.

---

## Key Insights

- Goal kicks with higher teammate density near the goalkeeper tend to receive **higher tactical scores**.
- The automated scoring system captures both **quantitative and contextual patterns**, supporting tactical evaluation.
- Structured build-up from the back is preferred, with short and medium passes showing more consistent outcomes.
- Match pressure, game pace, and prior goal kick quality influence tactical effectiveness.
- Visual analyses illustrate the **relation between player positioning and goal kick quality**, highlighting key decision-making factors.

---

## Usage

1. Explore notebooks in the `notebooks/` folder for step-by-step analysis.  
2. Review visualizations in the `figures/` folder to understand tactical patterns.  
3. Reference processed datasets in `data/` for custom analyses.

---

## License

This repository is for **educational and research purposes**. Data and results are derived from StatsBomb Open Data under their licensing terms.
