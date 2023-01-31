# SOM-for-Clustering-Iris-Dataset

# Task

▸Aplicar um modelo neural não supervisionado

▸Avaliar os padrões detectados em cada conjunto:

▸Clusters / outliers, etc.

▸Avaliar a homogeneidade dos agrupamentos

▸Variar os parâmetros do modelo (grid, taxas, número
de neurônios, etc.)

# References:

* https://github.com/JustGlowing/minisom
* https://github.com/JustGlowing/minisom/blob/master/examples/BasicUsage.ipynb
* https://towardsdatascience.com/understanding-self-organising-map-neural-network-with-python-code-7a77f501e985

# Introduction
Information about Iris Dataset from https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_iris.html

* Classes: 3
* Samples per class: 50
* Samples total: 150
* Dimensionality: 4
* Features: real, positive

# Hyperparameters:

* x: x dimension of the SOM
* y: y dimension of the SOM
* input_len: number of the elements os the vectors in the input
* sigma: spread of the neighborhood function (sigma(t) = sigma / (1+t/T))
* learning_rate (learning_rate(t)=learning_rate/(1+t/T))
* decay_function (function that reduces learning_rate and sigma at each interaction)
* neighborhood_function (default=gaussian): function that weights the neighborhood of a position in the map
* topology (rectangular (default) or hexagonal)
* activation_distance: distance used to active the map (euclidean (default), consine,manhattan, chebyshev)

# Definitions

* Reference: Evaluating Self-Or aluating Self-Organizing Map Quality Measur ganizing Map Quality Measures as Conv es as Convergence Criteria (from Gregory T. Breard )

* Quantization error: is a measure of the average distance between the data points and the map nodes to which they are mapped, with smaller values indicating a better fit.

* Topographic error: TE is calculated by finding the best-matching and second-best-matching neuron in the map for each input and then evaluating the positions. If the nodes are next to each other, then we say topology has been preserved for this input. If not, then this is counted as an error. The total number of errors divided by the total number of data points gives the topographic error of the map.
