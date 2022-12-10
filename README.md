# doom_rl
Reinforcement Learning agent trained to play Doom 

## Setup
1) clone repo
2) in repo directory create github subdirectory
3) in github subdirectory clone https://github.com/Farama-Foundation/ViZDoom.git

## Deadly Corridor Training
Because the deadly corridor level is difficult for the agent to learn two factors needed to be included. Reward shaping (which is done in the deadly corridor notebook), and Curriculum learning (which we need to set up in vizdoom config)

### Setting Up Curriculum Learning
To set up curriculem learning for the deadly corridor level:
1) navigate to github/VizDoom/scenarios
2) make copies of the deadly_corridor.cfg file named:
    deadly_corridor_s1.cfg
    deadly_corridor_s2.cfg
    deadly_corridor_s3.cfg
    deadly_corridor_s4.cfg
    deadly_corridor_s5.cfg
3) In each of the above files there should be a doom_skill variable on line 8. Alter this value to match the s level (i.e. in deadly_corridor_s1.cfg, doom_skill = 1)
At this point the deadly correidor agent is ready for training