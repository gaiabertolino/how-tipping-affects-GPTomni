# Corruptibility Analysis of GPT-4o Under Tip-Based Prompting

#### Keywords

`Large Language Models`, `GPT-4o`, `Behavioral Evaluation`, `TruthfulQA`, `Bias Induction`, `EmotionPrompt`, `Prompt Engineering`, `Statistical Metrics`, `NLP Evaluation`.

This project investigates whether and how the responses of the language model **GPT-4o** change—qualitatively and quantitatively—when the model is **promised a monetary tip**. The experiment replicates and extends observations originally made by developer *Theia Vogel*, who noted that GPT-4 Turbo appeared to produce longer and more detailed answers when offered a tip.

Building on this idea, this notebook systematically measures the **corruptibility** of GPT-4o using **controlled prompts**, **multiple tip levels**, and **evaluation against the TruthfulQA benchmark**. The results allow us to quantify how tips affect answer length, quality, and truthfulness.

This project was developed as part of an academic research experiment in artificial intelligence and behavioral evaluation of LLMs.

---

### Key Features

* **Controlled Prompting Experiment**: Each question is asked three times under different conditions — no tip, $20 tip, and $200 tip.
* **TruthfulQA Benchmarking**: Random selection of questions from TruthfulQA to evaluate truthfulness and robustness.
* **Statistical & Model-Based Metrics**: Uses BLEU, ROUGE, BLEURT, METEOR, TER, and BERTScore to compare model outputs.
* **Behavioral Analysis**: Examines how GPT-4o modifies answer length, detail level, and semantic similarity under tipping incentives.
* **Reproducible Notebook**: A complete Python notebook that runs the full pipeline, from prompt generation to evaluation and visualization.
* **Bilingual Resources**: Documentation and analysis available in both English and Italian.

---

### Project Structure

* **Notebook.ipynb**
  A complete and reproducible experiment containing:

  * *Experiment Setup*: Explanation of tipping behavior, emotional prompting, and prior research.
  * *Question Sampling*: Random extraction of 30 TruthfulQA questions.
  * *Response Generation*: Calls to GPT-4o with different tip amounts.
  * *Evaluation*: Computation of statistical and neural metrics (ROUGE, BLEU, BLEURT, TER, METEOR, BERTScore).
  * *Analysis*:

    * Comparison against ground truth (Best Answer + Correct Answer).
    * Comparison against the zero-tip condition.
    * Measurement of absolute and percentage increases in character length.
  * *Visualizations*: Plots and summaries highlighting behavioral differences across tip levels.

* **Notebook_ITA.ipynb** 
  Italian-translated version of the experiment, designed for academic purposes.

* **Presentation_ITA** 
  Slide deck in Italian summarizing the experiment and its results.
