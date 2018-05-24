# Turing Reproducible Research Champions: Elena Kochkina

Elena led the Turing team's submission to Task 8 at SemEval-2017, *RumourEval: Determining rumour veracity and support for rumours (subtask A)*, which achieved the best score out of the eight submissions.
Machine learning approaches such as branch-LSTM often require substantial computational resources, which poses an interesting challenge for reproducibility.
During this project, we will investigate options for providing access to limited compute resources and approaches to simplify the installation and setup process for those who already have access to such resources themselves.

Elena Kochkina, Maria Liakata and Isabelle Augenstein (2017) *Turing at SemEval-2017: Sequential Approach to Rumour Stance Classification with Branch-LSTM*, in Proceedings of the 11th International Workshop on Semantic Evaluations (SemEval-2017), pages 475-480.
Available at [arXiv:1704.07221](https://arxiv.org/abs/1704.07221) [cs.CL].

## Collaborators

Elena's co-authors were Maria Liakata and Isabelle Augenstein.


| <img src="./elena-kochkina-square.jpg" height="300"> | <img src="./maria-liakata-square.jpg" height="300">
| :-----------------------:|:---------------------------:
| Elena Kochkina           | Maria Liakata

## Reproducible Research Q&A with Elena

**Can you give us a brief overview of your paper?**

In this paper we deal with rumour stance classification, the task of determining the attitude of the users discussing a rumour towards the truthfulness of the rumour.
Stance classification is considered to be an important step towards rumour verification, therefore performing well in this task is expected to be useful in debunking false rumours.
We propose a LSTM-based sequential model that, through modelling the conversational structure of tweets, outperforms other systems submitted to the SemEval-2017 Task 8.

**Why is reproducible research important in your specific field?**

Reproducibility of research is a proof of its trustworthiness.
Reproducibility often implies openness and accessibility of research that leads to its increased impact.
Ease of reproducibility helps speed up the progress on solving research problems for those taking it further from the original study.
I think researchers should focus on research reproducibility when publishing their work and I am happy to see a strong drive towards it in many fields, including computer science.


**How will making the research presented in your paper reproducible help increase its impact?**

Branch-LSTM model illustrates the idea of utilising conversation structure and decomposing the tree-like structure into linear branches that can be applied to other tasks involving analysis of conversations.
Also, this model will become a baseline for the next SemEval-2019 competition *RumourEval: Determining rumour veracity and support for rumours*.
