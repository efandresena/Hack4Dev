# Hack4Dev
This repository host the pipeline created during the Hackathon in Astronomy to built a lihtweight image classifier for cubesats a little satelitte for downstream

# Description 
Our approach were ranked as the best 20 participants in the Hackathon in Astronomy. 
**B.8 Team08(3/3)**
Our team’s goal was to design a lightweight yet accurate image classification solution suited for resource-constrained
environments like CubeSats. We explored several approaches to balance accuracy, model size, and inference speed.
We evaluated different CNN architectures and machine learning pipelines. MobileNetV3-like CNN provided
strong accuracy by using Squeeze-and-Excitation and inverted residual blocks. SqueezeNet offered a very compact
architecture with accuracy close to AlexNet but with 50× fewer parameters, matching our aim for deployment on
limited hardware. Classical pipelines combining CNN features or handcrafted features, such as HOG with SVM,
performed reasonably well but required more complex preprocessing and had slower inference.
We carried out extensive background research, consulted tutorials and papers, and iteratively built and tested
prototypes. Models were compared by accuracy, size, and computational load. After several experiments, MobileNet-
like models emerged as the best trade-off between accuracy and efficiency.
Preprocessing included resizing images to fit model input, normalization to stabilize learning, and using the
imblearn framework to address class imbalance. For the handcrafted pipeline, we extracted HOG features and tested
CNN-based feature extraction combined with dimensionality reduction.
The final model, based on a MobileNet-like architecture, uses inverted residual blocks and Squeeze-and-Excitation
modules to emphasize important features while keeping the model lightweight. It was trained from scratch with tuned
hyperparameters to maximize accuracy without adding unnecessary complexity. Alternative pipelines using CNN
feature extractors followed by SVM classifiers achieved decent accuracy but were slower and less suited for real-time
deployment.
Throughout the project, we focused on creating a model that is both efficient and robust for deployment on small
satellites. After comparing different strategies, we concluded that the MobileNet-like architecture best balanced size,
speed, and accuracy, aligning with our initial goal of a lightweight yet effective solution.

**B.8 Team08(3/3)**
This work was done in collaboration as a team with 3 members:
- Mirindra Randriamanantena(My self)
- Member 2
- Member 3
