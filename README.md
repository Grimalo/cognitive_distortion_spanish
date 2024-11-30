# Cognitive Distortion Spanish 

### Summary
This project addresses the scarcity of Spanish-language resources for Natural Language Processing (NLP) in mental health, specifically in the detection of cognitive distortions. Given the dominance of English in scientific research and technological development, a gap exists in the availability of tools and models adapted to Spanish, limiting the effectiveness of NLP applications in Spanish-speaking contexts. To mitigate this problem, the project focused on translating and processing a dataset of cognitive distortions from English and Chinese into Spanish. Data was collected from various sources like Kaggle and GitHub, and 13 cognitive distortion labels relevant to the Peruvian context were selected with the guidance of a mental health expert. The translation was performed using the OpenAI GPT-4 API and ChatGPT interface. Subsequently, the data was preprocessed, including sentence vectorization using the BETO model, a BERT variant for Spanish. A multi-label classification model was implemented with BETO and trained on the translated and vectorized data. To address class imbalance, examples from over-represented classes were removed, and synthetic data was generated with ChatGPT for under-represented classes, achieving a balanced dataset with approximately 1500 examples per category. The final result is a BETO model trained to detect cognitive distortions in Spanish, contributing to the development of NLP tools for mental health in Spanish.

### References
| Paper/Dataset Name | Characteristics | Dataset Link |
|---|---|---|
| Detecting Cognitive Distortions from Patient-Therapist Interactions | 2,500 instances, 10 labels, English | [Link 1](https://www.kaggle.com/datasets/sagarikashreevastava/cognitive-distortion-detetction-dataset?resource=download) |
| Evaluating the Efficacy of Supervised Learning vs. Large Language Models... (Supervised Learning and Large Language Model Benchmarks on Mental Health Datasets) | 9,544 instances, 12 labels, Chinese | [Link 2](https://github.com/HongzhiQ/SupervisedVsLLM-EfficacyEval) |
| Cognitive Reframing of negative thoughts through human-language model interaction | 300 data pairs, 8 labels, English | [Link 3](https://github.com/behavioral-data/Cognitive-Reframing) |
| C2D2: A Resource for Analyzing Cognitive Distortions and Its Impact on Mental Health | 7,500 instances, 8 labels, Chinese (Restricted Access - contact Dr. Bichen Wang) | [Link 4](https://github.com/bcwangavailable/C2D2-Cognitive-Distortion) |
| Formulating Automated Responses to Cognitive Distortions for CBT Interactions | 200 data pairs, 14 labels, English | [Link 5](https://github.com/itoledorodriguez/cbt-dataset) |
| Detection and Positive Reconstruction of Cognitive Distortion sentences | 4,000 instances, 10 labels, Chinese | [Link 6](https://github.com/405200144/Dataset-of-Cognitive-Distortion-detection-and-Positive-Reconstruction/tree/main) |
content_copy
Use code with caution.
Markdown

This is ready to be pasted directly into your GitHub README.md file. Remember to replace "Link 1", "Link 2", etc. with the actual URLs. The markdown formatting creates a clean, organized table.
