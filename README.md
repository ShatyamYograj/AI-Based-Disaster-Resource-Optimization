# AI-Based-Disaster-Resource-Optimization

📌 Overview

Efficient disaster management requires rapid and optimal allocation of limited resources to multiple affected locations. This project presents an AI-based optimization framework that minimizes total travel distance while ensuring complete coverage of disaster-affected areas.

The system integrates:

Genetic Algorithm (GA) for route optimization

K-Means Clustering for spatial zoning

Constraint Satisfaction Problem (CSP) for feasibility enforcement

Benchmark experiments are performed using TSPLIB datasets, demonstrating significant distance reduction across different problem scales.

## 📌 Project Motivation

In disaster scenarios, delays in resource delivery can lead to loss of life and increased damage. Manual or greedy planning methods often fail to scale for large affected regions. This project is motivated by the need for intelligent, scalable, and data-driven decision-making tools that assist disaster response teams in planning efficient delivery routes under real-world constraints.

🎯 Objectives

Optimize disaster resource delivery routes

Minimize total travel distance and response time

Ensure realistic, constraint-compliant solutions

Evaluate scalability on small and large datasets

Provide quantitative performance analysis

🧠 Problem Description

Disaster resource routing closely resembles the Travelling Salesman Problem (TSP), which is an NP-Hard problem. As the number of affected locations increases, computing an exact optimal solution becomes computationally infeasible.

This project applies metaheuristic optimization techniques to efficiently compute near-optimal solutions under realistic constraints.

🧩 Algorithms Used
1️⃣ Genetic Algorithm (GA)

Used to evolve optimized routes through:
  
  - Population initialization
  
  - Fitness evaluation
  
  - Selection
  
  - Crossover
  
  - Mutation

Fitness Function:

  Fitness= 1/(Total Distance)

2️⃣ K-Means Clustering

Used to divide disaster locations into spatially coherent zones, improving:

  - Scalability
  
  - Realistic disaster planning
  
  - Optimization efficiency

3️⃣ Constraint Satisfaction Problem (CSP)

Ensures feasibility by enforcing:

  - Maximum travel distance constraints
  
  - Valid route generation
  
  - Rejection of infeasible solutions

📂 Dataset

The project uses TSPLIB benchmark datasets:

Dataset	    Locations	          Purpose
att48	         48	         Visualization & validation
a280	         280	       Scalability analysis

📌 Each dataset is processed individually, following standard research practice.

📊 Experimental Results
Dataset	    Initial Route      	Optimized Route	      Improvement
att48	      Random route	      GA optimized	          ~34%
a280	      Random route	      GA optimized	          ~13%

🔹 Improvement % decreases for larger datasets due to exponential growth in search space, which is expected for NP-Hard problems.

📈 Output Description

Small datasets (att48)

  Before vs After route visualization
    
  Clear demonstration of optimization

Large datasets (a280)

  Numerical analysis (distance & improvement %)
  
  Route visualization avoided due to clutter (research standard practice)

🛠️ Tech Stack

Programming Language: Python

Environment: Google Colab / Jupyter Notebook

Libraries:

NumPy

Matplotlib

Scikit-learn

Random

Math

🚀 How to Run the Project
1️⃣ Clone the repository
git clone https://github.com/your-username/disaster-resource-optimization.git
cd disaster-resource-optimization

2️⃣ Install dependencies
pip install numpy matplotlib scikit-learn

3️⃣ Run the notebook

Open the .ipynb file in Google Colab or Jupyter Notebook

Select the desired dataset (att48 or a280)

Run cells sequentially

📁 Project Structure
├── datasets/
│   ├── att48.tsp
│   ├── a280.tsp
├── src/
│   ├── data_loader.py
│   ├── ga_optimizer.py
│   ├── clustering.py
│   ├── constraints.py
├── results/
│   ├── plots/
│   ├── metrics/
├── README.md
└── main.ipynb

🧪 Evaluation Metrics

Total travel distance

Distance improvement percentage

Fitness convergence across generations

Runtime scalability

📌 Key Highlights

✔ Solves an NP-Hard real-world problem
✔ Uses hybrid AI optimization
✔ Quantitative, research-grade evaluation
✔ Scalable across dataset sizes
✔ Suitable for major final-year project

## ⚠️ Limitations

- Distances are calculated using Euclidean coordinates rather than real-world road networks.
- Full route visualization for large datasets becomes visually cluttered and is therefore avoided.
- The current implementation assumes a single delivery agent.
- Real-time traffic and dynamic disaster conditions are not considered.

🔮 Future Work

Multi-vehicle routing

GIS-based real-world distance mapping

Real-time traffic integration

Dynamic disaster scenario adaptation

Parallel GA implementation

👨‍💻 Author

Shatyam Yograj
Department of Information Technology

## 📜 License

This project is licensed under the MIT License and is intended for academic, research, and educational use.

⭐ If you find this project useful

Give it a ⭐ on GitHub — it really helps!
