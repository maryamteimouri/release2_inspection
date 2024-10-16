# release2_annotation
## Purpose of annotation
We want to get a rough idea about the actual content of the cleaned verion of the 2nd data release. More specifically, for a subset that should correspond to some language L we want to estimate:
1) the proportion of texts that are in fact not in the language L,
2) the proportion of texts that can be considered undesirable because they are unnatural,
3) the proportion of texts that can be considered undesirable porn texts.

Additionally, we plan to compare these characteristics for the older and the newer crawls, and also for the IA and CC crawls.

## Data for round 1 of annotation: 
* samples stratified by language and crawl group,
*  4 groups (cc/ia old/new),
*  first 5 batches per language,
*  200 examples per batch,
*  500/500 characters from the beginning of the fist/second half of each text.

## Annotation
Please select one or more batches for a language you want to annotate. Do not forget to push the annotated files back to this repository.

We ask to provide 3 binary labels for each example:
* porn? empty/1: if the text looks like porn put 1, otherwise leave empty
* unnatural? empty/1: if the most text looks unnatural (e.g. word lists in CEO, mostly boilerplate) put 1, otherwise leave empty
* lang correct? 0/1: always fill this field (otherwise we will not distinguish labeled and unlabeled examples), put 0 if most of the text is not in the target language, otherwise put 1.

## Advice on annotation
Annotating 20 examples from Russian, batch0 took 5 minutes for me, thus, the estimated time for annotating 1 batch is 1 hour.
One way to annotate is using LibreOffice Calc. For convenience freeze first 4 columns (select them and click View -> Freeze Rows and Columns). Also make the text area larger. This can look like this:
![image](https://github.com/user-attachments/assets/0a89750c-7b8b-47c3-9beb-584431d27162)

