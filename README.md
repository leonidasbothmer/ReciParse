# 🌯 ReciParse

### 🎯 Create Step by Step Guides from unstructured German Cooking Recipes

### 🌐 www.reciparse.de

### Abstract

When following recipes, most users appreciate a clear and easy-to-follow instruction set. As manually rewriting recipe texts from various sources to only include the most relevant information and to be structured in a straightforward "step-by-step" manner is laborious work, we explored potential automated solutions. This repository contains our our experiments in the extraction of semantic information from German recipe texts using Machine Learning. To demonstrate a first proof-of concept, we implemented a full natural language processing (NLP) pipeline, starting from conceptualizing a task-appropriate annotation scheme, to modelling using modern NLP methods as well as developing an illustrative web application front end which can be accessed via http://www.reciparse.de/ . Despite the inherent ambiguities of linguistical annotation, we managed to achieve an Inter-Annotator Agreement of over 95%. Our models are two sequentially stacked neural networks using transfer learning based on transformer architectures. The first is a "named entity recognizer" (NER) which identifies and categorizes appropriate subsets of a text into recipe-relevant classes. These entity predictions serve as the basis upon which the second model, the "relations component" (REL), assigns class entities to the appropriate steps and deals with cross-sentence references. We were able to achieve a notable micro average F-Score of 94.6% for NER, while REL manages to achieve 74.3%. This project lays a valuable foundation for future work on the topic and cogently demonstrates that this task can, in principle, be approximated by machine learning.
