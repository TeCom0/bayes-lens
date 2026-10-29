# Bayes Lens: one theorem, three worlds

An interactive, single-page app that shows what a positive medical test, an AI's cancer flag, and a social media feed each reveal once you apply Bayes' rule. Probability and statistics project.

**Live page:** https://tecom0.github.io/bayes-lens/

## What's inside

- **Diagnosis.** Adjust prevalence, sensitivity and specificity and watch the posterior change, with a probability tree, a population grid, and repeat tests where today's posterior becomes tomorrow's prior (including a setting for tests that share a cause of error).
- **Imaging AI.**
  - *Part A* takes the published sensitivity, specificity and prevalence of two mammography AI studies (Lunit INSIGHT MMG in Southern Denmark; Google's AI in five UK NHS services), predicts recall rate and PPV with Bayes' rule, and compares the prediction with what the authors reported.
  - *Part B* trains a Naive Bayes classifier in the browser on the Wisconsin Diagnostic Breast Cancer dataset (569 masses, 398 train / 171 test), step by step, and shows where the prior hides inside a trained model. The model matches scikit-learn's `CategoricalNB`.
- **Social feed.** A recommendation feed that keeps a posterior belief about engagement per item and samples from it (Thompson sampling), and how it narrows toward outrage content while engagement rises.
- **Platforms and limits.** Where Bayes' rule is used in real systems (spam filtering, ads, game matchmaking, clinical trials, ML libraries, LLMs) and the limitations that kept coming back: the prior dominates, likelihoods are estimates, evidence is rarely independent, sparse data, uncalibrated scores, drift, and the wrong objective.

Every number on the page is computed live from Bayes' rule; nothing is hard-coded except the scenario presets. Sources are cited on each tab.

## Run it

It is one self-contained `index.html` with no build step. Open it in a browser, or use the live page above.

## How it was built

The code was generated with Claude (Anthropic) and checked against hand calculations, as the page itself states.
