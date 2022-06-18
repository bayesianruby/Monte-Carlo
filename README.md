# Monte-Carlo

The goal of this project is to calculate numerically the expectation $E(f(G))$ where $f$ is a test function and $G$ is a Gaussian vector of dimension 5 with independent components, each component of which is centred with unit variance. 

Our algorithm will is able to work for any reasonable (bounded or sufficiently integrable) function f, so we designed a generic algorithm but one that is clever enough to do better than a basic algorithm.

Hence we use a Halton method to generate uniforms laws in 6 dimension, and we used Box Muller transformation to get gaussians. Then we made an estimator to get the expectation.

Here are the comparison between the error of basic Monte-Carlo and our algorithm:

![téléchargement](https://user-images.githubusercontent.com/80846462/174439115-7499b7dc-07d3-464c-bb43-03e32c5b6305.png)
![halton](https://user-images.githubusercontent.com/80846462/174439117-ac0a16e3-d663-4894-a8b8-a521ae246f6c.png)
