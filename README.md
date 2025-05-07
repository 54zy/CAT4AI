# Position: AI Evaluation Should Learn from How We Test Humans

This is a position paper accepted by ICML 2025

## ❗ What is Adaptive Testing About?


**Computerized Adaptive Testing** stands as one of the earliest and most successful integrations of educational practices and computing technology.  

In evaluating human abilities, psychometrics gradually replaced traditional paper-and-pencil testing with a more advanced approach—-adaptive testing. This approach employs an understanding of cognitive functions and processes to guide the design of assessments, including the measurement of human knowledge, abilities, attitudes, and personality traits. By capturing the characteristics and utility (e.g., difficulty, discrimination) of different items and adjusting the test items in real-time based on the test-taker's performance, adaptive testing avoids overwhelming them with numerous items all at once. Adaptive testing has been widely applied in high-stakes exams such as the Graduate Management Admission Test (GMAT), Graduate Record Examinations (GRE), and the Scholastic Assessment Test (SAT).



## Data in the Paper

All raw data mentioned in the paper can be found in the `data` directory, which includes:

- `GSM8K_irt_feature.json`, `MedQA_irt_feature.json`: Estimated IRT features of each item in the GSM8K and MedQA dataset (Figure 2,9,10).
- `guess/`: Guessing factors data for contaminated and uncontaminated items across three benchmarks (MATH, NarrativeQA, RAFT) (Figure 3). Here, 0 indicates no contamination, and 1 indicates contamination.
- `consistency.json`: Rankings consistency data with Full Benchmark.
- `similarity/`: The average Jaccard similarity coefficient data of the selected items for each LLM on the MATH benchmark. The number of selected items increases from 10% to 80% of the entire benchmark.


