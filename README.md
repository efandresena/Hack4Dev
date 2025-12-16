# Hack4Dev
This repository host the pipeline created during the Hackathon in Astronomy to built a lihtweight image classifier for cubesats a little satelitte for downstream

# Description 
Our approach was ranked as one of the best 20 participants in the Hackathon in Astronomy. 
prototypes.

Our team’s goal was to design a lightweight yet accurate image classification solution suited for resource-constrained environments like CubeSatsModels were compared by accuracy, size, and computational load.

After several experiments, MobileNet-
like models emerged as the best trade-off between accuracy and efficiency.
Preprocessing included resizing images to fit model input, normalization to stabilize learning, and using the imblearn framework to address class imbalance. For the handcrafted pipeline, we extracted HOG features and tested CNN-based feature extraction combined with dimensionality reduction.

The final model, based on a MobileNet-like architecture, uses inverted residual blocks and Squeeze-and-Excitation modules to emphasize important features while keeping the model lightweight.

It was trained from scratch with tuned
hyperparameters to maximize accuracy without adding unnecessary complexity. Alternative pipelines using CNN-based feature extractors followed by SVM classifiers achieved decent accuracy but were slower and less suited for real-time
deployment.

Throughout the project, we focused on creating a model that is both efficient and robust for deployment on small
satellites. After comparing different strategies, we concluded that the MobileNet-like architecture best balanced size,
speed, and accuracy, aligning with our initial goal of a lightweight yet effective solution.

**B.8 Team08(3/3)**

This work was done in collaboration as a team with 3 members:
- Mirindra Randriamanantena(My self)
- Member 2
- Member 3
