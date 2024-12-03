# Machine Learning-Driven Op-Amp Design with Explainable AI: A Transfer Learning Approach from TSMC N65 to SKY130
In the realm of analog integrated circuit (IC) design, the operational amplifier (op-amp) circuit, whose purpose is to amplify any differential signals, is a fundamental component of almost every circuit. Therefore, mastering op-amp design is essential for any analog circuit engineering. However, the complex, nonlinear relationship between the geometrical parameters (e.g., width and length) and the electrical characteristics of each Metal-Oxide-Semiconductor Field-Effect Transistor (MOSFET) within the op-amp makes it challenging to model a direct mathematical relationship between individual transistor attributes and circuit performance. Consequently, analog circuit design, including op-amp design, heavily relies on expert intuition to identify optimal transistor dimensions within an expansive design space. Further complicating this process, the electrical characteristics of transistors vary across technology nodes, requiring designers to adapt to new node-specific characteristics when transitioning designs to different technologies.

Addressing these challenges, in this project, we propose a black-box machine learning (ML) model called Extreme Gradient Boosting (XGBoost) to capture the relationship between component parameters and performance metrics in op-amp circuits. After training the black-box model, we employ an explainable artificial intelligence (XAI) technique called Shapley Additive Explanations (SHAP) to analyze how each component parameter impacts specific performance metrics, thereby providing actionable design insights. Additionally, this study incorporates transfer learning to bridge knowledge from TSMC N65 to the SKY130 technology node, facilitating efficient design adaptation to a new technology node.

Structure of this repository:
1. Folder 'Dataset': Containing the dataset used for training.
2. File 'Group35_Project.ipynb': Code of this project.
3. File 'Op-amp's schematic.png': Schematic of the employed op-amp circuit.

Main information of the project:
1. Language: Python
2. Libraries: pandas, numpy, sklearn, xgboost, shap, matplotlib.
3. Dataset: TSMC N65, SKY130

Contributor:
1. XiaoFeng Kuang - 2017365584​
2. Nguyen Quoc Thang - 202396764
