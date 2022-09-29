# Post-Translation Modification Prediction Tool: Phosphorilation
Implementation of several DeepLearning tools that predict General or Kinase-Specific phosphorilation sites based solely on the protein and, sometimes, on the Kinase residue sequence (FASTA).
Prediction tool | Method
--------------- | -------------------------
MusiteDeep      | DNN
DeepPhos        | DNN
GPS 5.0         | Group-based scoring PSSM
AKID            | DNN
NetPhorest      | ANN and PSSM

## Requirements.
### MusiteDeep
1. Conda environment with Python 2.0 (named python2)
    1. keras == 1.1.0
    2. numpy >= 1.8.0
    3. theano>=0.8.0
2. Keras with theano backend
    - Inside keras.json change backend from tensorflow to theano

### DeepPhos
1. Packages versions:
    1. keras == 2.0.0
    2. numpy >= 1.8.0
3. Keras with tensorflow backend
   - Inside keras.json change backend from theano to tensorflow

### GPS 5.0
1. No specific requirements. Only works in Linux.

### AKID
1. No specific requirements. Only works in Linux.

### NetPhorest
1. No specific requirements. Only works in Linux.
