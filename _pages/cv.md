---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[Download my CV (PDF)]({{ base_path }}/files/Resume.pdf)

Education
======
* Ph.D. in Operations Research, Massachusetts Institute of Technology, 2028 (expected)
  * Advisor: Prof. Alexandre Jacquillat
  * GPA: 5.0/5.0
  * Coursework: Machine Learning with Optimization, Probability Theory, Multimodal AI
* B.S.E. in Operations Research and Financial Engineering, Princeton University, 2022
  * Magna cum laude, GPA: 3.92/4.0
  * Senior thesis: *Managing Uncertainties in the Development of CO₂ Capture, Transport, & Storage Infrastructure: A Scenario Optimization Approach*
  * Coursework: Regression & Applied Time Series, Econometrics, Analysis of Big Data

Research Experience
======
* Sep 2024 – Present: Graduate Research Assistant
  * MIT Operations Research Center, Cambridge, MA
  * **Experimental evaluation of LLM agents.** Designed a replicable and scalable methodology to evaluate LLM agents for interactive combinatorial optimization and decision support. Built agents in LangGraph that call optimization solvers through MCP tool servers, varying tool access, prompt engineering, and solver support across 14 designs, along with a Python harness to evaluate them and run statistical tests.
  * **Large-scale optimization for election planning.** Built MIP models for polling-place location, voter assignment, and contiguous precinct redistricting for five Montana counties, reducing average voter travel burden by 5–12%. Developed an exact logic-based Benders decomposition for hierarchical districting and facility location, accelerated by a spanning-tree DP oracle and a new family of problem-specific cuts, that solves instances 100x larger than previous methods. Prototyped an interactive planning tool for election officials to explore, visualize, and generate optimized plans.

* May 2020 – May 2022: Undergraduate Research Assistant
  * Princeton University, Princeton, NJ
  * Performed sensitivity analysis with and refined a linear programming capacity expansion model that co-optimizes investment and dispatch across electricity, fuels, and end-use demand over multi-decade horizons.

Industry Experience
======
* Aug 2022 – Aug 2024: Supply Chain Analyst, promoted to Senior Analyst
  * Wood Mackenzie, Boston, MA
  * Built regression and time-series forecasting models on large-scale client transaction data and market indicators, producing price-benchmark distributions, cost models, and forecasts for procurement and investment decisions.
  * Built Python tools to collect, clean, and mine a proprietary transaction database, using NLP on unstructured records; benchmarked client spend against market trends to identify multi-million-dollar savings.
  * Owned analytics delivery for utility, oil & gas, and natural-resources clients, presenting findings to procurement and finance leadership.

Publications and Working Papers
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

{% if site.talks.size > 0 %}
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
{% endif %}

{% if site.teaching.size > 0 %}
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% endif %}

Skills
======
* **Languages:** Python, SQL, Julia, Java
* **Optimization:** Gurobi, CPLEX, JuMP; integer, robust, and stochastic optimization
* **Machine learning:** Deep learning, reinforcement learning, fine-tuning foundation models, NLP; PyTorch, scikit-learn, pandas, NumPy
* **Statistics:** Time-series forecasting, regression, statistical inference, hypothesis testing, experimental design
* **Data and visualization:** Tableau, SQL, matplotlib, seaborn, folium, GeoPandas
