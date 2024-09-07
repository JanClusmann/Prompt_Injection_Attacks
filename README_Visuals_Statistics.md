# R Code for VLM Performance Analysis in Medical Imaging

This repository contains R code used for analyzing the performance of Vision-Language Models (VLMs) in medical imaging tasks, with a focus on organ detection and lesion identification. The code was developed as part of the study "Prompt Injection Attacks on Large Language Models in Oncology".

## Contents

1. Processing and preparing the raw data.
2. Functions for conducting statistical tests and summarizing results.
3. Code for generating plots and figures used in the publication.
4. Utility functions for exporting results to Excel.

## Key Features

- Calculation of organ detection rates and lesion misdetection rates (LMR)
- Analysis of the impact of prompt injection on VLM performance
- Computation of Attack Success Rates (ASR)
- Statistical comparisons between different VLMs and conditions
- Visualization of results using ggplot2
- Export of summary statistics and test results to Excel

## Usage Summary Statistics and Visuals

To run the analysis:

1. Ensure all required R packages are installed (dplyr, ggplot2, rstatix, openxlsx).
2. Set the working directory to the repository root.
3. Import raw data (Column names "Case"                           "Modality"                       "Text prompt"                    "Adversarial prompt"             "Position of adversarial prompt" "Variation"                      "Model"                          "Language of injection prompt"   "Model Output 1"
 "Model output 2"                 "Model output 3"                 "Labels1"                        "Labels2"                        "Labels3"                        "Harmfulness1"                   "Harmfulness2"                   "Harmfulness3"                   "Comment"
"Labels_Mean"                    "Harmfulness_Mean"               "PI Unveiled"

4. Run the script

## Data

The raw data is not included in this repository due to privacy concerns. Please refer to the methods section of the associated publication for details on data collection and preprocessing.

## Output

The code generates:
- Summary statistics for VLM performance
- Statistical test results (Wilcoxon tests, Mann-Whitney U tests)
- Visualizations of organ detection rates, lesion misdetection rates, and attack success rates
- Excel files containing detailed results and statistics

## Citation

If you use this code in your research, please cite our paper:

[Citation details to be added upon publication]

## License

MIT License

Copyright (c) 2024 Jan Clusmann

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Contact

For questions or issues regarding the code, please open an issue in this repository or contact jan.clusmann@rwth-aachen.de

