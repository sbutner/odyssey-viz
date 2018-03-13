# Visualizing Narrative Arcs

Embedding discrete values, such as words, into high-dimensional continuous space has accelerated in popularity in recent years. Word embeddings proved effective for use in several semantic tasks, and helped spur the *2vec* craze. Skip-thought vectors, an attempt at *sentence2vec*, made use of a clever objective function: how well can the context (the sentence before and the sentence after) be reconstructed from the embedded sentence? 

# Process

Using the [pre-trained encoder](https://github.com/ryankiros/skip-thoughts), I converted each sentence in *The Odyssey* to a 4800-dimensional vector. Then, using [t-SNE](https://lvdmaaten.github.io/publications/papers/JMLR_2008.pdf) I reduced those embeddings to 5-dimensional vectors which I graphed as (X, Y, \[R,G,B\]) values. Finally, I appended each sentence's index as an additional coordinate to be able to visualize in narrative order. Used [rthreejs](http://bwlewis.github.io/rthreejs) to produce the interactive 3-D scatterplot.
