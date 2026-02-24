# Skin-Lesion-Classification
Skin Lesion classification using Computer Vision
Skin cancer remains a growing global health challenge, accounting for more than 1.5 million new cases annually [1]. Melanoma is the deadliest due to its aggressiveness if undetected [2].
Dermatoscopic examination has improved diagnosis but requires specialist expertise [3]. AI-based systems, especially CNNs, are increasingly applied in dermatology [5], but plain CNNs trained from scratch are limited on small, imbalanced datasets. 
Transfer learning with pretrained ResNet50 [6] enables better performance. HAM10000 [4] is a benchmark dataset with 10,015 dermoscopic images across seven diagnostic categories. Recent work reports >85% accuracy with transfer learning [7,8], but few studies compare plain CNNs vs ResNet50 with explainability.
Grad-CAM [9] enhances interpretability.

#Problem Statement
To implement a more robust and clinically reliable models that not only improve accuracy but also provide interpretability as in our experiments, a plain CNN baseline achieved only 62.6% test accuracy and a macro-F1 score of 0.43, with frequent misclassification of melanoma and basal cell carcinoma into benign categories.

#Objectives
To benchmark a baseline plain CNN against a transfer learning model (ResNet50) on the HAM10000 dataset.
To evaluate and compare both models using comprehensive metrics including accuracy, macro-F1, confusion matrices, and per-class performance.
To incorporate Grad-CAM visual explanations for ResNet50 predictions for clinical trust and interpretability

#Conclusion
ResNet50 significantly outperforms plain CNN on HAM10000 (accuracy 86.8% vs 62.6%). Macro-F1 improved to 0.80. 
Grad-CAM visualizations confirm lesion-focused attention, enhancing trust. The approach shows strong potential as a dermatology decision-support system. 
Future directions: address imbalance, external validation, explore ensembles.


