# Modulation of Optic System for MNIST Digit Classification

This project is a simulation of an optic system that can classify MNIST digits 0-3 using Fraunhofer diffraction. The classification is made by calculating the intensity of each quarter on the output screen, where every quarter represents a digit 0-3. The optimal mask for the optic system is found using an optimization algorithm called genetic algorithm.

## Prerequisites

- Python 3.x
- NumPy
- Matplotlib
- Scipy
- Jupyter

## Installation

1. Clone the repository: 

```
git clone https://github.com/yoavscode/optic-system-classifier.git
```

2. Navigate to the cloned directory: 

```
cd optic-system-classifier
mkdir train
```

3. Download MNIST csv dataset from [here](https://www.kaggle.com/datasets/oddrationale/mnist-in-csv)

4. Copy dataset to train folder:

```
cd Downloads
cp mnist_train.csv optic-system-classifier/train/
```

5. Install the required packages: 

```
pip install numpy matplotlib scipy jupyter
```

## Usage

To try out the optic system for yourself, open the Fraunhofer.ipynb file in Jupyter Notebook and run the cells. The notebook includes explanations of the code and visualizations of the classification results.

This will generate a plot of the intensity distribution on the output screen for each digit 0-3, as well as the final classification accuracy. The program will also output the optimal mask for the optic system.

## Optimization

The genetic algorithm is used to find the optimal mask for the optic system. The algorithm starts with a population of randomly generated masks, and then iteratively evolves the population by selecting the fittest individuals and combining their characteristics through crossover and mutation. The fitness function used is the classification accuracy of the optic system.

The default genetic algorithm parameters are:

- Population size: 20
- Number of generations: 2500
- Mutation rate: 0.1

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
