# **Explainable Misinformation Detection with LLMs**

Welcome to the **Explainable Misinformation Detection** project! This system focuses on identifying misinformation in text while providing meaningful explanations behind the detection. I used attention visualization, counterfactual reasoning, and saliency maps to give users insights into why certain text is flagged as misinformation and suggest more accurate alternatives.

## **Overview**

The rapid spread of misinformation is a growing challenge, and while machine learning models can detect misinformation, they often lack transparency. This project aims to bridge that gap by offering clear, explainable feedback on why a piece of text is identified as misinformation. 

And soooooo our model does the following!
1. First off, our system can identify whether a given text contains misinformation using a fine-tuned BERT model.
2. Secondly, our system focuses on attention visualization, which highlights the parts of the text that influenced the model’s decision.
3. Thirdly, our system achieves counterfactual Reasoning and so provide more accurate versions of the flagged text using a generative language model.
4. Lastly, with Salient Maps, I can pinpoint which tokens or phrases had the greatest impact on the model’s classification decision.

## **Features**

1. **Binary Classification**:
   - A BERT-based model is fine-tuned to classify text as either true or misinformation.
   - Uses datasets like LIAR or FEVER for training.

2. **Attention Visualization**:
   - Displays a heatmap over the input text, highlighting words or phrases that the model deemed important when classifying misinformation.

3. **Counterfactual Reasoning**:
   - Uses GPT-2 to propose alternative factual statements when misinformation is detected.
   - Helps users see what an accurate version of the text might look like.

4. **Saliency Maps**:
   - Provides another layer of explainability by visualizing which tokens contributed most to the model’s decision through saliency maps (e.g., Integrated Gradients).
