<h1>Facial Emotion Analysis for Recruitment Assessments</h1>


<h2>Project Overview</h2>
This project leverages deep learning techniques to analyze facial expressions and classify them into seven emotions: angry, disgust, fear, happy, sad, surprise, and neutral. The model's primary application is in recruitment assessments, where it can provide deeper insights into a candidate’s emotional state, engagement, stress levels, and behavioral reactions during an interview or aptitude test. This helps recruiters assess candidates' resilience and emotional responses, which are important for certain job roles. 
<br />

<h2>Objective</h2>
- To classify facial expressions into seven emotions: angry, disgust, fear, happy, sad, surprise, and neutral.<br />
- To provide insights into a candidate's emotional resilience, stress levels, and engagement during assessments.<br />
- To enhance the recruitment process by incorporating emotional analysis alongside cognitive skills tests.<br />

<h2>Languages and Utilities Used</h2>
- Python & PyTorch<br />
- Deep Learning Model: Vision Transformer (ViT)<br />
- Data Manipulation & Analysis: Pandas, NumPy<br />
- Model Training & Evaluation: torch, timm, sklearn<br />
- Visualization: Matplotlib, Seaborn<br />

<h2>Data Sources</h2>
- FER-2013 Dataset: 35,887 images of facial expressions categorized by emotion.<br />
- AffectNet Dataset: 34,553 images annotated with facial emotions.<br />
- MMA Facial Expression Dataset: 127,680 images across multiple categories.<br />

<h2>Program Walk-Through</h2>

<h3>1. Data Preparation</h3>
- Load and clean the datasets by removing irrelevant features and performing basic image preprocessing.<br />
- Normalize and augment the data (e.g., using transformations like rotation and flipping) to increase model robustness.<br />
- Split the data into training, validation, and test sets.<br />

<h3>2. Model Training</h3>
The model is based on Vision Transformer (ViT), trained to predict facial expressions. Key steps include:<br />
- <b>Model Architecture:</b> Vision Transformer (ViT) with fine-tuning for emotion classification.<br />
- <b>Optimization:</b> Hyperparameters were tuned for better model performance (e.g., learning rate, weight decay).<br />
- <b>Cross-Validation:</b> Used to evaluate the model on different data folds and reduce overfitting.<br />

<h3>3. Model Evaluation & Results</h3>
- <b>Performance Metrics:</b> The model achieved a weighted accuracy of 72.55% on the test set.<br />
- <b>Confusion Matrix:</b> Revealed that emotions like "disgust" and "fear" were difficult to classify, leading to misclassifications.<br />
- <b>Challenges:</b> Variations in lighting, pose, and occlusions contributed to inaccuracies, and data imbalance (with underrepresented emotions) impacted performance.<br />

<h3>4. Insights</h3>
- <b>Recruitment Application:</b> The model provides valuable insights into candidates' emotional responses, such as engagement and stress levels during assessments.<br />
- <b>Model Strengths:</b> The model performed well with emotions like “neutral” (84.74%) and “happy” (78.70%).<br />
- <b>Areas for Improvement:</b> Emotions like “disgust” (45.66%) and “fear” (57.95%) need further model tuning and additional data.<br />


