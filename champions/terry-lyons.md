# Turing Reproducible Research Champions: Terry Lyons

Terry's project is very interdisciplinary, bringing a signature-based machine learning approach to an application in mental health.
It is often not possible to fully release sensitive medical data; we will therefore investigate alternatives such as limited data sharing and the use of simulated datasets.

Imanol Perez Arribas, Guy Goodwin, Terry Lyons and Kate Saunders (2018) *A signature-based machine learning model for bipolar disorder and borderline personality disorder*.
Available at [arXiv:1707.07124](https://arxiv.org/abs/1707.07124) [stat.ML].

## Collaborators

#### Rough paths/signatures

| <img src="./imanol-perez-arribas-square.jpg" height="300"> | <img src="./terry-lyons-square.jpg" height="300">
| :-----------------------:|:---------------------------:
| Imanol Perez Arribas          | Terry Lyons

#### Clinical
Guy Goodwin, John Geddes, Kate Saunders

## Reproducible Research Q&A with Terry

**Can you give us a brief overview of your paper?**

The diagnosis and provision of feedback for psychiatric disorders is hampered by the dependency on narrative recall and the difficulty of defining their persistence over time.
The shortcomings of current diagnostic approaches have motivated a ‘bottom up’ approach to monitoring using more objective data streams.
However analysis of these data streams is very challenging.
This paper demonstrates that it is possible to place people on a spectrum using simple mood zoom information (daily scores for several emotions); the dimension reduction and restructuring achieved by signatures meant that even with the small samples available one was able to use second order information (the order of different events: anger before depression, …) in addition to first order (intensity, longevity of depression) of events to give considerable classification power and allow the differing diagnoses of the communities participating in this trial to be well separated.

Given the size of the trial, and the complex noisy nature of the data this was an excellent outcome clinically and from a data science point of view.
Specifically, we sought, and succeeded to a good degree, to classify the diagnosis of participants on the basis of their evolving mood and predict their mood the following day.
The generality of the signature-based machine learning model allows these problems to be treated in similar and generic methodology that can be shared with other contexts where one is analysing complex multimodal data.

**Why is reproducible research important in your specific field?**

This work contributes to our ability to capture medium term classification of mood disorder from higher frequency streamed data.
It is an area where effective discrimination could make a real difference, but where missing data and small datasets mean that results are often poor; sometimes, as here, novel approaches add real value.
The easy reproducibility of these results allows others to test and adopt these methods more quickly and also provides validation and significantly increased external confidence in the effectiveness of the approach.
The biggest challenge to reproducibility is that the raw data is really sensitive; overcoming this issue while still achieve the benefits mentioned above is key part of the project.

**How will making the research presented in your paper reproducible help increase its impact?**

There are numerous ways this project will assist.
Fundamentally, it will give faith in the novel methods once people realise they are easy to use (despite the alien math) and give effective analysis that is often state of the art straight out of the box.
