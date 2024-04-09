# PASA: Attack Agnostic Unsupervised Adversarial Detection using Prediction \& Attribution Sensitivity Analysis

Instead of just using a single threshold for comparision, PASA computes two metrics (prediction sensitivity and attribution sensitivity). See paper for details. In addition, PASA learns a lower and upper bounded threshold of $[\eta_1, \eta_2]$ for both metrics from the benign datasets. This helps improve the detection of adversarial samples significantly. At the moment, we follow an empirical approach to find the lower and upper bound of the metrics based on their distributions. We plan to design an automated tool to find the best threshold in future works.

Assume that PASA ($\phi$(.)) needs to evaluate a test instance $\textbf{x}$, then it first computes prediction sensitivity ($S_1$(.)) and attribution sensitivity ($S_2$(.)). During training, we learn the upper-lower bound for both metrics from benign datasets. Then, at test time, we decide if a sample is adversarial if either of the metrics does not satisfy the threshold i.e.

$$
\phi(\textbf{x}) = 1[S_1(\textbf{x})>\eta_2~\textnormal{or}~S_1(\textbf{x}) < \eta_1]
$$

\textbf{OR}

$$
\phi(\textbf{x}) = 1[S_2(\textbf{x})>\alpha_2~\textnormal{or}~S_2(\textbf{x}) < \alpha_1]
$$
