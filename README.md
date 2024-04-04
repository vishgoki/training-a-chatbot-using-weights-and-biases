# training-a-chatbot-using-weights-and-biases
This GitHub project trains a chatbot using the Cornell Movie-Dialogs Corpus with PyTorch. It covers dataset pre-processing, implementing a seq2seq model with Luong attention, training with mini-batches, greedy-search decoding, and chatbot interaction. A hands-on for understanding and applying NLP and weights and biases.

# Chatbot Training with Cornell Movie Dialogs Corpus

This repository guides you through training a chatbot using the Cornell Movie Dialogs Corpus in a PyTorch environment, based on a detailed PyTorch Chatbot Tutorial. The project focuses on a sequence-to-sequence model with Luong attention mechanisms, leveraging the PyTorch framework for an end-to-end chatbot training experience.

## Objective
- To understand and implement the sequence-to-sequence model architecture using PyTorch.
- To learn the process of data pre-processing, training, and interacting with a chatbot model.

## Steps to Completion

1. **Training the Model**
   - Make a copy of the tutorial notebook and execute the training and evaluation steps in your local Google Colab environment.

2. **Hyperparameter Optimization**
   - Integrate Weights and Biases (W&B) for hyperparameter optimization.
   - Set up a hyperparameter sweep with W&B using Random Search strategy for learning rate, optimizer, clip, teacher forcing ratio, and decoder learning ratio.

3. **Evaluation and Profiling**
   - Run hyperparameter sweeps and monitor the outcomes in the W&B dashboard.
   - Identify optimal hyperparameters based on minimum model loss and analyze their impact on model convergence using W&B's feature importance tool.
   - Utilize the PyTorch Profiler to measure time and memory consumption of the model's operations.

4. **Model Conversion to TorchScript**
   - Understand the differences between tracing and scripting as TorchScript conversion methods.
   - Convert the trained model to TorchScript and evaluate its performance.
   - Compare the latency of the TorchScript model against the original PyTorch model on both CPU and GPU.

5. **Deployment**
   - Serialize the best-performing model for deployment in non-Python environments.
   - (Bonus) Demonstrate the use of the TorchScript model in a C++ application.

## References
- [Cornell Movie Dialogs Corpus](https://www.cs.cornell.edu/~cristian/Cornell_Movie-Dialogs_Corpus.html)
- [Weights and Biases Framework Video Tutorial](https://www.youtube.com/watch?v=9zrmUIlScdY)
- [Weights and Biases Framework Colab project](https://colab.research.google.com/github/wandb/examples/blob/master/colabs/pytorch/Organizing_Hyperparameter_Sweeps_in_PyTorch_with_W%26B.ipynb)
- [PyTorch Profiler Example](https://pytorch.org/tutorials/recipes/recipes/profiler_recipe.html)
- [PyTorch TorchScript tutorial](https://pytorch.org/tutorials/beginner/deploy_seq2seq_hybrid_frontend_tutorial.html)

## Contributions
We welcome contributions and suggestions on how to improve this project. Feel free to fork the repository, make changes, and submit pull requests.

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
