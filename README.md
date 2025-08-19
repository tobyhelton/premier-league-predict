# Premier League Goal Line Prediction (R Project)

## Project Overview
This project applies **predictive modeling in R** to forecast whether Premier League matches will finish **over or under the 2.5 and 3.5 goal lines**.  

To evaluate the practical application of the model, I simulated a simple betting strategy:
- Bet **$10** on the model’s prediction for each line (2.5 and 3.5 goals).  
- Tracked **profits and losses** across matches in an Excel results sheet.  

---

## 🔧 Tech Stack
- **Language:** R  
- **Libraries:** `tidyverse`, `dplyr`, `tidymodels`, `tidylog`, `yardstick`, `rsample`, `stringr`, `recipes`, `kknn`, `zoo`  
- **Tools:** RStudio, Excel  

---

## Workflow
1. **Data Collection & Preparation**
   - Imported historical Premier League match results from footystats.org (`premier_stats24-25.xlsx`).  
   - Engineered features such as recent goal trends, home/away averages, and head-to-head goal history.  
   - Prepared outcome labels for **over/under 2.5 goals** and **over/under 3.5 goals**.  

2. **Modeling**
   - Built classification models for each goal line threshold:  
     - Logistic Regression  
     - Random Forest  
     - KNN  
   - Optimized hyperparameters with cross-validation.  

3. **Prediction & Evaluation**
   - Stored predictions in a results Excel file (`Predictions 2.xlsx`).  
   - Recorded whether each prediction was correct and tracked simulated betting results.  
   - Evaluated model performance using accuracy, precision/recall, and betting ROI.  

---

## 📊 Results
- **Best Model:** [KNN].  
- **Accuracy:**
  - 67% Across the 2.5 and 3.5
  - 2.5 Only: 58%
  - 3.5 Only: 73%   
- **Simulated Betting Performance:**  
  - Over/Under 2.5 goals → Profit/Loss: $[223 Profit]  
  - Over/Under 3.5 goals → Profit/Loss: $[35 Profit]  
- **Insights:**  
  - Models performed better on [2.5] line.  
  - Betting simulation showed [profitable] return compared to random guessing.  

---

## 📂 Repository Structure

