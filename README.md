# PRE-TRAINED-MODEL
# TOPSIS Analysis for Text Sentence Similarity Models

## Introduction
This analysis employs the Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS) to evaluate and rank different pre-trained models for text sentence similarity tasks. TOPSIS is a multi-criteria decision making method that helps identify the best alternative that has the shortest geometric distance from the positive ideal solution and the longest geometric distance from the negative ideal solution.

## Methodology

### Selected Models
The analysis evaluates five popular pre-trained models:
1. BERT-base: A widely used transformer-based model
2. RoBERTa: An optimized version of BERT
3. SBERT: Specialized sentence embedding variant of BERT
4. Universal Sentence Encoder: Google's sentence embedding model
5. SimCSE: Contrastive learning-based sentence embeddings

### Evaluation Criteria
Five key criteria were considered with different weights based on their importance:

1. Accuracy (35% weight)
   - Measures the model's performance in sentence similarity tasks
   - Higher values are preferred
   - Benchmark scores based on standard datasets

2. Inference Speed (20% weight)
   - Measured in milliseconds per inference
   - Lower values are preferred
   - Critical for production deployment

3. Model Size (15% weight)
   - Measured in megabytes
   - Lower values are preferred
   - Impacts deployment flexibility and resource requirements

4. Training Cost (15% weight)
   - Relative units considering computational resources
   - Lower values are preferred
   - Important for fine-tuning and adaptation

5. Maintenance (15% weight)
   - Scored on a scale of 1-10
   - Higher values are preferred
   - Considers ease of updates, community support, and documentation

### Implementation Details

The TOPSIS analysis follows these steps:

1. Decision Matrix Creation
   - Raw data normalized to allow comparison across different units
   - Each criterion scaled appropriately

2. Weighted Normalization
   - Weights applied to normalized values
   - Reflects the relative importance of each criterion

3. Ideal Solutions
   - Positive ideal: Best values for each criterion
   - Negative ideal: Worst values for each criterion

4. Distance Calculation
   - Euclidean distances computed from both ideal solutions
   - Considers all criteria simultaneously

5. Final Scoring
   - Relative closeness to ideal solution calculated
   - Scores range from 0 to 1 (higher is better)

## Results

### Model Rankings
The TOPSIS analysis yielded the following rankings (from highest to lowest score):
1. RoBERTa (0.723)
2. BERT-base (0.689)
3. SimCSE (0.654)
4. SBERT (0.621)
5. Universal Sentence Encoder (0.587)

### Key Findings

1. Performance vs. Efficiency Trade-off
   - RoBERTa leads despite larger size due to superior accuracy
   - Universal Sentence Encoder shows efficiency but lower accuracy

2. Resource Considerations
   - Lighter models (SBERT, USE) offer good maintenance scores
   - Heavier models (RoBERTa, BERT) require more resources but provide better accuracy

3. Practical Implications
   - RoBERTa recommended for accuracy-critical applications
   - Universal Sentence Encoder suitable for resource-constrained environments
   - BERT-base offers good balance of performance and resource usage

## Conclusion
The TOPSIS analysis reveals RoBERTa as the optimal choice when considering all criteria, though the final selection should consider specific use case requirements and constraints. The analysis provides a structured framework for model selection based on multiple practical considerations.
## Results:

![image](https://github.com/user-attachments/assets/78391acf-dcbe-40ee-b1a9-9c4b44ea55f0)
## Graph:

![image](https://github.com/user-attachments/assets/e9fd9649-581a-4c0e-b1f4-cdcdc6281cd9)
