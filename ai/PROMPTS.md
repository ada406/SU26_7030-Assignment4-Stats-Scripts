# Prompts Log — Assignment 4 (AI-assisted Stats Scripts)

Tool used: Cursor (AI coding assistant)

This file records the prompts used to build the AI-assisted materials in the `ai/` folder for Assignment 4.

---

## 1. Initial notebook, data files, and environment

> i need your help to on an assignment. you are going to use these data files: /Users/lizzieadams/Downloads/wages.txt /Users/lizzieadams/Downloads/iris.csv /Users/lizzieadams/Downloads/brain_size.csv . create a jupyter notebook to answer these questions from brain_size.csv: 1. what is the mean value for VIQ of the full population? 2. how many males and females were in the study? 3. what is the average MRI count expresssed in log units for males and females? I would like the code to answer these questions all in one cell, with comments explaining what each line does and why it is required. also create an environment file with everything necessssary for the assignment. please give me all the files for review

**Follow-up setup prompt:**

> please put all the files for this in a folder called "ai". please name the notebook file ai/stats_python.ipynb.

**Outputs produced from these prompts:**
- `ai/stats_python.ipynb` (first exercise cell)
- `ai/environment.yml`
- `ai/brain_size.csv`
- `ai/iris.csv`
- `ai/wages.txt`
- `ai/README.md`

---

## 2. Scatter matrices by gender

> looks great so far! now with the same dataset, plot scatter matrices of height vs weight and for PIQ vs VIQ vs FSIQ for males and then females. after this analysis, clearly state whether subpopulations correspond to gender. add this to the notebook in a new coding cell. again, provide comments to explain all steps. please give me the updated notebook file to review

**Outputs produced from this prompt:**
- Updated `ai/stats_python.ipynb` with a new scatter-matrix exercise cell and conclusion about gender subpopulations

---

## 3. Hypothesis tests for Weight and VIQ

> looks great! the next exercise is to test the differnece between weights in males and females. then, use non parametric statistical tests (t tests) to test for differences in VIQ between males and females. again, please use a new coding cell with comments. please give me the new notebook file for review!

**Outputs produced from this prompt:**
- Updated `ai/stats_python.ipynb` with independent t-test for Weight and Mann–Whitney U test for VIQ
- `scipy` / `matplotlib` added to `ai/environment.yml` as needed

---

## 4. Linear regression parameters and summary

> looks great! the next exercise is to get the estimated parameters from a linear regression on this data. please print the summary. again, this should be in a new code cell and include comments. please give me the file for review

**Outputs produced from this prompt:**
- Updated `ai/stats_python.ipynb` with OLS model `VIQ ~ Gender + 1`, printed parameters and summary

---

## 5. Adjusted gender comparison (covariates)

> looks great! the next. exercise is to test if the VIQ values of males and females are different after removing the effects of brain size, height, and weight. please put this exercise in a new coding cell, with comments, and give me the file for review

**Outputs produced from this prompt:**
- Updated `ai/stats_python.ipynb` with OLS model `VIQ ~ Gender + MRI_Count + Height + Weight`, summary, and F-test for the gender effect

---

## 6. Extension: mixed-effects model

> can you now extend the analysis with one new method: a mixed effects model. this should be in a new notebook: "ai/stats_extension.ipynb"

**Outputs produced from this prompt:**
- `ai/stats_extension.ipynb` (long-format IQ scores; mixed-effects model with subject random intercept)
- `ai/README.md` updated to list the extension notebook

---

## 7. Prompt log

> now create a prompt log (ai/PROMPTS.md) for the same ai folder. include: [prompts 1–6 above]

**Outputs produced from this prompt:**
- `ai/PROMPTS.md` (this file)

---

## Notes

- Prompts are recorded as used in the Assignment 4 AI-assisted workflow.
- AI-generated notebooks and supporting files were reviewed before committing.
- Spelling and wording above match the original prompts as given.
