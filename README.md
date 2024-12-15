# NLP Project

# **AI-Generated Content Detection: A Transformer-Based Approach**

## **Project Overview**
This project explores the detection of machine-generated text using three powerful transformer-based models: **BERT**, **RoBERTa**, and **T5**. With the rise of AI-generated text, our goal was to create a robust system that can differentiate between human-written and machine-generated content. We fine-tuned pre-trained models on labeled datasets and evaluated their performance across key metrics, such as accuracy, precision, recall, and F1-score.

## **Models Used**
- **BERT**: Bidirectional Encoder Representations from Transformers.
- **RoBERTa**: An optimized variant of BERT with improved training strategies.
- **T5**: Text-to-Text Transfer Transformer, a versatile model treating all NLP tasks as text generation.

## **Methodology**
We followed a systematic approach to develop and evaluate the models:
1. **Data Preparation**:  
   - Preprocessed and tokenized datasets.
   - Assigned binary labels: "Human-Written" (0) and "Machine-Generated" (1).

2. **Model Training**:  
   - Fine-tuned BERT, RoBERTa, and T5 using hyperparameters like batch size, learning rate, and epochs.
   - Monitored training and validation loss for convergence.

3. **Evaluation**:  
   - Assessed models using performance metrics: accuracy, precision, recall, F1-score, and confusion matrices.
   - Analyzed results to identify challenges and areas for improvement.

## **Results**
| **Model**   | **Accuracy** | **Precision** | **Recall** | **F1-Score** | **F1 Macro** |
|-------------|--------------|---------------|------------|--------------|--------------|
| **BERT**    | 78.1%        | 75.04%        | 94.16%     | 83.27%       | 75.46%       |
| **RoBERTa** | **81.0%**    | **83.0%**     | **81.0%**  | **79.0%**    | **77.0%**    |
| **T5**      | 73.0%        | 73.0%         | 73.0%      | 71.0%        | 70.0%        |

- **RoBERTa** outperformed other models with the best balance of precision and recall.
- Challenges included misclassifying human-written text as machine-generated, resulting in high false positives.

## **Challenges Faced**
- **Dataset Limitations**: Limited size and lack of diverse machine-generated text examples impacted the models' generalizability.
- **Hyperparameter Optimization**: Identifying the ideal combination of learning rate, batch size, and epochs required multiple experiments.
- **False Positives**: All models struggled to differentiate human-written text from machine-generated, highlighting a common challenge in NLP.

## **Future Improvements**
- Expanding the dataset with more diverse and larger examples.
- Exploring **ensemble models** combining the strengths of BERT, RoBERTa, and T5.
- Fine-tuning on multilingual datasets for broader applicability.
- Implementing **explainability techniques** to better understand model predictions.

