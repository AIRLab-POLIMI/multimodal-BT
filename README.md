# Multimodal Behavior Tree Generation: A Small Vision-Language Model for Robot Task Planning

![](images\graphical_abstract.png)

## Overview
Large and small language models have been widely used for robotic task planning. At the same time, vision-language models (VLMs) have successfully tackled problems such as image captioning, scene understanding, and visual question answering. In this work, we combine these two approaches by deploying a compact, open-source multimodal model to generate behavior trees for robotic task planning. The main obstacle to achieving this goal is the lack of an existing dataset that links visual observations and instructions to executable behavior trees. We propose a method to construct such a dataset starting from existing robotic episodes (i.e., Open X-Embodiment), in which a large model serves as a teacher in a multi-stage generation pipeline. We use this dataset to fine-tune VLMs ranging from 500M to 4B parameters via parameter-efficient fine-tuning (PEFT). The generated behavior trees, compatible with the BehaviorTree.CPP library, are evaluated both offline, using structural and lexical metrics, and online through the execution of household tasks in a state-of-the-art embodied simulator. Our results demonstrate that our fine-tuned 4B-parameter VLM approaches the performance of state-of-the-art closed-source models, achieving an 87\% success rate while requiring only a fraction of the computational resources.

> [!WARNING]
> The manuscript is under review, and the source code and dataset will be released after publication.

> [!CAUTION]
> Temporary Citation (Preprint) - ArXiv: 
>

**Authors**: [Cristiano Battistini](mailto:cristiano.battistini@mail.polimi.it), [Riccardo Andrea Izzo](mailto:riccardo.izzo@mail.polimi.it), [Gianluca Bardaro](mailto:gianluca.bardaro@polimi.it) and [Matteo Matteucci](mailto:matteo.matteucci@polimi.it)  
**Location**: [**AIRLab** (The Artificial Intelligence and Robotics Lab of Politecnico di Milano)](https://airlab.deib.polimi.it/)

