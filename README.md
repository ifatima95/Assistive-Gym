# Assistive-Gym: Reinforcement Learning for Personalized Assistive Tasks

Welcome to the **Assistive-Gym** project! This repository explores reinforcement learning (RL) techniques applied to assistive robotic tasks in a simulated environment. It evaluates the performance of advanced RL algorithms, optimizing task efficiency, safety, and adaptability.

---

## Overview

Assistive robotics plays a critical role in healthcare, where personalized and adaptive solutions are necessary to meet diverse patient needs. This project leverages the **Assistive Gym Framework** and evaluates the following RL algorithms:

- **Recurrent PPO**: A policy-based RL technique extended with recurrent neural networks for handling sequential decision-making.
- **DreamerV2**: A model-based RL approach that leverages latent world models for adaptability.
- **DreamerV3**: An advanced model-based RL technique with enhanced scalability and task efficiency.

These algorithms are tested across tasks like **bed bathing**, **feeding**, **drinking**, and **dressing**, using the following evaluation metrics:
1. **Mean Reward**: Measures task efficiency and overall performance.
2. **Mean Task Success**: Quantifies the success rate in completing the task.
3. **Mean Force**: Evaluates safety by monitoring physical interaction forces.

---

## Cloning and Installing Libraries

To set up the environment and perform experiments, the repositories for Assistive-Gym and each RL technique must be cloned, and their dependencies installed.

### Steps for Windows

1. Clone the **Assistive-Gym** repository:
   ```bash
   git clone https://github.com/Healthcare-Robotics/assistive-gym.git
   
2. Clone the required RL technique repositories:
      ```bash
      git clone https://github.com/Stable-Baselines-Team/stable-baselines3-contrib.git
      git clone https://github.com/jurgisp/pydreamer.git
      git clone https://github.com/danijar/dreamerv3.git
      git clone https://github.com/Farama-Foundation/D4RL.git

3.Install Miniconda or Anaconda for managing the Python environment.
4. Create a virtual environment:
    ```bash
     
       conda create --name myenv python=3.6
5. Activate the environment:
   ```bash
   conda activate myenv

6. Install required dependencies using pip:
   ```bash
   pip install -r requirements.txt

## Steps for Mac

1. Open Terminal and clone the Assistive-Gym repository:
     ```bash
     git clone https://github.com/Healthcare-Robotics/assistive-gym.git
2. Clone the required RL technique repositories:
     ```bash
     git clone https://github.com/Stable-Baselines-Team/stable-baselines3-contrib.git
     git clone https://github.com/jurgisp/pydreamer.git
     git clone https://github.com/danijar/dreamerv3.git
     git clone https://github.com/Farama-Foundation/D4RL.git

3. Install Homebrew for package management if not already installed:
     ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
4. Install Miniconda or Anaconda.
5. Create and activate the virtual environment as done in the Windows section.
6. Install required dependencies using pip:
7. pip install -r requirements.txt

## Potential Installation Issues

During installation, some common issues you might face include:
- Compatibility Issues: TensorFlow and Stable-Baselines must have matching versions. Verify the compatibility in their respective repositories.
- Missing pybullet Library: Install it manually if not included in the dependencies:
* pip install pybullet
* Algorithm-Specific Errors: If a specific RL technique fails, recheck the requirements.txt file or install the libraries manually.

## Approach

This project evaluates three RL techniques—Recurrent PPO, DreamerV2, and DreamerV3—on their ability to perform assistive tasks simulated in the Assistive-Gym environment.
- Key Steps:
1. Environment Setup: Configure the Assistive-Gym environment for each RL algorithm.
2. Training: Train each model using predefined hyperparameters optimized for assistive tasks.
3. Evaluation: Collect performance metrics such as:
* Mean Reward: Reflecting efficiency and task performance.
* Task Success Rate: Measuring the algorithm's ability to complete tasks.
* Mean Force: Evaluating safety through interaction forces.
4. Results for each model are stored in JSON files for further analysis.

## References

This project builds upon the following repositories and frameworks:
1.Assistive Gym Framework: [https://github.com/Healthcare-Robotics/assistive-gym]
2. Stable Baselines3 :[https://github.com/Stable-Baselines-Team/stable-baselines3-contrib]
3. PyDreamer: [https://github.com/jurgisp/pydreamer]
4. DreamerV3: [https://github.com/danijar/dreamerv3]

## Contributions

This project was developed by Fatima Alderazia as part of ongoing research in assistive robotics. Contributions are welcome! Feel free to fork the repository, open issues, or submit pull requests.
