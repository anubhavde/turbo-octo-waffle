# turbo-octo-waffle

## **Detecting Higgs Boson Particle**
### Searching for the Higgs Boson
The Standard Model is a particle physics hypothesis that explains some of the most fundamental forces in the universe. The mass of matter is explained by one elementary particle, the **Higgs boson**. The Higgs boson was first theorised in 1964, but it took over 50 years for it to be observed, i.e it was discovered in the the Large Hadron Collider in 2012. 

The data from these experiments totaled millions of megabytes. So, using Deep Learning to determine whether an observed particle collision produced a Higgs boson or not, I have constructed a Wide and Deep neural network.

### The Collision Data
The collision of protons at high energy can produce new particles like the Higgs boson. These particles can't be directly observed because they decay almost instantly. So to detect the presence of a new particle, we instead observe the behavior of the particles they decay into, their "decay products".

The Higgs dataset contains 21 "low-level" features of the decay products and also 7 more "high-level" features derived from these.

## Wide and Deep Neural Networks
A Wide and Deep network trains a linear layer side-by-side with a deep stack of dense layers therefore proving to be effective on tabular datasets.

Both the dataset and the model are very large therefore taking extremely huge amounts of time and resources, even for a GPU (I tried to train my models using a NVIDIA GTX 1060 Ti with Max Q Design which resulted in my system overheating for prolonged hours at just the first epoch). So, to speed up training, I have used Kaggle's Tensor Processing Units (TPUs), an accelerator ideal for large workloads.

##### Please note in this repository only the validation part of the dataset has been uploaded. The entire dataset can be downloaded from https://www.kaggle.com/datasets/ryanholbrook/higgs-boson.
