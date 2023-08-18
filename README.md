**Believable Story Generarion using Transformers**

This repository contains all the code and data used in our research project, where we utilized GPT-2, GPT-3, and GPT-4 language models for generating anime narratives. The project involves both zero-shot story generation and fine-tuning of the models on a custom dataset.

**Contents**

src/: This directory contains all the necessary code files.

anime_info.csv: This is the dataset used in the project, collected from MyAnimeList via API requests up to the date of June 7th.

survey_Results.csv: This file contains the results of our human evaluation survey.

FinalCalculations.ipynb: This Jupyter notebook contains all the calculations for the standardization and comparison of the ratings.

**Code**

- dataset_fetcher.ipynb: This Jupyter notebook sends API requests to MyAnimeList to collect our dataset.
- ZeroShot_Stories.ipynb: This Jupyter notebook makes use of GPT-2, GPT-3 and GPT-4 for zero-shot story generation. The GPT-2 model is accessed through Hugging Face, while the GPT-3 and GPT-4 models are accessed via OpenAI.
- Anime_Generation_GPT2_SampleTest1.ipynb: This Jupyter notebook contains the code for fine-tuning the GPT-2 model.
- GPT3_Anime_Generator_Model_final.ipynb: This Jupyter notebook contains the code for fine-tuning the GPT-3 model.

**Setup**


The project is entirely written in Python and was developed using Google Colab.

**Dataset**

The anime_info.csv dataset was generated by running the dataset_fetcher.ipynb Jupyter notebook, which collects data from MyAnimeList via API requests. The dataset used in this project is up-to-date as of June 7th.

**Generation & Fine-Tuning**

Zero-shot story generation is performed in the ZeroShot_Stories.ipynb notebook, using GPT-2, GPT-3, and GPT-4 models. Fine-tuning of the GPT-2 and GPT-3 models is done in the Anime_Generation_GPT2_SampleTest1.ipynb and GPT3_Anime_Generator_Model_final.ipynb notebooks respectively.

The fine-tuning process consists of:

- Cleaning the dataset.
- Training the model on our data.
- Fine-tuning for story generation.
- Automatic evaluations.
- Evaluation & Standardization
- Human evaluation results are stored in survey_Results.csv. These results are used to calculate the average human rating. The FinalCalculations.ipynb Jupyter notebook is then used to standardize all the ratings for comparison purposes.


**The Best Rated Story combined with midjourney**

![Kota1](https://github.com/rkj43/Believable-Story-Generation-using-Transformers-master/assets/53295999/552bf307-14e8-42be-b52f-106eaa055c1f)
![Kota4](https://github.com/rkj43/Believable-Story-Generation-using-Transformers-master/assets/53295999/0f19cf03-c2a6-441b-822f-7c8d45d7b2fd)
![Kota3](https://github.com/rkj43/Believable-Story-Generation-using-Transformers-master/assets/53295999/44cd8418-3795-4a97-b8d5-24620c51e53a)
![Kota2](https://github.com/rkj43/Believable-Story-Generation-using-Transformers-master/assets/53295999/884cb0a2-cc7c-4aa9-a5e5-2f2754e33758)
![Kota5](https://github.com/rkj43/Believable-Story-Generation-using-Transformers-master/assets/53295999/e7960195-977f-45eb-8c80-da0a5b4ea2cd)


**Conclusion**

This project provides valuable insights into the narrative generation capabilities of GPT-2, GPT-3, and GPT-4 models. We hope this repository will be a useful resource for others looking to explore this field of research.

**Credits:**
We have referenced several websites and papers to help us finish this project. Credits for the scientific papers are in the final report.
Here we will list out some notable websites that were used to refer for the coding part.
- https://platform.openai.com/examples
- https://huggingface.co/docs/transformers/model_doc/gpt2
- https://scikit-learn.org
- https://stackoverflow.com/
- https://www.kaggle.com/code/floevan/dl-and-ml-for-nlp/notebook#SIMPLE-RNN
- https://www.midjourney.com
