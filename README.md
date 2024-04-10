# PASA: Attack Agnostic Unsupervised Adversarial Detection using Prediction \& Attribution Sensitivity Analysis

Repository for the paper "PASA: Attack Agnostic Unsupervised Adversarial Detection using Prediction \& Attribution Sensitivity Analysis," accepted at 9th IEEE European Symposium on Security and Privacy. This paper proposes an adversarial detection of images and non-image data using two statistics at test time: feature attribution and model prediction sensitivity. 

The directory consists of the following folders:
- Ablation Study: This folder consists of notebooks for running an ablation study to measure how each of our statistical measures performs in adversarial detection when used standalone.
- Adaptive Attack: This folder consists of notebooks for performing adaptive attacks on the target model when an adversary knows about the defense.
- Evaluation: This folder consists of notebooks to perform the evaluation of our proposed method on image data.
- Security Evaluation: This folder consists of notebooks to perform the evaluation of our proposed method against adversarial attacks on non-image data.
