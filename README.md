# project_R
Linguistic Data: Quantitative Analysis and Visualisation

Hypothesis
Entropy should be higher in colloquial speech than in scientific texts and this difference should be the most noticeable in three linguistic parameters:

1) Most frequent colloquial phrases like "you know"
2) Elliptical structures
3) Contracted forms


Our data is a combined dataset that includes tweets about COVID-19 that were obtained through Kaggle and parsed scientific articles about COVID-19 that were sampled from CORD corpus. In this work we only used the texts themselves without any additional information from the datasets. The datasets concerned the scientific articles have the following columns:

1. `text` - the text of the articles
2. `contracted` - contracted forms and most frequent colloquial phrases found in the article
3. `count_contr` - the amount of contracted forms normalised ny the number of words in the article
4. `elliptical_rate` - the amount of elliptical sentences normalised ny the number of words in the article

Data in the repository:
* `twitter_data_ellipse.csv.gz` - twitter data
* `cleaned_dataset_science_pt1_ellipse.csv.gz` - first part of the scientific data
* `dataset_science_pt2_ellipse.csv.gz` - second part of the scientific data
* `data.csv` - combined data without `text` column

Python scripts:
* `Data.ipynb` - clean duplicates in scientific texts
* `prepare_twitter_data.ipynb ` - prepares twitter data
* `R_project.ipynb` - prepares scientific data
* `Udpipe_R.ipynb ` - obtaines sentences with elliptical structure

`twitter_data.Rmd` - creates two draft datasets Scientific articles + twitter
