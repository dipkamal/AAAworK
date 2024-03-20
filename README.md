# PASA: Attack Agnostic Unsupervised Adversarial Detection using Prediction \& Attribution Sensitivity Analysis

Repository for the paper "PASA: Attack Agnostic Unsupervised Adversarial Detection using Prediction \& Attribution Sensitivity Analysis," submitted at 9th IEEE European Symposium on Security and Privacy.

This paper provides our implementation of unsupervised adversarial detection using feature attribution and model prediction sensitivity.

The directory consists of the following folders:
- Ablation Study: This folder consists of notebooks for running an ablation study to measure how each of our statistical measures performs in adversarial detection when used standalone.
- Adaptive Attack: This folder consists of notebooks for performing adaptive attacks on the target model when an adversary knows about the defense.
- Collect Adversarial Samples: This folder consists of a notebook that will save adversarial samples using various adversarial attacks and save them as numpy files.
- Evaluation: This folder consists of notebooks to perform the evaluation of our proposed method.
- Security Evaluation: This folder consists of notebooks to perform the evaluation of our proposed method against non-image data.
