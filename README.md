# GPT-like basic Large Language Model implementation in PyTorch

This is a basic implementation of a GPT like Large Language Model. It is the rewritten version of an "free code camp" example, with cleaned up code, added visualisation and improved routines. 

The goal of this notebook is not necessarily to get perfect results but to understand how the architecture works or to simply implement improvements.

I improved a couple of things to help understanding the structure, like:
- variable names are better to read (no abbrevations) and more consistent
- fix the loss calculation which was to complex
- improved optimisation loop (train, loss calculation, testing, loss calculation)
- added visualisation plot to see how training improves

Though, there is still room for improvement, like encapsulating layer results in the all the forward functions (memory-wise this will gain some performance). 
