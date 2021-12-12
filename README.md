# DLRL Coursework

## Deep Learning

For the Deep Learning sub-module, we were tasked to build a generative model, using of the CIFAR10 (32x32) & STL10 (96x96) image datasets to develop pictures of a pegasus.

### Abstract from my report:

This paper proposes using a GLO model to generate images that look like a Pegasus. This model uses a basic generator architecture along with the Laplacian loss function, an informative loss equation which helps at a range of image resolutions. Then, we map each image to a point on the n-dimensional spherical latent space, acting as our probability distribution. Using this spherical distribution, we examine the latent space between horses and birds with the intention of generating a smooth interpolation of the two images.

To view the full paper please visit: https://julianwyatt.co.uk/DLRL

### Comments:
I quickly learned however that this model was not able to produce high quality samples as the space between image latents was not meaningful. 
For example see below the high quality reconstructions vs low quality interpolations:

| Image | Info |
| ------------- | ------------- |
| <img src="./reconBatch.png" alttext="Best Image Reconstruction" width="450px">  | Best Image Reconstruction  |
| <img src="./best-batch.png" alttext="Best Image Interpolation" width="450px">  | Best Image Interpolation  |


## Reinforcement Learning

For the module, we were tasked to develop an RL agent to play Atari Gravitar. The aim of Gravitar is complex, even for humans. The player must meander around gravity, visiting planets, collecting fuel, all while shooting other space ships. This makes the game notoriously difficult for agents to learn due to the sparse, long term reward structure. Therefore, I looked towards sequential models such as LSTMs from recent papers such as R2D2.
Please see https://www.youtube.com/embed/oTNwsHRPOeM for my most intuitive gameplay sequence.
