# Cognitive Distortion Spanish 

### Summary
This project addresses the scarcity of Spanish-language resources for Natural Language Processing (NLP) in mental health, specifically in the detection of cognitive distortions. Given the dominance of English in scientific research and technological development, a gap exists in the availability of tools and models adapted to Spanish, limiting the effectiveness of NLP applications in Spanish-speaking contexts. To mitigate this problem, the project focused on translating and processing a dataset of cognitive distortions from English and Chinese into Spanish. Data was collected from various sources like Kaggle and GitHub, and 13 cognitive distortion labels relevant to the Peruvian context were selected with the guidance of a mental health expert. The translation was performed using the OpenAI GPT-4 API and ChatGPT interface. Subsequently, the data was preprocessed, including sentence vectorization using the BETO model, a BERT variant for Spanish. A multi-label classification model was implemented with BETO and trained on the translated and vectorized data. To address class imbalance, examples from over-represented classes were removed, and synthetic data was generated with ChatGPT for under-represented classes, achieving a balanced dataset with approximately 1500 examples per category. The final result is a BETO model trained to detect cognitive distortions in Spanish, contributing to the development of NLP tools for mental health in Spanish.

### Labels

| Cognitive Distortion | Description |
|---|---|
| All-or-Nothing Thinking | Seeing things in black and white categories, with no middle ground. |
| Overgeneralization | Seeing a single negative event as a never-ending pattern of defeat. |
| Mental Filtering | Focusing only on negative details while ignoring positive ones. |
| Disqualifying the Positive | Transforming positive experiences into negative ones. |
| Jumping to Conclusions | Making negative assumptions without sufficient evidence.  Includes "Mind Reading" (assuming others' negative thoughts) and "Fortune Telling" (predicting negative outcomes). |
| Magnification (Catastrophizing) & Minimization | Exaggerating the importance of shortcomings or minimizing the importance of desirable qualities. |
| Emotional Reasoning | Mistaking feelings for facts. |
| Should Statements | Using critical "should," "must," or "ought" statements that lead to guilt and frustration. |
| Labeling | Assigning global negative traits to oneself or others. |
| Personalization | Taking responsibility for events outside one's control. |
| Comparison and Despair | Feeling inadequate by comparing oneself to others, leading to hopelessness. |
| Blaming | Holding others responsible for one's own pain or problems. |

### 

This repository contains the following:

* **Code:** The code for this project, implemented in Google Colab, is provided in the `code` directory (`cognitive_distortion_classifier.ipynb`).  This includes the data preprocessing, model training, and evaluation scripts.

* **Dataset:** The processed dataset, translated into Spanish and vectorized for use with the BETO model, is available in the `data` directory. 

### References
| Paper/Dataset Name | Characteristics | Link |
|---|---|---|
| Detecting Cognitive Distortions from Patient-Therapist Interactions | 2,500 instances, 10 labels, English | [Link 1](https://www.kaggle.com/datasets/sagarikashreevastava/cognitive-distortion-detetction-dataset?resource=download) |
| Evaluating the Efficacy of Supervised Learning vs. Large Language Models... (Supervised Learning and Large Language Model Benchmarks on Mental Health Datasets) | 9,544 instances, 12 labels, Chinese | [Link 2](https://github.com/HongzhiQ/SupervisedVsLLM-EfficacyEval) |
| Cognitive Reframing of negative thoughts through human-language model interaction | 300 data pairs, 8 labels, English | [Link 3](https://github.com/behavioral-data/Cognitive-Reframing) |
| C2D2: A Resource for Analyzing Cognitive Distortions and Its Impact on Mental Health | 7,500 instances, 8 labels, Chinese (Restricted Access - contact Dr. Bichen Wang) | [Link 4](https://github.com/bcwangavailable/C2D2-Cognitive-Distortion) |
| Formulating Automated Responses to Cognitive Distortions for CBT Interactions | 200 data pairs, 14 labels, English | [Link 5](https://github.com/itoledorodriguez/cbt-dataset) |
| Detection and Positive Reconstruction of Cognitive Distortion sentences | 4,000 instances, 10 labels, Chinese | [Link 6](https://github.com/405200144/Dataset-of-Cognitive-Distortion-detection-and-Positive-Reconstruction/tree/main) |

