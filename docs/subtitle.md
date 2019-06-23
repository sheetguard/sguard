# Demo subtitle

## Part 1: Introduction

### Frame 1: title

Hello, everyone. In this video, we will show you our SGuard: a feature-based clustering tool for effective spreadsheet defect detection. 

### Frame 2: Motivation

<mark>Spreadsheets are widely used in many fields, while they are also error-prone. So, how to detect such spreadsheet defects? Our SGuard is targeted on effectively detecting such defects.</mark>

### Frame 3: SGuard's workflow

1. Our SGuard's workflow contains three components.
2. At the beginning, we obtain all cells in a worksheet.
3. The first component uses a two-stage clustering technique to cluster cells with similar computational semantics based on their shared strong (e.g., formula semantics) and weak features (e.g., layout information), aiming for a high recall rate.
4. After executing this component, expanded cell clusters are generated.
5. The second component refines the clustering results by squeezing out irrelevant cells from clusters and removing unquantified clusters, aiming for a high precision.
6. After executing this component, refined cell clusters are generated.
7. The third component analyzes the refined clusters and detect outliers in each cluster as defects to be presented to end users, aiming for providing useful bug information.

### Frame 4: tool with example

Next, we will show our SGuard's graphical interface with an illustrative example used in our paper.

## Part 2: GUI operation

1. First, to select a specific Excel spreadsheet file for analysis, you clicks the “Open Excel File” button in the menu bar and then all its associated worksheets would be listed in the left “Worksheet list” area for watch.
2. After that, you can select one or multiple spreadsheet defect detection techniques from the right “Internal techs” panel to analyze the worksheets in the opened spreadsheet. We integrate six techniques for comparison, <mark>in which our WARDER can achieve the best performance on selected spreadsheets.</mark>
3. Then, with a worksheet selected from the left panel and techniques selected from the right panel, you can click “Start analysis” to start SGuard’s defect detection process. When the analyses are complete, the results would be shown in the central panel for the selected worksheet.
4. Then one can choose to inspect certain results by clicking “Defective cells” or “Marked clusters” in the right middle panel.
5. In the “defective cells" part, you can simultaneously select multiple techniques to show all defective cells detected by at least one technique, while in the "marked clusters" part, the clustering result is shown one by one to avoid confusion. In this example, our WARDER can correctly recognize seven precise cell clusters, and detect seven true defects exactly.
6. Moreover, you can also easily save the detection results as files by clicking the “Save to files”  for later analyses or reuse. Some logging information would also be shown during the SGuard execution for deeper investigation.
7. You can also look into these clustering and detection result in our generated Excel files.

## Part 3 (Frame 5): Contact us

That is all about SGuard, thanks for watching. If you have any question, please contact us via video comments or email.
<mark> For more information, you can visit our SGuard's homepage. </mark>
