---
layout: post
title: Validating Bill of Material (BOM) data
---

Bill of Material (BOM) is a highly used data representation in the Industry domain. It is used in engineering for both design and production processes. Each new or updated model of the machine means changes to the BOM, which can introduce human errors. For example, you want to upgrade the engine of a car, but overlook the limitations of the car suspension that might be incompatible with the new engine. In this project, we developed a way to automatically search for such mistakes using Machine Learning.
<p align="center">
    <img src="/images/Schneckengetriebe.png" height="400px"/>
</p>

The BOM is a list of components and parts within a machine (e.g. car, chair, shelf from Ikea, ...). The BOM contains properties of the part and relationships between the parts. The simplest relationship is the parent-child relation, e.g. car -> car skeleton -> door -> exterior mirror -> actual mirror part - forming a tree-like structure. The tree structure is used to describe each part not just by part properties, but also by the neighbouring parts - embeddings. 

Association mining is a data-based approach to learning statistically significant patterns. Correct BOMs can be used to learn patterns that occur in the "good" machines. These learned patterns can be used to uncover mistakes in the new or updated BOMs to spot any deviations from the correct BOMs.

I was (tech)leading a BOM validator project team at Kendaxa for ~ 1 year, where we implemented these ideas for various industries.