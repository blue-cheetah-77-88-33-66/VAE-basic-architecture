# VAE-basic-architecture
<h2>Basic architecture of Variational Auto-Encoders</h2>


<img src="https://github.com/mustafasbahar59/VAE-basic-architecture/assets/117897880/2d69ca58-a3e8-41d0-9b4d-05b63c1c1d72" width="800">

The simple architecture of VAE is shown above.

VAE stands for "Variational Autoencoder." It is a type of generative model that combines elements of both autoencoders and probabilistic modeling. VAEs are used for unsupervised learning and have been particularly effective in generating new data samples, such as images, while also learning meaningful latent representations.

An autoencoder is a type of neural network architecture that is trained to reconstruct its input data at the output layer. It consists of an encoder network that compresses the input data into a lower-dimensional representation (latent space) and a decoder network that reconstructs the original input from the latent representation. Autoencoders are primarily used for data compression, denoising, and dimensionality reduction.

VAEs extend the concept of autoencoders by incorporating probabilistic modeling into the latent space. In a VAE, the encoder network maps the input data to a probability distribution in the latent space instead of directly producing a deterministic representation. This probability distribution is usually assumed to be a multivariate Gaussian. The decoder network then samples from this distribution to generate a reconstructed output.

The training of a VAE involves maximizing the evidence lower bound (ELBO), which is a lower-bound approximation of the log-likelihood of the data. The ELBO is decomposed into two components: the reconstruction loss, which encourages the decoder to generate outputs similar to the original inputs, and the KL divergence, which encourages the learned latent distribution to match a predefined prior distribution (usually a standard Gaussian).

By learning a latent space with a predefined prior distribution, VAEs enable the generation of new data samples by sampling from the latent space. This allows for the exploration and interpolation of the data distribution. Additionally, the continuous and structured nature of the latent space in VAEs makes it possible to perform operations such as image editing, interpolation between images, and style transfer.

VAEs have been widely used in various domains, including image generation, text generation, and speech synthesis. They have proven to be effective in learning meaningful representations and generating novel data samples with applications in areas like image synthesis, anomaly detection, and data augmentation<.

<h2>Reference:</h2>
Kingma, D. P., & Welling, M. (2013). Auto-encoding variational bayes. arXiv preprint arXiv:1312.6114.
