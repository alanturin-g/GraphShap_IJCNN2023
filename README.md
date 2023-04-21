# GraphShap
Explaining Identity-aware Graph Classifiers through the Language of Motifs

Most methods for explaining black-box classifiers  (e.g., on tabular data, images, or time series) rely on measuring the impact that removing/perturbing features has on the model output. This forces the explanation language to match the classifier's feature space. 

However, when dealing with graph data, in which the basic features correspond to the edges describing the graph structure, this matching between features space and explanation language might not be appropriate. Decoupling the feature space (edges) from a desired high-lever explanation language (such as motifs) is thus a major challenge towards developing actionable explanations for graph classification tasks.

In this paper we introduce GraphShap, a Shapley-based approach able to provide motif-based explanations for  identity-aware graph classifiers, assuming no knowledge whatsoever about the model or its training data: the only requirement is that the classifier can be queried as a black-box at will. For the sake of computational efficiency we explore a progressive approximation strategy and show how a simple kernel can efficiently approximate explanation scores, thus allowing GraphShap to scale on scenarios with a large explanation space (i.e., large number of motifs).

We showcase GraphShap on a real-world brain-network dataset consisting of patients affected by Autism Spectrum Disorder and a control group. Our experiments highlight how the classification provided by a black-box model can be effectively explained by few connectomics patterns.

The code in this repository allows to re-obtain all results and plots from the paper.
Some logged files in /data have been compressed to comply with GitHub limits.
