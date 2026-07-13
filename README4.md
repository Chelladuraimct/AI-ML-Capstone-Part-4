# Part 4 – LLM Powered Feature

## Track Chosen

**Track C – Model Prediction Explanation Pipeline**

In this part, the best-performing machine learning model from Part 3 (`best_model.pkl`) will be loaded and used to generate predictions for three feature vectors.

The predicted class and probability will then be sent to an LLM through the OpenRouter API. The LLM will return a structured JSON explanation which will be validated using a JSON Schema.

This implementation includes:

- Secure API key handling
- Prompt engineering
- Structured JSON output
- JSON Schema validation
- PII Guardrails
- Temperature comparison (0 vs 0.7)
- End-to-end prediction explanation pipeline

# Part 4B – Load Best Model and Generate Predictions

In this section:

- Load the trained pipeline (`best_model.pkl`)
- Load the cleaned dataset
- Create three feature-vector inputs
- Predict class labels
- Predict class probabilities
- Implement a PII guardrail before every LLM call

# Project Summary

This project demonstrates the integration of a Machine Learning model with a Large Language Model (LLM) to generate explainable AI predictions for medical diagnosis.

## Components Developed

- Trained Random Forest classification model
- OpenRouter API integration
- Secure API key handling
- JSON schema generation and validation
- Structured LLM explanations
- Prompt engineering
- Response validation
- Safety guardrails for PII detection
- Temperature comparison
- Multi-record testing

## Results

- Machine Learning predictions were generated successfully.
- OpenRouter API returned structured JSON explanations.
- JSON schema validation passed.
- Safety filtering blocked sensitive patient information.
- Temperature experiments demonstrated deterministic and creative outputs.
- The complete Explainable AI pipeline executed successfully.

## Conclusion

The project successfully combines traditional Machine Learning with Large Language Models to provide interpretable predictions. The structured JSON output makes the explanations suitable for downstream applications while maintaining consistency through schema validation and safety guardrails.

# Final Conclusion

In this capstone project, an end-to-end Explainable AI (XAI) pipeline was developed by integrating a trained Machine Learning model with a Large Language Model using the OpenRouter API.

The workflow included:

- Medical data preprocessing
- Prediction using a Random Forest model
- Explanation generation using an LLM
- JSON schema validation
- Prompt engineering
- Safety guardrails
- Multi-record testing
- Temperature comparison

The generated explanations were returned in a structured JSON format, validated successfully, and demonstrated how Large Language Models can improve the interpretability of Machine Learning predictions.

This project highlights the practical application of Explainable AI for healthcare decision support while ensuring reliability, reproducibility, and responsible AI practices.
