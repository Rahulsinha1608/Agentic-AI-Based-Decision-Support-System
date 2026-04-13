# Agentic AI Based Decision Support System for Land Filling and Soil Recommendation

> 6th Semester Project | School of Computer Engineering  
> KIIT Deemed to be University, Bhubaneswar, Odisha – 751024  
> March 2026

---

## 📌 Overview

This project introduces an AI-powered decision support system that recommends the most appropriate soil type for land filling operations. By combining a **Random Forest machine learning model** with an **Agentic AI decision validation layer**, the system automates soil suitability assessment — a task traditionally reliant on manual GIS analysis and domain expertise.

The system is accessible through a simple, user-friendly **web interface**, making it usable by both technical and non-technical users such as planners and engineers.

---

## 👥 Team Members

| Name              | Roll Number |
|-------------------|-------------|
| Rahul             | 23052015    |
| Ritesh Kumar Singh| 23052017    |
| Adarsh Kumar      | 2305589     |
| Ashish Kumar      | 2305610     |

**Project Guide:** Dr. Raghunath Dey  
**Institution:** School of Computer Engineering, KIIT University

---

## 🎯 Objectives

- Build a system that suggests the right soil type for land filling based on environmental and terrain parameters.
- Automate soil suitability assessment using machine learning (Random Forest).
- Integrate an AI decision agent for rule-based validation of predictions.
- Provide an accessible web interface for end users without technical expertise.

---

## 🗂️ Dataset

| Parameter             | Value                                                                 |
|-----------------------|-----------------------------------------------------------------------|
| Total Samples         | 912                                                                   |
| Training Set          | 300 samples                                                           |
| Testing Set           | 612 samples                                                           |
| Input Features        | Temperature, Humidity, Rainfall, Soil Moisture, Distance from Coast, Longitude, Latitude, Groundwater Depth |
| Output                | Soil type recommendation with suitability score                       |
| Soil Classes          | Alluvial, Black, Laterite, Red                                        |
| Most Important Feature| Groundwater Depth                                                     |
| Second Important      | Distance from Coast                                                   |

---

## 🏗️ System Architecture & Methodology

The system is built around **6 core components**:

1. **Data Collection** – Soil and environmental data sourced from public soil databases and research datasets. Key factors: soil composition, slope, moisture, proximity to water bodies, and load demands.

2. **Data Preprocessing** – Missing value handling, outlier correction, numerical normalization, and feature selection to isolate the most impactful parameters.

3. **Model Training (Random Forest)** – An ensemble of decision trees is trained to learn the relationship between soil parameters and suitability classes.

4. **Soil Suitability Prediction** – The trained model predicts the appropriate soil type and outputs a suitability score based on user-provided land parameters.

5. **Agent-Based Decision Validation** – An AI agent applies environmental rules and constraints to validate and filter model outputs, ensuring recommendations are practical and trustworthy.

6. **Web-Based User Interface** – A clean, minimal web app where users input land parameters and receive soil recommendations with confidence scores.

---

## 📊 Model Performance

| Metric               | Value  |
|----------------------|--------|
| Accuracy             | 94%    |
| Precision            | 92%    |
| Recall               | 93%    |
| F1 Score             | 93%    |
| Correct Predictions  | 857 / 912 |
| Incorrect Predictions| 55 / 912  |

> The weighted average F1-score of **0.94** confirms reliable performance across most soil classes. Laterite soil showed comparatively lower performance due to limited training samples. Red soil had zero support in the test set.

---

## 🔍 Key Features

- **Machine Learning Core** – Random Forest classifier for accurate soil type prediction.
- **Agentic Validation** – Rule-based AI agent ensures outputs conform to real-world environmental constraints.
- **Explainability** – Feature importance analysis (Groundwater Depth and Distance from Coast are top predictors).
- **Web Interface** – User inputs land parameters; system returns soil recommendation + suitability score.
- **No GIS Expertise Required** – Unlike traditional methods, this system needs no specialized GIS software.

---

## 📈 Comparison with Existing Methods

| Method                             | Technique                              | Performance         | Limitation                          |
|------------------------------------|----------------------------------------|---------------------|--------------------------------------|
| GIS-Based DSS for Landfill         | GIS + AHP + WLC                        | Spatial index 0–10  | No ML; requires GIS expertise        |
| Random Forest Soil Classification  | Random Forest                          | R² ≈ 1.0            | Synthetic dataset; no recommendations|
| ML Land Suitability Assessment     | MLP Neural Network                     | Accuracy ≈ 99%      | Agriculture-focused only             |
| Explainable AI (Saudi Arabia)      | GIS + Fuzzy AHP + Bagging Ensemble     | R² ≈ 0.882          | Region-specific                      |
| Agentic AI for Smart Agriculture   | CNN + RF + XGBoost + XAI               | Accuracy + F1 Score | Depends heavily on dataset quality   |
| **Proposed System (This Project)** | **Random Forest + Agentic AI + Web UI**| **Accuracy ≈ 94%**  | Requires reliable environmental data |

**Advantage of this system:** It is one of the few that combines ML prediction, automated decision reasoning, and a web-accessible interface — making it practical for planners and engineers without technical backgrounds.

---

## 🧾 Research Gap Addressed

Existing literature is dominated by:
- GIS-based spatial analysis requiring specialized expertise.
- ML models that classify soil but stop short of actionable recommendations.
- Systems without user-friendly interfaces for non-technical users.

This project fills that gap by delivering an end-to-end system: from data input → ML prediction → agent validation → accessible recommendation output.

---

## 🔮 Future Scope

- Expand the dataset to cover more geographic regions for broader applicability.
- Integrate GIS maps for enhanced geographical visualization.
- Adopt more advanced ML models (e.g., XGBoost, deep learning) for higher accuracy.
- Add real-time data feeds for dynamic environmental conditions.

---

## 📚 References

1. [GIS-Based Environmental Decision Support System for Municipal Landfill Site Selection](https://www.emerald.com/meq/article-abstract/24/5/583/279135/GIS-based-environmental-decision-support-system?redirectedFrom=fulltext)
2. [Advanced Soil Classification Method Using Random Forest](https://www.mdpi.com/2076-3417/14/16/7202)
3. [Machine Learning Based Land Suitability Assessment](https://dergipark.org.tr/en/pub/nesciences/article/1569166)
4. [Advancements in Soil Quality Assessment – ML & AI Approaches](https://www.tandfonline.com/doi/abs/10.1080/00103624.2024.2406484)
5. [Human-Centric AI for Sustainable Development](https://www.mdpi.com/2078-2489/11/1/39)
6. [Explainable AI Framework for Landfill Site Selection (Saudi Arabia)](https://www.sciencedirect.com/science/article/pii/S2352186423004601)
7. [Residential Construction Site Selection Using XAI](https://www.mdpi.com/2071-1050/16/10/4235)
8. [Agentic AI Decision Support for Smart Agriculture](https://www.nature.com/articles/s41598-026-39472-w)
9. [Agricultural Land Suitability Classification in Semi-Arid Ecosystem](https://link.springer.com/article/10.1007/s10668-023-04440-1)

---

## 📄 License

This project was submitted in partial fulfilment of the requirements for the **Bachelor's Degree in Information Technology** at KIIT Deemed to be University. Academic use only.
