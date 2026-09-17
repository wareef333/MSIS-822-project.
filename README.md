# MSIS-822-project.
Project Title: Detection of AI-Generated Arabic Text: A Data Mining Approach
This is the final project of the Advanced Data Analytics techniques course.

The datasetKFUPM-JRCAI/arabic-generated-abstracts (Available on Hugging Face) were provided by the prof.

The dataset is organized into different subsets based on generation methods:
Generation Methods
1. by_polishing - Text refinement approach where models polish existing human
abstracts
2. from_title - Free-form generation from paper titles only
3. from_title_and_content - Content-aware generation using both title and paper content

## Methodology & Workflow

This project follows the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) framework:

1. **Business & Data Understanding**: Initial loading and structural analysis of the `KFUPM-JRCAI/arabic-generated-abstracts` dataset.
2. **Data Preprocessing & EDA**: Modular cleaning pipeline (diacritic removal, character normalization, ISRI stemming) and linguistic EDA across classes.
3. **Feature Engineering**: Extraction of assigned stylometric features and TF-IDF/BERT embeddings after a strict 70/15/15 train/val/test split to prevent data leakage.
4. **Modeling**: Benchmarking baseline models (Logistic Regression), tuning traditional ML classifiers (SVM, XGBoost), and training deep learning approaches (BERT/Feedforward NN).
5. **Evaluation & Interpretation**: Assessment on the held-out test set using F1-score, ROC-AUC, and feature importance analysis.

the first step is eda, where i combined all dataframe into one.I asses the data using three criteria of data statistcal measure. 1. Central Tendency. 2.Dispersion / Spread 3. Shape & Distribution

