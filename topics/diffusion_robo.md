# Diffusion-Literature-for-Robotics
Summary of the most important papers and blogs about diffusion models for people to learn about diffusion models. Further, it contains an overview of published robotics diffusion papers.

# Table of Contents
1. [Learning about Diffusion models](#Learning-about-Diffusion-models)
2. [Diffusion in Robotics](#Diffusion-in-Robotics)

    2.1 [Imitation Learning and Policy Learning](#Imitation-Learning-and-Policy-Learning)

    2.2 [Online RL](#Online-RL)
    
    2.3 [Offline RL](#Offline-RL)

    2.4 [Inverse RL](#Inverse-RL)

    2.5 [Task and Motion Planning](#tamp)

    2.5 [Tactile Sensing & Pose Estimation](#Grasping-&-Tactile-Sensing-&-Pose-Estimation)

3. [Code Implementations](#Code-Bases)

4. [Diffusion History](#Diffusion-History)

---

## Learning about Diffusion models 
<a name="Learning-about-Diffusion-models"></a>
While there exist many tutorials for Diffusion models, below you can find an overview of some of the best introduction blog posts and video:

- [What are Diffusion Models?](https://www.youtube.com/watch?v=fbLgFrlTnGU&t=1s): an introduction video, which introduces the general idea of diffusion models and some high-level math about how the model works

- [Diffusion Models | Paper Explanation | Math Explained](https://www.youtube.com/watch?v=HoKDTa5jHvg) another great video tutorial explaining the math and notation of diffusion models in detail with visual aid

- [Generative Modeling by Estimating Gradients of the Data Distribution](https://yang-song.net/blog/2021/score/): blog post from the one of the most influential authors in this area, which introduces diffusion models from the score-based perspective 
- [What are Diffusion Models](https://lilianweng.github.io/posts/2021-07-11-diffusion-models/): a in-depth blog post about the theory of diffusion models with a general  summary on how diffusion model improved over time 
- [Understanding Diffusion Models](https://arxiv.org/pdf/2208.11970.pdf): an in-depth explanation paper, which explains the diffusion models from both perspectives with detailed derivations

If you don't like reading blog posts and prefer the original papers, below you can find a list with the most important diffusion theory papers:

- Sohl-Dickstein, Jascha, et al. ["Deep unsupervised learning using nonequilibrium thermodynamics."](http://proceedings.mlr.press/v37/sohl-dickstein15.pdf) _International Conference on Machine Learning_. PMLR, 2015.

- Ho, Jonathan, et al. ["Denoising diffusion probabilistic models."](https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf) _Advances in Neural Information Processing Systems_ 33 (2020): 6840-6851.
- Song, Yang, et al. ["Score-Based Generative Modeling through Stochastic Differential Equations."](https://arxiv.org/pdf/2011.13456) _International Conference on Learning Representations_. 2020.

- Ho, Jonathan, and Tim Salimans. ["Classifier-Free Diffusion Guidance."](https://arxiv.org/pdf/2207.12598) _NeurIPS 2021 Workshop on Deep Generative Models and Downstream Applications_. 2021.

- Karras, Tero, et al. ["Elucidating the Design Space of Diffusion-Based Generative Models."](https://arxiv.org/pdf/2206.00364) _Advances in Neural Information Processing Systems_ 35 (2022)

A general list with all published diffusion papers can be found here: [Whats the score?](https://scorebasedgenerativemodeling.github.io/)

---

## Diffusion in Robotics
<a name="Diffusion-in-Robotics"></a>
Since the modern diffusion models have been around for only 3 years, the literature about diffusion models in the context of robotics is still small, but growing rapidly. Below you can find most robotics diffusion papers, which have been published at conferences or uploaded to Arxiv so far:

---

### Imitation Learning and Policy Learning
<a name="Imitation-Learning-and-Policy-Learning"></a>

- Ha, Huy, Pete Florence, and Shuran Song. ["Scaling Up and Distilling Down: Language-Guided Robot Skill Acquisition."](https://arxiv.org/pdf/2307.14535) arXiv preprint arXiv:2307.14535 (2023).

- Xu, Mengda, et al. ["XSkill: Cross Embodiment Skill Discovery."](https://arxiv.org/pdf/2307.09955) arXiv preprint arXiv:2307.09955 (2023).

- Li, Xiang, et al. ["Crossway Diffusion: Improving Diffusion-based Visuomotor Policy via Self-supervised Learning."](https://arxiv.org/pdf/2307.01849) arXiv preprint arXiv:2307.01849 (2023).

- Ng, Eley, Ziang Liu, and Monroe Kennedy III. ["Diffusion Co-Policy for Synergistic Human-Robot Collaborative Tasks."](https://arxiv.org/pdf/2305.12171) arXiv preprint arXiv:2305.12171 (2023).

- Chi, Cheng, et al. ["Diffusion Policy: Visuomotor Policy Learning via Action Diffusion."](https://arxiv.org/pdf/2303.04137) _Proceedings of Robotics: Science and Systems (RSS)_ 2023.

- Reuss, Moritz, et al. ["Goal-Conditioned Imitation Learning using Score-based Diffusion Policies."](https://arxiv.org/pdf/2304.02532) _Proceedings of Robotics: Science and Systems (RSS)_ 2023.

- Yoneda, Takuma, et al. ["To the Noise and Back: Diffusion for Shared Autonomy."](https://arxiv.org/pdf/2302.12244) _Proceedings of Robotics: Science and Systems (RSS)_ 2023.

- Dai, Yilun, et al. ["Learning Universal Policies via Text-Guided Video Generation."](https://arxiv.org/pdf/2302.00111) arXiv preprint arXiv:2302.00111 (2023).

- Jiang, Chiyu, et al. ["MotionDiffuser: Controllable Multi-Agent Motion Prediction Using Diffusion."](https://openaccess.thecvf.com/content/CVPR2023/papers/Jiang_MotionDiffuser_Controllable_Multi-Agent_Motion_Prediction_Using_Diffusion_CVPR_2023_paper.pdf) Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2023.

- Kapelyukh, Ivan, et al. ["DALL-E-Bot: Introducing Web-Scale Diffusion Models to Robotics."](https://openreview.net/forum?id=HzOy6lUzPj1) _IEEE Robotics and Automation Letters (RA-L)_ 2023.

- Pearce, Tim, et al. ["Imitating human behaviour with diffusion models."](https://openreview.net/pdf?id=Pv1GPQzRrC8) 
" _International Conference on Learning Representations_. 2023.

- Yu, Tianhe, et al. ["Scaling robot learning with semantically imagined experience."](https://arxiv.org/pdf/2302.11550.pdf) arXiv preprint arXiv:2302.11550 (2023).


---

### Online RL 
<a name="Online-RL"></a>

The number of papers  The standard policy gradient objective requires the gradient of the log-likelihood, which is only implicitly defined by the underlying Ordinary Differential Equation (ODE) of the diffusion model. 

- Yang, Long, et al. ["Policy Representation via Diffusion Probability Model for Reinforcement Learning."](https://arxiv.org/pdf/2305.13122) arXiv preprint arXiv:2305.13122 (2023).

- Mazoure, Bogdan, et al. ["Value function estimation using conditional diffusion models for control."](https://arxiv.org/pdf/2306.07290) arXiv preprint arXiv:2306.07290 (2023).

--- 

### Offline RL
<a name="Offline-RL"></a>

- Yuan, Hui, et al. ["Reward-Directed Conditional Diffusion: Provable Distribution Estimation and Reward Improvement."](https://arxiv.org/pdf/2307.07055) arXiv preprint arXiv:2307.07055 (2023).

- Hu, Jifeng, et al. ["Instructed Diffuser with Temporal Condition Guidance for Offline Reinforcement Learning."](https://arxiv.org/pdf/2306.04875) arXiv preprint arXiv:2306.04875 (2023).

- Hegde, Shashank, et al. ["Generating Behaviorally Diverse Policies with Latent Diffusion Models."](https://arxiv.org/pdf/2305.18738) arXiv preprint arXiv:2305.18738 (2023).

- Xiao, Wei, et al. ["SafeDiffuser: Safe Planning with Diffusion Probabilistic Models."](https://arxiv.org/pdf/2306.00148) arXiv preprint arXiv:2306.00148 (2023).

- Li, Wenhao, et al. ["Hierarchical Diffusion for Offline Decision Making."](https://openreview.net/pdf?id=55kLa7tH9o) _International Conference on Machine Learning_. PMLR, 2023.

- Liang, Zhixuan, et al. ["AdaptDiffuser: Diffusion Models as Adaptive Self-evolving Planners."](https://arxiv.org/pdf/2302.01877) _International Conference on Machine Learning_. PMLR, 2023.

- Lu, Cheng, et al. ["Contrastive Energy Prediction for Exact Energy-Guided Diffusion Sampling in Offline Reinforcement Learning."](https://arxiv.org/pdf/2304.12824.pdf)  _International Conference on Machine Learning_. PMLR, 2023.

- Zhu, Zhengbang, et al. ["MADiff: Offline Multi-agent Learning with Diffusion Models."](https://arxiv.org/pdf/2305.17330) arXiv preprint arXiv:2305.17330 (2023).

- Kang, Bingyi, et al. ["Efficient Diffusion Policies for Offline Reinforcement Learning."](https://arxiv.org/pdf/2305.20081) arXiv preprint arXiv:2305.20081 (2023).

- Ni, Fei, et al. ["MetaDiffuser: Diffusion Model as Conditional Planner for Offline Meta-RL."](https://arxiv.org/pdf/2305.19923) _International Conference on Machine Learning_. PMLR, 2023.


- He, Haoran, et al. ["Diffusion Model is an Effective Planner and Data Synthesizer for Multi-Task Reinforcement Learning."](https://arxiv.org/pdf/2305.18459) arXiv preprint arXiv:2305.18459 (2023).

- Ajay, Anurag, et al. ["Is Conditional Generative Modeling all you need for Decision-Making?."](https://arxiv.org/pdf/2211.15657) _International Conference on Learning Representations_. 2023.

- Hansen-Estruch, Philippe, et al. ["IDQL: Implicit Q-Learning as an Actor-Critic Method with Diffusion Policies."](https://arxiv.org/pdf/2304.10573) arXiv preprint arXiv:2304.10573 (2023).

- Zhu, Zhengbang, et al. ["MADiff: Offline Multi-agent Learning with Diffusion Models."](https://arxiv.org/pdf/2305.17330) arXiv preprint arXiv:2305.17330 (2023).

- Zhang, Edwin, et al. ["LAD: Language Augmented Diffusion for Reinforcement Learning."](https://arxiv.org/pdf/2210.15629) arXiv preprint arXiv:2210.15629 (2022).

- Brehmer, Johann, et al. [EDGI: Equivariant Diffusion for Planning with Embodied Agents](https://openreview.net/forum?id=OrbWCpidbt) _Workshop on Reincarnating Reinforcement Learning at ICLR_ 2023. 

- Janner, Michael, et al. ["Planning with Diffusion for Flexible Behavior Synthesis."](https://arxiv.org/pdf/2205.09991.pdf) _International Conference on Learning Representations_. 2022.

- Wang, Zhendong, et al. ["Diffusion policies as an expressive policy class for offline reinforcement learning."](https://arxiv.org/pdf/2208.06193.pdf)  _International Conference on Learning Representations_. 2023.

- Brehmer, Johann, et al. ["EDGI: Equivariant Diffusion for Planning with Embodied Agents."](https://arxiv.org/pdf/2303.12410) arXiv preprint arXiv:2303.12410 (2023).

- Chen, Huayu, et al. ["Offline Reinforcement Learning via High-Fidelity Generative Behavior Modeling."](https://openreview.net/pdf?id=42zs3qa2kpy)" _International Conference on Learning Representations_. 2023.


--- 

### Inverse RL
<a name="Inverse-RL"></a>

- Nuti, Felipe, Tim Franzmeyer, and João F. Henriques. ["Extracting Reward Functions from Diffusion Models."](https://arxiv.org/pdf/2306.01804) arXiv preprint arXiv:2306.01804 (2023).

---

### Task and Motion Planning
<a name="tamp"></a>

- Fang, Xiaolin, et al. ["DiMSam: Diffusion Models as Samplers for Task and Motion Planning under Partial Observability."](https://arxiv.org/pdf/2306.13196) arXiv preprint arXiv:2306.13196 (2023).

- Liu, Weiyu, et al. ["StructDiffusion: Object-centric diffusion for semantic rearrangement of novel objects."](https://arxiv.org/pdf/2211.04604) _Proceedings of Robotics: Science and Systems (RSS)_ 2023.

- Mishra, Utkarsh A., and Yongxin Chen. ["ReorientDiff: Diffusion Model based Reorientation for Object Manipulation."](https://arxiv.org/pdf/2303.12700) _RSS 2023 Workshop on Learning for Task and Motion Planning_

- Urain, Julen, et al. ["SE (3)-DiffusionFields: Learning cost functions for joint grasp and motion optimization through diffusion."](https://arxiv.org/pdf/2209.03855) _IEEE International Conference on Robotics and Automation (ICRA)_ 2023

- Carvalho, J. et al. [Conditioned Score-Based Models for Learning Collision-Free Trajectory Generation](https://www.ias.informatik.tu-darmstadt.de/uploads/Team/JoaoCarvalho/Conditioned_Score_Based_Models_for_Learning_Collision_Free_Trajectory_Generation.pdf), _NeurIPS 2022 Workshop on Score-Based Methods_ 

---

### Tactile Sensing & Pose Estimation

<a name="Grasping-&-Tactile-Sensing-&-Pose-Estimation"></a>

- Simeonov, Anthony, et al. ["Shelving, Stacking, Hanging: Relational Pose Diffusion for Multi-modal Rearrangement."](https://arxiv.org/pdf/2307.04751) arXiv preprint arXiv:2307.04751 (2023).

- Higuera, Carolina, Byron Boots, and Mustafa Mukadam. ["Learning to Read Braille: Bridging the Tactile Reality Gap with Diffusion Models."](https://arxiv.org/pdf/2304.01182) arXiv preprint arXiv:2304.01182 (2023).


---

## Code Implementations
<a name="Code-Bases"></a>

There exist numerous implementations of all diffusion models on github. Below you can find a curated list of some clean code variants of the most important diffusion models in general and for robotics:

- [Diffusers](https://github.com/huggingface/diffusers): the main diffusion project from HuggingFaces with numerous pre-trained diffusion models ready to use 

- [k-diffusion](https://github.com/crowsonkb/k-diffusion): while its not the official code-base of the EDM diffusion models from [Karras et al., 2022](https://arxiv.org/pdf/2206.00364), it has very clean code and numerous samplers. Parts of the code have been used in various other projects such as [Consistency Models](https://github.com/openai/consistency_models) from OpenAI and diffusers from HuggingFaces.

- [denoising-diffusion-pytorch](https://github.com/lucidrains/denoising-diffusion-pytorch): a clean DDPM diffusion model implementation in Pytorch to get a good understanding of all the components 

- [Diffuser](https://github.com/jannerm/diffuser): Variants of this code are used in numerous trajectory diffusion OfflineRL papers listed above

- [diffusion_policy](https://github.com/columbia-ai-robotics/diffusion_policy): Beautiful Code implementation of Diffusion policies from [Chi et al., 2023](https://diffusion-policy.cs.columbia.edu/#paper) for Imitation Learning with 9 different simulations to test the models on

- [dpm-solver](https://github.com/LuChengTHU/dpm-solver): One of the most widely used ODE samplers for Diffusion models from [Lu et al. 2022](https://arxiv.org/abs/2206.00927) with implementations for all different diffusion models including wrappers for discrete DDPM variants 


--- 

## Diffusion History
<a name="Diffusion-History"></a>
Diffusion models are a type of generative model inspired by non-equilibrium thermodynamics, introduced by [Sohl-Dickstein et al., (2015)](https://arxiv.org/abs/1503.03585). The model learns to invert a diffusion process, that gradually adds noise to a data sample. This process is a Markov chain consisting of diffusion steps, which add random Gaussian noise to a data sample. The diffusion model is used to learn to invert this process. While the paper was presented  in 2015, it took several years for the diffusion models to get widespread attention in the research community. Diffusion models are a type of generative model and in this field, the main focus are vision based applications, thus all theory papers mentioned in the text below are mostly focused on image synthesis or similar tasks related to it. 

There are two perspectives to view diffusion models. The first one is based on the initial idea of  [Sohl-Dickstein et al., (2015)](https://arxiv.org/abs/1503.03585), while the other is based on a different direction of research known as score-based generative models. In 2019 [Song & Ermon, (2019)](https://proceedings.neurips.cc/paper/2019/file/3001ef257407d5a371a96dcd947c7d93-Paper.pdf) proposed the _noise-conditioned score network (NCSN)_, which is a predecessor to the score-based diffusion model. The main idea was to learn the score function of the unknown data distribution using a neural network. This approach had been around before, however their paper and the subsequent work [Song & Ermon (2020)](https://arxiv.org/abs/2006.09011) enabled scaling score-based models to high-dimension data distributions and made them competitive on image-generation tasks. The key idea in their work was to perturb the data distribution with various levels of Gaussian noise and learn a noise-conditional score model to predict the score of the perturbed data distributions. 


In 2020, [Ho et al., (2020)](https://arxiv.org/abs/2006.11239) introduced  _denoising diffusion probabilistic models (DDPM)_, which served as the foundation for the success of Diffusion models. At that time, Diffusion models still were not  competitive with state-of-the-art generate models such as GANs. However, this changed rapidly the following year when [Nichol & Dhariwal (2021)](https://arxiv.org/abs/2105.05233) improved upon the previous paper and demonstrated, that Diffusion models are competitive with GANs on image synthesis tasks. Nevertheless, it is important to note, that Diffusion models are not the jack of all trades. Diffusion models still struggle with certain image traits such as generating realistic faces or generating the right amount of fingers. 

Another important idea for diffusion models in the context of image generation has been the introduction of _latent diffusion models_ by [Rombach & Blattman et al., (2022)](https://arxiv.org/abs/2112.1075). By training the diffusion model in the latent space rather than the image space directly, they were able to improve the sampling and training speed and made it possible for everyone to run their own diffusion model on local PCs with a single GPU. Recent AI generated art is mostly based on the stable AI implementation of latent diffusion models and is open source: [Github repo](https://github.com/CompVis/stable-diffusion). Check out some cool Diffusion art on the [stable-diffusion-reddit](https://www.reddit.com/r/StableDiffusion/).


**Conditional Diffusion models**
The initial diffusion models are usually trained on marginal distributions $p(x)$, but conditional image generation is also an research area of great interest. Therefore, we need conditional diffusion models to _guide_ the generation process. Currently, there are three common methods to enable conditional generation with diffusion models:

- Classifier Guided Diffusion by [Dhariwal & Nichol (2021)](https://arxiv.org/abs/2105.05233)
- Classifier-Free Guidance (CFG) by [Ho & Salimans, (2021)](https://openreview.net/forum?id=qw8AKxfYbI)
- directly training a conditional diffusion model $p(x|z)$ 

CFG is used in many applications, since it allows to train a conditional diffusion model  and unconditional diffusion model at the same time. During inference, we can combine both models and control the generation process using a guidance weight. 

**Diffusion models perspectives**

As previously mentioned, diffusion models can be viewed from two different perspectives:
- the denoising diffusion probabilistic perspective based on [Ho et al., (2020)](https://arxiv.org/abs/2006.11239) 
- the score-based model perspective based on  [Song & Ermon, (2019)](https://proceedings.neurips.cc/paper/2019/file/3001ef257407d5a371a96dcd947c7d93-Paper.pdf)

There has been a lot of effort to combine these two views into one general framework. The best generalization has been the idea of stochastic differential equations (SDEs) first presented in [Song et al. (2021)](https://arxiv.org/pdf/2011.13456) and further developed to unified framework in [Karras et al. (2022)](https://arxiv.org/pdf/2206.00364).

While diffusion models have mainly been applied in the area of generative modeling, recent work has shown promising applications of diffusion models in robotics. For instance, diffusion models have been used for behavior cloning and offline reinforcement learning, and have also been used to generate more diverse training data for robotics tasks.

Diffusion models offer several useful properties in the context of robotics, including:

- *Expressiveness*: can learn arbitrarily complicated data-distributions 
- *Training stability*: they are easy to train especially in contrast GANs or EBMs
- *Multimodality*: they are able to learn complicated multimodal distributions
- *Compositionality*: Diffusion models can combined in a flexible way to jointly generate new samples

Overall, diffusion models have the potential to be a valuable tool for robotics.

---