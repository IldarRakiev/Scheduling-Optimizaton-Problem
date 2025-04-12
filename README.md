# Scheduling Optimization using Artificial Immune System (AIS)

This project aims to solve the **scheduling optimization problem** from the Kaggle competition "Santa's Workshop Tour 2019". The goal is to assign 5,000 families to 100 days before Christmas, **minimizing total cost** while satisfying strict constraints on daily occupancy. We implemented a hybrid **Artificial Immune System (AIS)** algorithm enhanced with **Simulated Annealing** and smart heuristics. The solution outperforms standard **Genetic Algorithms (GA)** and **Artificial Bee Colony (ABC)** methods and was validated through Kaggle's official evaluation system. Best score obtained using algorithm is **3,871,232.87** .

## Repository Structure

```text
.
├── data/
│   ├── family_data.csv           # Dataset provided by Kaggle
│   └── formula.png               # Visual explanation of cost function
│
├── optimization algorithms/
│   ├── abc.ipynb                 # Artificial Bee Colony implementation
│   └── ga.ipynb                  # Genetic Algorithm implementation
│
├── raw_implementations/
│   ├── raw_algorithm.ipynb       # Initial naive algorithm
│   └── raw_algorithm_new_functions.ipynb  # Early improvements and function testing
│
├── Reports/
│   ├── NIC_Project_proposal.pdf  # Proposal describing early plan and goals
│   └── NIC_Report.pdf            # Final report with methodology, experiments, and conclusions
│
├── AIS Implementation.ipynb      # Full and final AIS implementation with hybrid enhancements
│
├── best_solution.csv             # Final optimized solution (submitted to Kaggle)
│
├── README.md
|
└── LICENSE                       # Project license file
```


## How to run the project

1. **Requirements**: Ensure you have Python 3.7+ and Jupyter Notebook installed.

2. **Install Dependencies** (if needed):
   ```bash
   pip install numpy pandas matplotlib
   ```

3. **Run the AIS Algorithm**:
   Open the notebook:
   ```
   AIS Implementation.ipynb
   ```
   Run all cells to execute the complete optimization pipeline and view the results.

4. **Compare with other algorithms**:
   You can explore and run `ga.ipynb` and `abc.ipynb` inside the `optimization algorithms` folder to compare results and behavior.


## 📌 Notes

- The final solution in `best_solution.csv` is fully constraint-satisfying and Kaggle-evaluated.
- The `raw_implementations` folder provides insight into the iterative development process.
- The `Reports` folder contains a detailed write-up of experiments and observations.
