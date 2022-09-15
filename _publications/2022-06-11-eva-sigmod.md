---
title: "EVA: A Symbolic Approach to Accelerating Exploratory Video Analytics with Materialized Views"
collection: publications
permalink: /publications/2022-06-11-eva-sigmod.md
excerpt: 'This paper is about the number 2. The number 3 is left for future work.'
date: 2022-06-11
venue: "SIGMOD '22: Proceedings of the 2022 International Conference on Management of Data"
paperurl: 'https://dl.acm.org/doi/abs/10.1145/3514221.3526142'
# citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---
Advances in deep learning have led to a resurgence of interest in video analytics. In an exploratory video analytics pipeline, a data scientist often starts by searching for a global trend and then iteratively refines the query until they identify the desired local trend. These queries tend to have overlapping computation and often differ in their predicates. However, these predicates are computationally expensive to evaluate since they contain user-defined functions (UDFs) that wrap around deep learning models.

In this paper, we present EVA, a video database management system (VDBMS) that automatically materializes and reuses the results of expensive UDFs to facilitate faster exploratory data analysis. It differs from the state-of-the-art (SOTA) reuse algorithms in traditional DBMSs in three ways. First, it focuses on reusing the results of UDFs as opposed to those of sub-plans. Second, it takes a symbolic approach to analyze predicates and identify the degree of overlap between queries. Third, it factors reuse into UDF evaluation cost and uses the updated cost function in critical query optimization decisions like predicate reordering and model selection. Our empirical analysis of EVA demonstrates that it accelerates exploratory video analytics workloads by 4x with a negligible storage overhead (1.001x). We demonstrate that the reuse algorithm in EVA complements the specialized filters adopted in SOTA VDBMSs.

<!-- [Download paper here](http://academicpages.github.io/files/paper2.pdf)

Recommended citation: Your Name, You. (2010). "Paper Title Number 2." <i>Journal 1</i>. 1(2). -->