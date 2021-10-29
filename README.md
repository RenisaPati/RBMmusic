# RBMmusic

The Restricted Boltzmann Machine:
RBM is the neural network that belongs to the energy-based model
· It is a probabilistic, unsupervised, generative deep machine learning algorithm.
· RBM’s objective is to find the joint probability distribution that maximizes the log-likelihood function.
· RBM is undirected and has only two layers, Input layer, and hidden layer
· All visible nodes are connected to all the hidden nodes. RBM has two layers, visible layer or input layer and hidden layer so it is also called an asymmetrical bipartite graph.
· No intralayer connection exists between the visible nodes. There is also no intralayer connection between the hidden nodes. There are connections only between input and hidden nodes.
· The original Boltzmann machine had connections between all the nodes. Since RBM restricts the intralayer connection, it is called a Restricted Boltzmann Machine.
What makes RBMs different from Boltzmann machines is that visible node isn’t connected to each other, and hidden nodes aren’t connected with each other.

Here, in this project, I have used the inherent pattern detection and generative capabilities of the RBM to generate music.

Data:
The same data consists of audio files of MIDI (Musical Instrument Digital Interface) format.
I have used 100 audio files of "pop" genre.

Technicalities:
I used Tensorflow libraries for the implementation.
- The hidden and visible nides of the network layers are first initialised.
- The input parameters are then updated based on the difference between the samples and original values.
- Training the model by using each music file (.midi) as input and generating the midi files as output.
- After training, a Gibbs chain in run where visible nodes are initialised to 0.
- Extracted vector is reshaped into n number of nodes and then saved as output .midi file.


