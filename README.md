# GPT-like basic Large Language Model implementation in PyTorch

This is a basic implementation of a GPT like Large Language Model. It is the rewritten version of an "free code camp" example, with cleaned up code, added visualisation and improved routines. 

The goal of this notebook is not necessarily to get perfect results but to understand how the architecture works or to simply implement improvements.

I improved a couple of things to help understanding the structure, like:
- variable names are better to read (no abbrevations) and more consistent
- fix the loss calculation which was to complex
- improved optimisation loop (train, loss calculation, testing, loss calculation)
- added visualisation plot to see how training improves

## Todo

Though, there is still room for improvement, like 
- encapsulating layer results in the all the forward functions (memory-wise this will gain some performance)
- actually implementing batch-wise training, right now the batch size does not really matters, as we train on one batch each epoch

# COLAB
You can find the notebook in Google's Colab: 

https://drive.google.com/file/d/1qnXidqmzZUYt-1MDyZJEHABKQaatMY-7/view?usp=sharing

If you want to run the notebook for your self, you need to provide your own data. To do this just change those values:

    source_data_path = "drive/MyDrive/Colab Notebooks/data"
    source_data = "text.txt"

# Additional Resources

As a good starting point to understand how deep learning works with PyTorch, I suggest this 1-day course by Daniel Bourke: 

- https://www.youtube.com/watch?v=Z_ikDlimN6A

To understand how the mathematics behind Large Language Models work, there is one great resource:

- https://flyte.org/blog/getting-started-with-large-language-models-key-things-to-know

The following resources describes how transformers work

- https://e2eml.school/transformers.html
- http://jalammar.github.io/illustrated-transformer/
- https://ig.ft.com/generative-ai/
