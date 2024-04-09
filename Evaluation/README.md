# PASA: Attack Agnostic Unsupervised Adversarial Detection using Prediction \& Attribution Sensitivity Analysis

Instead of just using a single threshold for comparision, PASA computes two metrics (prediction sensitivity and attribution sensitivity). See paper for details. In addition, PASA learns a lower and upper bounded threshold of $[\eta_1, \eta_2]$ for both metrics from the benign datasets. This helps improve the detection of adversarial samples significantly. At the moment, we follow an empirical approach to find the lower and upper bound of the metrics based on their distributions. We plan to design an automated tool to find the best threshold in future works.

$$
\phi(\textbf{x}) = 1[S(\textbf{x})>\eta_2~\textnormal{or}~S(\textbf{x}) < \eta_1]
$$