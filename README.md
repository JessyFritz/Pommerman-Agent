# Pommerman-Agent
This notebook trains an agent for the Pommerman environment using a DQN.

**Note**: If possible, use Colab for an easier install.

Agent will be trained on the pixel representations of the fully observable state, where the frame stack consists of downscaled grayscale images. It can perform six different actions (Stop, Up, Down, Left, Right, Bomb). The network consists of 3 Conv Layers with ReLU activations and 2 final Linear Layers.

The notebook performs Curriculum Learning with 5000 episodes against no_bomb_random_actor and 25000 episodes against the SimpleAgent.
The final win ratio after a day of training was above 55%. The following image shows the increase in performance for the first 5000 played games.

<img src="https://user-images.githubusercontent.com/39498906/183265175-900bd7e5-0744-46f8-a88c-87a0450530cc.png" width="800">

![image](https://user-images.githubusercontent.com/39498906/183265044-55e1fefa-c541-400c-b717-f002b364058f.png)
