# Navigating Tomorrow
Navigating Tomorrow: Assessing Large Language Models in Event Prediction


## Datasets Overview

This repository includes three datasets utilized in the thesis project "Navigating Tomorrow: Assessing Large Language Models in Event Prediction." 
Each dataset is created to analyze different aspects of event prediction and model evaluation.

### Common Dataset Structure
- **Categories**: Articles in each dataset are divided into three main entity types:
  - **Organizations (ORG)**
  - **Locations (LOC)**
  - **Persons (PER)**
- **Details**:
  - **Events Count**: Lists the number of events before and after the model's training cut-off.
  - **Entities Count**: Total count of unique entities.
  - **Split Result**: Categorization into "popular" based on entity popularity scores (Wikipedia Pageview Analytics), with counts and detailed event information.

### 1. **news_dataset.json**
- A comprehensive collection of news articles that serves as the primary source for evaluating models' performances.

### 2. **counterfactual_news_dataset.json**
- Sample of the **news_dataset.json**. It contains news articles altered to create counterfactual scenarios to test model abilities in discerning and reacting to modified events.

### 3. **reasoning_news_dataset.json**
- Sample of the **news_dataset.json**. It focuses on scenarios requiring reasoning to predict outcomes, challenging the models' capabilities beyond factual recall.

### Model Responses
- Each dataset entry includes responses from various models regarding the likelihood of certain events occurring.
- **Models Included**:
  - **Llama2 7b**
  - **Llama2 70b**
  - **Gemma 7b**
  - **GPT-3.5 Turbo**
  - **Mistral 7b**
  - **Mixtral 8x7b**
- **Responses**: Models provide answers like "yes" or "no" to predict events' occurrence, detailed for scenarios before and after the training cut-off.

