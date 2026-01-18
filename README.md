<<<<<<< HEAD
# Student-Learning-Path-Modeling-HMM
A Gaussian HMM-based framework to model student learning paths by tracking mental fatigue and language friction. Includes a personalized recommendation engine for adaptive learning.
=======
🎓 Human-Centric Student Path Modeling using Gaussian HMM
📍 Project Overview

Traditional learning platforms (Coursera, Udemy) focus only on Performance (Right/Wrong answers). This project shifts the focus to the Human Element. We model the "Hidden" mental states of students—specifically Mental Fatigue and Language Friction—to provide personalized resource recommendations.

This is especially relevant for international students in Berlin, who face cognitive exhaustion due to language barriers while studying complex subjects like Data Science.
✨ Key Features

    Hidden State Detection: Uses Gaussian Hidden Markov Models (HMM) to identify latent states: Steady, At-Risk, and High-Load.

    Fatigue Scoring: A custom logic to calculate exhaustion based on cumulative interaction sequences.

    Language Friction Integration: Factors in the difficulty of learning in a non-native language.

    Smart Recommendations: Dynamically suggests content (e.g., Short Videos vs. Comprehensive PDFs) based on the predicted mental state.

🧠 The Model: Why HMM?

Unlike static clustering (like K-Means), HMM treats learning as a journey. It captures:

    Temporal Dependency: A student's state today depends on their behavior yesterday.

    Transition Probabilities: The likelihood of a student moving from a 'Steady' state to 'Burnout'.

Mathematical Foundation: The model calculates the optimal state sequence using the Viterbi algorithm:
S^=argSmax​P(S∣O,λ)
📊 Dataset

We utilized the OULAD (Open University Learning Analytics Dataset), focusing on:

    studentVle.py: For clickstream data and engagement tracking.

    studentInfo.py: For demographic and final result mapping.

🚀 Getting Started
1. Prerequisites

    Python 3.10+

    hmmlearn

    scikit-learn

    pandas, numpy, matplotlib, seaborn

2. Installation
Bash
>>>>>>> f17dd771 (Initial commit: Student Path HMM Project)
