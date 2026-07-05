# ARMA
ARMA: Adversarially Robust Malware Attribution with Global Perturbations and Adversarial Consistency Regularization
# Abstract
Attributing APT (Advanced Persistent Threat) malware
to their respective groups is crucial for threat intelligence
and cybersecurity. However, APT adversaries often conceal their
identities, rendering attribution inherently adversarial. Existing
machine learning-based attribution models, while effective, remain
highly vulnerable to adversarial attacks. For example, the
state-of-the-art byte-level model MalConv sees its accuracy drop
from over 90% to below 2% under PGD (Projected Gradient
Descent) attacks. Existing gradient-based adversarial training
techniques for benign/malicious malware detection or image
processing were adapted to malware attribution in this study,
revealing that both robustness and training efficiency require
significant improvement. To address this, we propose ARMA, a
novel single-step adversarial training approach that integrates
global perturbations to generate enhanced adversarial samples
and employs adversarial consistency regularization to improve
representation quality and resilience. We further provide a
theoretical analysis explaining how global perturbations converge
to reusable class-specific patterns and how the combined consistency
and distribution alignment losses strengthen a marginbased
robustness condition, thereby justifying the design of
ARMA. A novel APT malware dataset named AMG18, featuring
diverse samples and realistic class imbalances, is introduced
for evaluation. Extensive experiments show that ARMA consistently
outperforms nine competing methods—including five
adversarial-training methods, two defense-oriented methods, and
two non-adversarial baselines—in both adversarial robustness
(e.g., achieving over 80% Robust Accuracy and outperforming
the next-best method by more than 10 percentage points under
PGD attacks) and training efficiency (e.g., over twice as fast as
multi-step PGD-based approaches), while maintaining superior
Standard Accuracy in non-adversarial scenarios. The ARMA trained attribution model and the AMG18 dataset are publicly
available at https://github.com/Yuxia-Sun/ARMA.

## Repository Structure

- `Model/` — trained model parameters (`ARMA.ckpt`)
- `Samples/` — sample files for visualization
