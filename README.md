# In Search For A Cure: Recommendation with Knowledge Graph on CORD-19

## Tutors

* Le Zhang, Microsoft
* Iris Shen, Microsoft
* Jianxun Lian, Microsoft
* Chieh-Han Wu, Microsoft
* Miguel Fierro, Microsoft
* Andreas Argyriou, Microsoft

## Introduction

The Coronavirus (COVID-19) that for weeks pressingly called for research that
helps establish containment of the pandemic from academia’s perspective. The
CORD-19, or COVID-19 Open Research Dataset [8], was launched in March 2020, in
response to a request from the White House’s office of Science and Technology
Policy. The collaboration from AI2, Microsoft, the NLM at the NIH, and other
prestigious research institutes aims at empowering the world’s AI researchers
with a text and data mining tools to help accelerate COVID-19 related research.
CORD-19 is a free resource of over 45,000 scholarly articles, including over
33,000 with full text, about the coronavirus for use by the global research
community. In CORD-19, over 90% of the publications are mapped with articles in
the Microsoft Academic Graph (MAG) [9][12][13] which is an academic domain
knowledge graph containing various types of scientific publication records,
citation relationships, as well as authors, institutions, journals, and fields
of study. This hands-on tutorial introduces the CORD-19 dataset together with an
associated academic knowledge graph – a subgraph of Microsoft Academic Graph
(MAG) includes 6 types of entities with one million nodes and over one million
edges covering more than 100K bio-med academic concepts. The general aim of the
tutorial is to empower data science and machine learning research community,
especially the attendees of the tutorial session, to build their own knowledge
graph aware applications with the help of MAG and CORD-19 data set. In the lab
session, a particular use case of finding relevant articles for COVID-19, to
help scientists in the healthcare domain to perform efficient academic research,
is illustrated with hands-on examples and codes. The demonstrated knowledge
graph-based recommender model as well as the industry-grade operationalization
architecture is based on top of the academic research and development outcome
from Microsoft Research Asia and the Microsoft Azure Global Industry team, which
is mostly covered in the Microsoft/Recommender GitHub repository [2][5]. 


## Outline

The general objective of the tutorial session to help the attendees ramp up with
hands-on experience around knowledge graph, recommendation, and the application
of the technologies on CORD-19 dataset. In total the tutorial will take 3 hours.
Detailed session information can be found as below.
1.  Opening (15 mins) 
    1.  General introduction of context (3 mins) 
        1.  Briefly
        talk about COVID-19 outbreak and its impact on economy, society, and human
        beings. 
        1. Talk about joint efforts from industry and academia to fight
        against COVID-19 – CORD-19 dataset for building knowledge-aware AI system
        that prevents further spread of the virus. 
    1.  Lab 0: Environment setup (12
        mins) 
        1.  Install and configure of the required software and tool 
        1. Test
        of the packages, APIs, and scripts for the later lab sessions. 
1.  Module I: Basics of the dataset CORD-19 and the Knowledge Graph (25 mins) 
    1.
    Introduction of the Dataset CORD-19 (5 mins) 
    1.  Introduction of knowledge
    graph and Microsoft Academic Graph (MAG) (5 mins) 
    1.  Lab 1: Link the
    CORD-19 and MAG via the academic knowledge API (15 mins)
1.  Module II: Understanding contents with the aid of the Knowledge Graph (40
    mins) 
    1.  Introduction of content understanding with knowledge graph (10
    mins) 
        1.  Discuss semantically understanding of a given document with text
    information by using knowledge graph 
        1. Discuss classification of a given
    document with knowledge graph 
    1.  Lab 2 – 1: Document classification (10
    mins) 
        1.  Illustrate the general APIs of Language Similarity tool. 
        1.
    Demonstrate how to use the Language Similarity tool to tag / classify the
    document 
    1.  Introduction of document understanding by using the knowledge
    graph structural info (10 mins) 
    1.  Lab 2 – 2: Analytical study of author
    co-citation network (10 mins) 
        1.  Create author collaboration graph 
        1.
    Analyze the author co-citation with the homogeneous network 
1.  Module III: Applications of Knowledge Graph: Academic Recommender Systems
    (45 min) 
    1. Introduction to academic recommendation with knowledge graph (5
    min) 
        1. Introduce the user2item recommendation which is to recommend related
           papers for researchers based on their citation history.
        1. Introduce the item2item recommendation which is given an article, to
           recommend a list of related papers.
    1. Introduction to Microsoft/Recommenders (5 min) 
    1. Introduction on Knowledge-aware Recommender algorithms (5 min) 
        1. Discuss the knowledge graph data in the scenario of academic
           recommendations.
        1. Discuss the Deep Knowledge-aware Network model (DKN[1]) that injects
           knowledge entities into document content for better recommendations.
    1. Lab 3 – 1: Data preparation (10 min) 
        1. Manipulate data from raw datasets.
        1. Training, validating, and testing data construction.
    1. Lab 3 – 2: Pretraining embeddings (10 min)
        1. Pretrain word embeddings.
        1. Pretrain knowledge graph embeddings.
    1. Lab 3 – 3: Building knowledge-aware recommendation models (15 min)
        1. Use DKN to build a User2Item recommendation model.
        1. User DKN to build a Item2Item recommendation model.
    1. Lab 3 – 4 (optional): Model evaluation and comparison (5 min)
        1. Compare variants of DKN: with and without the knowledge entities.
        1. Compare DKN with a graph-based model:  LightGCN[14].
1.  Module IV: Operationalization of KG-based recommender system (40 mins) 
    1. Lab 4: Explanation of the knowledge-graph based analytics on CORD-19 data
    set (20 min) 
        1.  Walk through the basic tools and software (e.g., Python
    matplotlib) used for visualizing graph structured data. 
        1. Illustrate the
    usage of the visualization tools for the built knowledge graph-based paper
    recommender. 
    1.  Introduction to globally distributed graph data storage for
    scalable queries via Gremlin (10 min) 
    1.  Introduce real-time scoring and
    ranking for recommending papers for users by using Kubernetes (10 min)
1.  Closing (15 mins) 
    1.  Present the summary of the tutorial 
    1.  Discuss about
    future work and discussion 
    1.  Question and answer

## Link to the code
[Link](https://aka.ms/kdd2020-covid-demo) to the code used in the tutorial. 

## Useful links

* [Microsoft/Recommenders](https://github.com/microsoft/recommenders) 
* [Microsoft Academic Graph Application on COVID-19 research](https://github.com/microsoft/mag-covid19-research-examples)


## References

1.	Hongwei Wang et al, “DKN: Deep Knowledge-Aware Network for News Recommendation”, ACM WWW 2018.
2.	Andreas Argyriou, Miguel Fierro, and Le Zhang, “Microsoft Recommenders: Best Practices for Production-Ready Recommendation Systems, ACM WWW 2020.
3.	Shen, Zhihong, and Dong, Yuxiao. From Graph to Knowledge Graph Algorithms and Applications. edX, 2019. https://www.edx.org/course/graphsto- knowledgegraphs-3
4.	Tang, Jie, and Dong, Yuxiao. Representation Learning on Networks: Theories, Algorithms, and Applications. WWW, 2019. https://www2019.thewebconf.org/tutorials.
5.	Le Zhang et al, “Building production-ready recommendation systems at scale”, KDD 2019. 
6.	Perozzi, Bryan, Rami Al-Rfou, and Steven Skiena. "Deepwalk: Online learning of social representations." Proceedings of the 20th ACM SIGKDD international conference on Knowledge discovery and data mining. 2014.
7.	Hamilton, Will, Zhitao Ying, and Jure Leskovec. "Inductive representation learning on large graphs." Advances in neural information processing systems. 2017.
8.	CORD-19, url: https://pages.semanticscholar.org/coronavirus-research
9.	Microsoft Academic Graph Documentation, url: https://docs.microsoft.com/en-us/academic-services/graph/
10.	Microsoft Academic Graph Application on COVID-19 research, url: https://github.com/microsoft/mag-covid19-research-examples
11.	Understanding Documentation By Using Semantics, url: https://www.microsoft.com/en-us/research/project/academic/articles/understanding-documents-by-using-semantics/
12.	Wang, Kuansan, et al. “Microsoft Academic Graph: When Experts Are Not Enough.” Quantitative Science Studies, vol. 1, no. 1, 2020, pp. 396–413.
13.	Wang, Kuansan, et al. “A Review of Microsoft Academic Services for Science of Science Studies.” Frontiers in Big Data, vol. 2, 2019.
14. Xiangnan He, et al. LightGCN: Simplifying and Powering Graph Convolution Network for Recommendation. SIGIR '20

