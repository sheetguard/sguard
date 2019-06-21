# SGuard Homepage

## Introduction

### End-users' puzzle

Nowadays, spreadsheets (e.g., Excel, Google Sheets) are being widely used in many fields, such as, corporate reporting, financial statistics, etc. However, spreadsheets are found to be error-prone, especially for their formula-related cells. These errors (namely, spreadsheet defects) are hard to detect, since spreadsheets are usually not supported by auditing and tracking services and semantic relationships among spreadsheet cells are typically vague.

### Our solution

Our tool SGuard can effectively detect such spreadsheet defects. As shown in the ![workflow figure](graphics/workflow.png), SGuard learns spreadsheet features to cluster cells with similar computational semantics, and then refine these clusters to recognize anomalous cells as defects. SGuard well balances the trade-off between the precision (87.8%) and recall rate (71.9%) in the defect detection, and achieves an F-measure of 0.79, exceeding existing spreadsheet defect detection techniques.

## Usage

### Prerequisites

We have released our tool SGuard as an executable jar file and tested it on Windows 10 installed with Java 8. For  full functionality, we strongly encourage users to execute SGuard on Windows 10, since its partial functionality need platform-dependent DLL files used by Z3 constraint solver.

### Demonstration



### Video

We also provide a vivid [video](xx) presentation on YouTube.

## Related research work

This tool SGuard builds on our previous work, [CUSTODES](https://dl.acm.org/citation.cfm?id=2884796) (ICSE16) and [WARDER](https://cs.nju.edu.cn/changxu/1_publications/QRS19.pdf) (QRS19). For further information about CUSTODES, you can visit another [website](http://sccpu2.cse.ust.hk/custodes/).

## Contact us

If you have any question, please feel free to contact authors via [email](mailto:njulida@outlook.com) or creating an [issue](https://help.github.com/en/articles/creating-an-issue) in this repository.
