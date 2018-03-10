# Fully Automated Fact Checking Using External Sources

## Paper abstract:
Given the constantly growing proliferation of false claims online in recent years, there has been also a growing research interest in automatically distinguishing false rumors from factually-true claims. Here, we propose a general-purpose framework for fully-automatic fact checking using external sources, tapping the potential of the entire Web as a knowledge source to confirm or reject a claim. Our framework uses a deep neural network with LSTM text encoding to combine semantic kernels with task-specific embeddings that encode a claim together with pieces of potentially-relevant text fragments from the Web, taking the source reliability into account. The evaluation results show
good performance on two different tasks and datasets:
- rumor detection and 
- fact checking of the answers to a question in community question answering forums.

## Authors:
Georgi Karadzhov, Preslav Nakov, Lluís Màrquez, Alberto Barrón-Cedeño, Ivan Koychev
## Paper link: https://arxiv.org/abs/1710.00341

Please, cite the following paper if you use the resources below:
```bib
@InProceedings{RANLP2017:factchecking,
  author    = {Georgi Karadzhov and Preslav Nakov and Llu\'{i}s M\`{a}rquez and Alberto Barr\'on-Cede\~no and Ivan Koychev},
  title     = {Fully Automated Fact Checking Using External Sources},
  booktitle = {Proceedings of the 2017 International Conference on Recent Advances in Natural Language Processing},
  month     = {September},
  year      = {2017},
  address   = {Varna, Bulgaria},
  series    = {RANLP~'17}
}
```
## Resources

### Code:
Available upon request.

### Table:Rumour detection resources

| Name | Short description | Link|
| --- | --- | --- |
| Claims | Claims from snopes.com, each of them is labeled with Rumour or Non-rumour.  | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4cGM1ZVYya0xlZUU) | 
| Data splits | Exact splits used for training and evaluation of factchecking system  | [Train-Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4Nm5mMGp2cTBTaDQ) [Test-Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4N2p1UGthTWhzaWM)  [Development-Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4MDU1NERJSkwwQWs)| 
| Website credibility | Manually annotated list of websites. Possible labels(reputed-source, forum-type, others)  | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4Zm11VG56S19OMXc) | 
| Web data | Each claim augmented with automaticaly collected web data. Also includes all calculated similarities and avg. sentence vectors.  | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4NlhRZFl6c2hEQm8) | 
| Best web resources | Only web data, that has the highest similarity to the original claim. This is used to train the task-specific embeddings.  | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4OGJrR2tJNTVPYnM) | 
| Task-specific embeddings | Combined representation of a claim and the supporting web data. | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4NkdkNEV5RGJQckE) | 

### Table:Factchecking in cQA resources

| Name | Short description | Link|
| --- | --- | --- |
| QAs | Question and comments, from QatarLiving forum. | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4V3hqZldEM0Y2N28) | 
| QAs-concatenated | Question and comments, from QatarLiving forum, concatenated to represent a single entity. This data is used in the system. | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4V05jSzNDYnl4Mjg) | 
| Data splits | Exact splits used for training and evaluation of factchecking system  | [Train-Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4djB5LW1NQ3I1VXc) [Test-Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4RG9GSGlHUmFUZGc)  [Development-Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4YV93alRuU0hWNmM)| 
| Website credibility | Manually annotated list of websites. Possible labels(reputed-source, forum-type, others). For cQA dataset we also annotated wheter the website is Qatar related as it is relevant to the credibility of an answer  | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4dl9RLU1iNk9rZGM) | 
| Web data | Each QA-pair augmented with automaticaly collected web data. Also includes all calculated similarities and avg. sentence vectors.  | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4M2NBVHZWRE8tWVE) | 
| Best web resources | Only web data, that has the highest similarity to the original QA-pair. This is used to train the task-specific embeddings.  | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4TUo4cmhmYVhLYlE) | 
| Task-specific embeddings | Combined representation of a QA-pair and the supporting web data. | [Download](https://drive.google.com/uc?export=download&id=0B0rQz7n3NJj4eFBYRFhmampxSXM) | 
