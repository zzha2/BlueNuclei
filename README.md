# BlueNuclei
Fully automated cell death classifier for transfected neurons
This is a beta version. This program is still under active testing and improvement. Currently it takes czi files (from Zeiss microscopes) only, and is only suitable for neurons. Extension to other file type and cell types will be a future work.
What the program does: 1. extract GFP channel (GFP transfected neurons) and DAPI channel (nuclei). Pre-process the images with some thresholding techniques. 2. For each neuron in the GFP channel, identify its corresponding nucleus in the DAPI channel. 3. Use a pre-trained support vector machine (SVM) to determine whether the nucleus (i.e. the neuron) is live or dead. 4. Output summary: live/dead neuron count in this image. Then move on to the next image. 
Source code for training the SVM is also available.
