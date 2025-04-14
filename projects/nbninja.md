---
layout: project
type: project
image: images/nbninja_thumbnail.png
title: NBNinja - Automatic 2D Layouts for Jupyter Notebooks
permalink: projects/nbninja
# All dates must be YYYY-MM-DD format!
date: 2023-05-25
labels:
  - Python
  - Abstract Syntax Trees
  - Graph Theory
  - Code Analysis
  - Research
summary: Developed NBNinja, a Python tool that automatically restructures linear Jupyter Notebooks into optimal 2D spatial layouts by analyzing code dependencies through Abstract Syntax Trees, identifying logical breakpoints, and constructing dependency graphs with networkx.
---

<img class="ui rounded image" src="../images/nbninja_visualization.png">*Visualization of a notebook dependency graph showing how NBNinja identifies optimal split points for 2D layouts.*

## Project Overview

As part of my Master's thesis on enhancing collaborative data science environments, I developed NBNinja, a Python tool that automatically restructures linear Jupyter Notebooks for optimal 2D spatial layouts. This research addressed a fundamental challenge in data science collaboration: the inherently linear nature of notebooks that doesn't align with the non-linear thinking process of data exploration.

## Technical Implementation

NBNinja employs sophisticated code analysis techniques:
- **AST Parsing**: Transforms notebook code into Abstract Syntax Trees to analyze structure
- **Dependency Analysis**: Identifies variable and function dependencies between cells
- **Graph Construction**: Builds a dependency graph using networkx to represent relationships
- **Minimum Cut Identification**: Finds optimal split points that minimize cross-connections
- **Layout Suggestion**: Proposes logical multi-column arrangements to reduce clutter

## Research Validation

I validated the effectiveness of this approach through:
- **Large-Scale Analysis**: Testing on nearly 800 public notebooks from diverse sources
- **Structural Metrics**: Measuring improvements in cohesion and coupling compared to standard methods
- **Visualization Tools**: Developing optional interactive graph visualization for explainability
- **Academic Presentation**: Demonstrating results at research venues

## Technical Innovations

The project introduced several innovative approaches:
- Using AST-based analysis rather than simple text parsing for deeper code understanding
- Applying graph theory concepts to notebook restructuring for the first time
- Developing metrics to quantify the quality of notebook layouts
- Creating a programmatic approach to a previously manual process

## Skills Demonstrated

This project showcases my abilities in:
- Advanced Python programming and package development
- Understanding and manipulation of Abstract Syntax Trees
- Application of graph theory algorithms to practical problems
- Research methodology and validation
- Technical documentation and academic presentation

## Impact and Applications

NBNinja served as a core component of my Master's thesis framework and demonstrated the potential for automated tools to enhance collaborative data science workflows. The research contributed to the broader understanding of how spatial organization affects comprehension and collaboration in computational notebooks.

The tool continues to inform research on improving data science collaboration environments and has applications for both educational settings and professional data science teams.