# Machine-Learning-Based-Interpretation-of-Lip-Movements

This repository presents the complete implementation of machine learning based lip reading system developed as part of my undergraduate thesis. The model is designed to recognize spoken words by analyzing video frames of a speaker’s lip movements, utilizing the GRID dataset — a well-structured audio-visual corpus widely used in visual speech recognition (VSR) research.

The architecture combines **3D Convolutional Neural Network (3D CNN)** for spatiotemporal feature extraction with **Bidirectional Long Short-Term Memory (BiLSTM)** network for sequence modeling. The model is trained using **Connectionist Temporal Classification (CTC) loss** to handle unaligned input-output sequences at the character level. The input shape is `(75, 46, 140, 1)`, representing grayscale video frames over time.

This implementation includes:
- Data preprocessing (frame extraction, grayscale conversio,normalization, fixed-length padding)  
- Character-level tokenization
- Custom training loop with callbacks for learning rate scheduling, accuracy monitoring  
- Evaluation metrics including accuracy, precision, recall, F1 score, and confusion matrix  
- Visualization of training vs validation loss and character level accuracy

The goal is to achieve high accuracy, demonstrating effective speech recognition. This work has potential applications in silent communication, accessibility technologies, surveillance systems and so on.
