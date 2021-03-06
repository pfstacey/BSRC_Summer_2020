# Megastructure Observability within TESS Light Curves
### Piper Stacey
#### Howard Isaacson, Steve Croft
##### Ann Marie Cody, Doug Caldwell, Brian Powell, Marvin Morgan

##### ~ Breakthrough Listen's Berkeley SETI Research Center ~

Contents of this repository:
Supplimentary artificial objects folders under the names: 
artifacts, blogpost_word, names, circularity, subtract_artifacts, Extra Shapes

Results of artificial object light curves folders under the names:
result_blogpost_word, result_noisy_artifacts, results_names, results_subtract_artifacts

Folder EightBitTransit contains a README.md to let user know how to download EightBitTransit code from GitHub.

### Code Breakdown:
#### NOTE: ALL CODE CAN ONLY BE RUN IN PYTHON 2
##### name_transit.ipynb:
This code allows a user to model any name (or any object) provided the user has a png black and white image of the object they would like to model

##### Injecting_TESS_Noise.ipynb:
This code allows a user to add noise to the transit model generated by EightBitTransit. The user can choose whether they want to implement Gaussian (recommended because of the Poisson distribution of photon collection) or non-Gaussian noise to their light curves. This script also has a preliminary way to ensure images are black and white and can be modified to change image size and shape. 

##### Simple Noise addition (non-gaussian).ipynb:
This code only allows the use to generate non-Gaussian noise. This is not recommended. 

##### LC_to_Megastruct.ipynb:
This code is preliminary and allows for choppy modeling of possible megastructures that could be generating features of existing light curves. Because of structure degeneracies, see Sandford and Kipping 2018 for more, these models are not very precise and are better to run on a stronger processor than your local computer.

##### Circularity Difference for One Object.ipynb:
This code allows a user to measure the circularity difference between any artificial object and a planet. It also allows them to model the respective transits of their artificial object and a planet of exactly the same size (ensuring the same transit depth for both light curves). This script also allows the user to calculate the observability of their artificial object as something different than a planet (is the object observable as something different than a planet?). This script can only calculate observability at a single magnitude. 

##### Circularity and Observability at any Mag.ipynb:
This code allows a user to measure the non-circularity and observability indexes of a set of articial objects across magnitudes. It can then plot the non-circularity threshold to be observable (above an observability index of 3) at each magnitude to demonstrate a trend between increased stellar noise and lack of observability. 

#### Note again: all code must be run in Python 2

#### For more information, read Creating_a_VM_in_BLs_Sandbox.pdf and BSRC_Final_WriteUp.pdf

##### Contact piper.f.stacey.23@dartmouth.edu with questions. 
###### Hope the world found a vaccine! Best, Piper
