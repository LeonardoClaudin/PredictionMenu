# Post-Translation Modification Prediction Tool: Phosphorilation
Implementation of several DeepLearning tools that predict General or Kinase-Specific phosphorilation sites based solely on the protein and, sometimes, on the Kinase residue sequence (FASTA).
Prediction tool | Method
--------------- | -------------------------
MusiteDeep      | DNN
DeepPhos        | DNN
GPS 5.0         | Group-based scoring PSSM
AKID            | DNN
NetPhorest      | ANN and PSSM

## REQUIREMENTS.
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
No specific requirements. Only works in Linux.
Installation for local use is required (recommended in home directory).

### AKID
No specific requirements. Only works in Linux.

### NetPhorest
No specific requirements. Only works in Linux.

## HOW TO
1. Unzip the PTM_phosphorilation.zip
2. Make the main.sh an exxecutable bash script.
    - Inside terminal, type: chmod u+x main.sh at the correct working directory
    - run the program like: ./main.sh
3. Select which tool to implement for the prediction and follow the instructions.

### MusiteDeep
Store input FASTA file with the protein sequences inside *MusiteDeep* folder.

###DeePhos
Currently not working. Working on an update.

### GPS 5.0
Accepts FASTA files of any given residue length. File can be loaded from any directory.

### AKID
Requires FASTA files for the Kinase (in order to create kinase determinants) and FASTA files for the protein sequences (input).
Both should be stored inside *AKID/input* folder.

### NetPhorest
Only requires FASTA file of any given residue length. File should be stored inside *NetPhorest* folder.
