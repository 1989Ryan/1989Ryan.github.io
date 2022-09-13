---
title: "Differentiable Parsing and Visual Grounding of Verbal Instructions for Object Placement"
date: 2022-09-13T20:45:25+08:00
draft: true
---

Zirui Zhao, Wee Sun Lee, David Hsu



School of Computing, National University of Singapore

[<a href='./appendix.pdf'>Appendix</a>] [Dataset (comming soon)]

## Abstract

Grounding spatial relations in natural language for object placing could have ambiguity and compositionality issues. To address the issues, we introduce ParaGon, a PARsing And visual GrOuNding framework for language-conditioned object placement. It parses language instructions into relations between objects and grounds those objects in visual scenes. A particle-based GNN then conducts relational reasoning between grounded objects for placement generation. ParaGon encodes all of those procedures into neural networks for end-to-end training, which avoids annotating parsing and visual grounding labels. Our approach inherently integrates parsing-based methods into a probabilistic, data-driven framework. It is data-efficient and generalizable for learning compositional instructions, robust to noisy language inputs, and adapts to the uncertainty of ambiguous instructions.

