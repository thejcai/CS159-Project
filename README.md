# CS 159 Project
Normalizing Flows for Recurrent Neural Networks: Flow-RNN


## Running the model on Google Cloud 

From the deployment manager, once the VM has been deployed open the Jupyter notebook instance. Upload the files in the sketch_rnn sub-repo. Create a log directory for checkpoints. 

Verify the hyperparameters in the sketch_rnn_train.ipynb file are what you want. In between runs, you have to restart the kernel. 

You will also want to check the tf.app.flags.DEFINE_string fields at the top of the notebook - make sure these properly specify where you want the log files saved, and whether you are resuming training. 

We will use the following hyperparameters:

  num_steps = 25000
  dec_model = "layer_norm"
  enc_model = "layer_norm"
  kl_weight = 0.25
  num_flows = depends on the particular experiment being run
  
  
