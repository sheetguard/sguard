# Review Collection

## Reviewer 1

0. Being a mac user, I couldn't, unfortunately, run the jar on my own machine.

- **FACT:** I can run the jar on my mac, when the running process does not trigger the Z3 solver used in AmCheck/CACheck.

- **TODO:** ???

1. Section III.A: are the set of features listed complete? Are there other features used that the authors are not listing?

- **FACT:** In our paper, we list four of six weak features: *"SGUARD considers six weak features, including cell address, label [5], rectangle cell ranges [7], gap template [17], etc."* 

- **TODO:** Add all six features and related references.

2. Section III.A: the authors cite a few works to explain the approach, making the paper not really self-contained. I do understand this is because of the page limitations, though.

- **TODO:** ignore.

3. Section IV: The authors would benefit if the proposed solution would have been implemented as a plugin rather than a stand-alone tool.

- **TODO:** ignore.

4. Results: please report false negatives.

- **TODO:** ignore.

5. Section V: why using 300 worksheets? How were they selected?

- **FACT:** *"... on the VEnron2 spreadsheets, which consists of two parts: complete 6,258 worksheets and sampled 300 worksheets [12]."*

- **TODO:** 

6. there are a bunch of missing references. A work that comes to mind is: ...

- **TODO:** Add two related references, as we did in our QRS paper.

## Reviewer 2

1. It seems that the first stage in “cell clustering” is only for formula cells, while the second stage is for the data cells. Correspondingly, “strong features” are in terms of formula cell; while “weak features” are in terms of data cells. The above points should be explicitly indicated, current presentation is a bit confusing. And it is better to list a few “strong features” for better understanding the work flow.

2. I am curious about stage-2 of cell clustering. Data cells have different features from formula cells. Then, how can they be included into the seed clusters that consists of formula cells only? How was the similarity measured? I suggeste the authors give a bit more explanations.

3. It seems that the detected defects are all about the formulas: e.g. data cells will be reported as “missing formula”, formula cells with inconsistent formulas will be reported as “defect formula”. But how about the other types of defects? How many types of defects are considered in the experiments? Are the “missing formula” for data cells regarded as “true positive”? This relates to experimental results.

## Reviewer 3

1. While I appreciate that the paper is forthright about SGuard's relation to CUSTODES (SGuard's predecessor), my primary concern is that the current approach is only a minor increment over CUSTODES. The approach described in Section III seems to be the same as CUSTODES's approach. I would be helpful to highlight whatever differences there may be much more explicitly.

2. I also question the choice of evaluation benchmarks. SGuard's performance on the EUSES dataset is not bad, however the spreadsheets contained in that dataset are all rather simple, uniform, and in general don't represent the complexities of real-world spreadsheets. There is some concern that the tool is overfit to this set of spreadsheets. This problem is evidenced by the much worse performance on the VEnron2 dataset.

3. The paper distinguishes between CUSTODES and CUST-OPT, however only CUSTODES appears throughout the results. Which version of CUSTODES is SGuard evaluated against?

4. SGuard should also be compared against Melford, which claims a significantly lower false positive rate than CUSTODES (Melford: Using Neural Networks to Find Spreadsheet Errors).
