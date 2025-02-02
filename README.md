# Topsis-for-Pretrained-Models--102203846

This project applies the TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) method to evaluate and rank pre-trained text generation models based on multiple performance criteria. The analysis identifies the best model by calculating its closeness to the ideal solution using normalized criteria and weights.

# Project Overview

In this study, several text generation models are evaluated based on the following criteria:

Perplexity: Lower is better (indicates better model performance). <br>
BLEU Score: Higher is better (measures n-gram overlap between the generated text and reference text). <br>
ROUGE Score: Higher is better (measures recall and overlap of sequences). <br>
Latency: Lower is better (time taken to generate text). <br>
Memory Usage: Lower is better (indicates model efficiency). <br>
The TOPSIS method is used to rank these models by:

Normalizing the criteria values.
Assigning weights to each criterion.
Calculating the ideal best and worst solutions.
Determining the closeness coefficient for each model.

# Visualizations
Heatmap of Normalized Criteria: <br>
Shows how each model performs across all criteria.

Radar Chart: <br>
Visualizes the multi-criteria performance of each model.

Bar Plot for Criteria Contribution: <br>
Highlights the contribution of each criterion to the rankings.

Scatter Plot of Rankings vs Closeness Score: <br>
Displays the relationship between the closeness coefficient and the model rankings.

Box Plot of Criteria Spread: <br>
Shows the distribution of normalized values for each criterion.

# Methodology
TOPSIS Steps: <br>
1.Normalize the criteria using vector normalization. <br>
2.Multiply by weights to get the weighted normalized decision matrix. <br>
3.Calculate the ideal best and worst solutions. <br>
4.Compute the Euclidean distance to the ideal solutions. <br>
5.Calculate the closeness coefficient. <br>
6.Rank models based on Ci. <br>

# Results
Best Model: The model with the highest closeness coefficient. <br>
Insights: <br>
Models with a lower perplexity and latency but higher BLEU and ROUGE scores tend to rank higher. <br>
Memory efficiency also plays a significant role in determining the best model.

# Contributing
Feel free to open issues or submit pull requests to improve the project.

# License
This project is licensed under the MIT License.


