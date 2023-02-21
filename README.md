# Aliaidar_Alikhan_advancedProgramming_finalProject

Report

Introduction:
    Problem:
        There are various methods to solve the time-dependent Schrodinger equation, and one of the most popular ones is to use a machine learning model like a recurrent neural network (RNN) with Long Short-Term Memory (LSTM) units. In this report, I present our work on using an RNN-LSTM to predict the quantum state of a spin-half particle in a magnetic field over time.
    Literature review with links:
        https://www.hershsingh.net/notes/qcipu_2021.pdf
        https://en.wikipedia.org/wiki/Pauli_matrices
        https://uwaterloo.ca/physics-of-information-lab/sites/ca.physics-of-information-lab/files/uploads/files/aqm_lecture_notes_75.pdf
        https://en.wikipedia.org/wiki/Hamiltonian_(quantum_mechanics)
        https://www.youtube.com/playlist?list=PLUl4u3cNGP61-9PEhRognw5vryrSEVLPr https://www.researchgate.net/publication/222301414_Numerical_approaches_to_time_evolution_of_complex_quantum_systems
    Current work:
        The problem in this project is predicting the evolution of a quantum state of a spin-half particle in a                                                                         magnetic field over time. In this report, I present my work on using an RNN-LSTM to predict the quantum state of a spin-half particle in a magnetic field over time. The RNN with LSTM is a good model for this problem because it is designed to handle sequential data and can capture dependencies over time. In the case of the quantum state evolution problem, the evolution of the quantum state over time can be seen as a sequence of states, where the state at time t depends on the state at time t-1. I also provide a literature review of other solutions to the problem and describe our current work.

Data and methods:
    Information about the data:
        Generated synthetic data using Hamiltonian Here, I simulate a qubit using the Pauli matrices. The initial state is |0>, and the time evolution is given by e^(-iHt), where H is the Hamiltonian and t is the time. I created a dataset of 1000 samples, each representing the state of a spin-half particle at a specific time. The particle is in a magnetic field with a magnitude of 1 in the z-direction. The time interval between samples is 0.01. We split the dataset into training and testing sets with a ratio of 8:2. We used the training set to train the RNN-LSTM model.
    Description of the ML models you used with some theory: 
        I used the RNN-LSTM model to predict the evolution of the quantum state of the spin-half particle over time. The RNN is a type of neural network that has feedback connections. This allows the network to use its previous outputs as inputs for the current time step. An LSTM is a type of RNN that can selectively remember or forget information from the previous time step. This makes it suitable for modeling time series data like the quantum state of the spin-half particle.
    Results:
        The model was able to predict the evolution of the quantum state of the spin-half particle with high accuracy.I also visualized the true and predicted quantum state of the spin-half particle over time using a line plot. The plot showed that the predicted state closely matched the true state.
    Discussion:
        The RNN-LSTM model was able to accurately predict the evolution of the quantum state of a spin-half particle in a magnetic field over time. The model was able to achieve high accuracy with a small dataset of 1000 samples. This demonstrates the effectiveness of using an RNN-LSTM for solving the time-dependent Schrodinger equation for a spin-half particle in a magnetic field.
    Next steps:
        In future, I can create a model for more complex systems with more accuracy. And maybe with convolutional neural network (CNN) or a Transformer for predicting the evolution of the quantum state.
