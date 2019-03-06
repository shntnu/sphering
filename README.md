# Experiments with whitening 

The regularization parameter $\epsilon$ (here, varied from $1$ to $10^{-9}$) determines the shape of the curve below, 
which shows the eigenvalues of the whitened covariance matrix: 

$\hat{\sigma_{i}} = \sigma_{i}/(\sigma_{i} + \epsilon)$, 
where $\hat{\sigma_{i}}$ is the $i^{th}$ eigenvalue of the whitened covariance matrix, $\sigma_{i}$ is the $i^{th}$ eigenvalue of the original covariance matrix. 

Setting $\epsilon = \sigma_{j}/10$ gives $\hat{\sigma_{j}} \approx 0.9$, i.e., the curve will drop to $0.9$ by the $j^{th}$ eigenvector. 

A possible heuristic then would be to select $j$ to be the estimated "true" dimensionality of the data.

![Global whitening](global_whitening.gif "Variance of whitened data.")

