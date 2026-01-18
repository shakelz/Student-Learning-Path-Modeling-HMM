🎓 Human-Centric Student Path Modeling using Gaussian HMM
📍 Project Overview

Traditional Learning Management Systems (LMS) primarily focus on performance metrics, such as whether a student answered a question correctly. This project introduces a Human-Centric approach by analyzing the 'Mental State' and 'Language Fatigue' of learners.

Specifically designed with the context of international students in Berlin, our model captures the "hidden" exhaustion caused by language barriers and content overload. Using Gaussian Hidden Markov Models (HMM), the system dynamically recommends personalized learning resources based on the student's predicted cognitive state.
🧠 The Motivation: Beyond Grades

    The Language Barrier Tax: International students often experience higher cognitive loads when studying complex Data Science topics in a non-native language.

    Hidden Exhaustion: Burnout is a latent variable—it is not explicitly recorded in databases. We use sequential behavior to "decode" this hidden state.

    Content Overload: Instead of a linear path, we provide an adaptive one that knows when a student needs a "Recap Video" versus a "Research Paper."

🔬 Methodology & Model Comparison

We compared two distinct approaches to validate our results:
1. Baseline Model: K-Means Clustering

    Mechanism: Groups students based on the Euclidean distance of their activity metrics.

    Limitation: It is a "Static" model. It treats each day as an independent event and fails to capture the learning journey or historical context.

2. Proposed Model: Gaussian Hidden Markov Model (HMM)

    Mechanism: Models learning as a Sequential Process. It assumes the student's state today is influenced by their activity yesterday.

    Advantage: It identifies Latent (Hidden) States. By analyzing transition probabilities, the model accurately predicts when a student is moving from a "Steady" state into a "High-Load/Exhausted" state.

✨ Key Learning States & Personalized Recommendations

Our model identifies three primary hidden states:
State	Mental Condition	Characteristics	Recommendation
State 0	Steady	Balanced engagement, low fatigue.	Comprehensive Research Papers & Case Studies
State 1	At-Risk	Very low activity, disengaged.	Urgent Tutor Support & Motivational Content
State 2	High-Load	Peak engagement but high fatigue.	Short Visual Recap Videos (Low-effort)
📂 Dataset Information

This project utilizes the Open University Learning Analytics Dataset (OULAD).

    Source: UCI Machine Learning Repository - OULAD

    Features: We focused on studentVle.csv (Clickstream data) and studentInfo.csv (Demographics and Language Friction indicators).

🚀 Setup & Installation

    Clone the Repository:
    git clone https://github.com/shakelz/Student-Learning-Path-Modeling-HMM.git



Install Requirements:
Bash

    pip install -r requirements.txt

    Data Preparation: Download the OULAD dataset from the link above and ensure studentVle.csv and studentInfo.csv are in the project root directory.

    Run the Analysis: Open Student_Path_HMM.ipynb in Jupyter Notebook or VS Code and run all cells.

🛠 Tech Stack

    Language: Python 3.12

    Modeling: hmmlearn, scikit-learn

    Data Handling: pandas, numpy

    Visualization: matplotlib, seaborn

👨‍💻 Author

Abdul

    Masters in Data Science Candidate, Berlin, Germany.

    Interest: Educational Data Mining & Human-Computer Interaction.
