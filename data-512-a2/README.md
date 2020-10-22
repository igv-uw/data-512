# Objective
Identify potential sources of bias in a corpus of human-annotated data, and describe some implications of those biases.
The corpus you will use is called the Wikipedia Talk corpus, and it consists of three datasets. Each dataset contains
thousands of online discussion posts made by Wikipedia editors who were discussing how to write and edit Wikipedia articles.
Crowdworkers labeled these posts for three kinds of hostile speech: “toxicity”, “aggression”, and “personal attacks”.  
This repository focuses on analyzing aggression and toxicity to identify possible sources of biases by checking if groups are
under or over represented in the pool of workers that labeled the data. We also check if different groups of workers
significantly label comments differently from other groups.  
The motivation of this analysis is to keep in mind and to account for these possible biases when training a model using the presented datasets, as they may impact predictions of the model in the future.

# Data
Datasets from [Figshare](https://figshare.com/projects/Wikipedia_Talk/16731).

# Resources
- [Wiki Detox](https://meta.wikimedia.org/wiki/Research:Detox).
- [Perspective API](https://www.perspectiveapi.com/#/home).

# License
Project under [MIT License](LICENSE).
