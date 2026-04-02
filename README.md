# FERPI: Flood Emergency Response Priority Intelligence 🌊🇱🇰

**Flood Emergency Response Priority Intelligence (FERPI)** is a multi-task Machine Learning project designed to enhance disaster management in Sri Lanka. By combining predictive environmental modeling with socio-economic data, FERPI provides actionable intelligence for prioritizing emergency resource allocation.

## 🚀 Key Project Tasks

The project implements a complete end-to-end ML pipeline across four distinct tasks:

1.  **Task 1: Flood Occurrence Classification**
    *   Predicts the binary likelihood of a flood event (Yes/No) based on internal meteorological indicators.
    *   **Best Model:** Hist Gradient Boosting (AUC-ROC: 0.9571).

2.  **Task 2: Flood Risk Intensity Regression**
    *   Predicts a continuous risk intensity score (0-100) for every location.
    *   **Best Model:** Hist Gradient Boosting (R² Score: 0.9952).

3.  **Task 3: Habitation Suitability Classification**
    *   Evaluates locations from a human safety perspective, categorizing areas as "Safe" or "Dangerous" for living based on infrastructure resilience.
    *   **Best Model:** Hist Gradient Boosting (Accuracy: 99.2%).

4.  **Task 4: Regional Risk Zonation (Clustering)**
    *   Uses Unsupervised Learning (K-Means & Agglomerative Clustering) to group Sri Lankan districts into response zones.

## 💡 Novel Contribution: ERAS Scoring
We developed the **Emergency Resource Allocation Score (ERAS)**. This formula integrates ML risk outputs with population density and infrastructure scores to automatically rank districts by their immediate need for rescue operations.

$$ERAS = (35\% \times \text{Risk}) + (25\% \times \text{Prob}) + (20\% \times \text{Vulnerability}) + (20\% \times \text{Zone Rank})$$

## 🛠️ Technology Stack
*   **Language:** Python
*   **Environment:** Jupyter Notebook
*   *Libraries:** Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn.
*   **Version Control:** Git & GitHub.

## 👥 Team Members
*   **Thivakar G** - (Member 1): Preprocessing, Tasks 1 & 3.
*   **Jathudshan** - (Member 2): EDA, Tasks 2 & 4.

## 📂 Project Structure
*   `FERPI_Sri_Lanka_Flood_ML.ipynb`: Full implementation code and visualizations.
*   `FERPI_Assignment_Report.docx`: Comprehensive academic report (Local Only).
*   `submission.txt`: Final submission meta-data.

---
*Developed for the Machine Learning (IT4060) Assignment.*
