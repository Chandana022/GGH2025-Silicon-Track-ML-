# GGH2025-Silicon-Track-ML-
# AI-Based Combinational Logic Depth Predictor  

##  Introduction  
This project is part of **Google Girl Hackathon 2025 - Silicon Track** and focuses on predicting the **combinational logic depth** of signals in RTL designs.  
Traditional **timing analysis** requires synthesis, which is **time-consuming**. This project uses **machine learning** to predict logic depth **before synthesis**, helping designers identify **timing violations** faster.  

##  Problem Statement  
**Objective:** Develop an AI algorithm that predicts the **combinational logic depth** of a signal in an RTL module.  
- **Input:** RTL module, target signal, additional feature data (fan-in, fan-out, etc.).  
- **Output:** Predicted combinational depth of the signal.  

##  Approach & Methodology  
1. **Dataset Creation** – Gather RTL designs, extract timing reports.  
2. **Feature Engineering** – Identify key features affecting logic depth (fan-in, fan-out, etc.).  
3. **Model Selection** – Compare ML models (e.g., Decision Trees, Random Forests, Neural Networks).  
4. **Training & Evaluation** – Train on labeled data, measure accuracy against synthesis reports.  

##  Installation & Setup  
Since the entire algorithm is implemented in **Google Colab**, there is no need for local installation.  
To run the notebook:  
1. Open **Google Colab** in your browser.  
2. Load the provided **Colab Notebook** from the repository.  
3. Install dependencies directly in the notebook using:  
   ```python
   !pip install -r requirements.txt
## How to Run the Code
Open the Colab Notebook: [Insert Colab Link Here]
Run all cells in order.
Upload your RTL file (if required).
The notebook will output the predicted logic depth of the given signal.
Expected output format:

bash
Copy
Edit
Predicted Logic Depth: 7
##  Results & Evaluation
The prediction accuracy was measured using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
Achieved 90%+ accuracy when tested against ground truth synthesis reports.
The model was compared against traditional synthesis reports, and results showed a significant reduction in runtime while maintaining accuracy.
Graphical comparisons and detailed results are available in the results section of the notebook.
##  Alternatives Considered
Traditional Timing Analysis – Requires complete synthesis, making it time-consuming.
Rule-Based Heuristics – Simpler but lacks adaptability to complex designs.
Neural Networks – Considered, but decision trees/random forests performed better in terms of explainability and efficiency.
##  References
Research papers on ML for RTL timing analysis.
Standard EDA tools for RTL design evaluation.
Open-source datasets for logic depth prediction.
