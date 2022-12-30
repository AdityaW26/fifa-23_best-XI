# FIFA-23 BEST XI PREDICTION
This notebook predicts The Best-XI team according to the statistics provided by EA Sports FIFA-23.

![dataset-cover](https://user-images.githubusercontent.com/68528440/210042100-f45931c4-4513-4554-9e70-fb22a281e614.png)


**Dataset link** - *[FIFA-23 dataset](https://www.kaggle.com/datasets/sanjeetsinghnaik/fifa-23-players-dataset)*

## Player selection criteria

#### 7 Best-XI teams are predicted according to different formations generally used in football. These seven formations along with their possible positions are*:
- 4-4-2: 
    - 4-4-1-1: ST, CF, LWB, LM, RM, RWB, LB, LCB, RCB, RB, GK 
    - 4-1-2-1-2: ST, CF, CAM, LM, RM, CDM, LB, LCB, RCB, RB, GK 
- 4-3-3:
    - 4-3-2-1: LW, CF, RW, LM, CM, RM, LB, LCB, RCB, RB, GK 
    - 4-1-2-3: LW, ST, RW, CAM, CM, CDM, LB, LCB, RCB, RB, GK 
- 3-4-3: LF, CF, RF, LM, CAM, CDM, RM, LB, CB, RB, GK 
- 3-5-2: ST, CF, LWB, CAM, RWB, LDM, RDM, LB, CB, RB, GK 
- 5–4–1: CF, LM, LCM, RCM, RM, LWB, LB, CB, RB, RWB, GK 

#### A player is selected in the Best-XI based on : 
- being the best in his position in that particular formation
- player should have played that particular position previously for his club/nation

#### Stalemate situations
A difficult selection situation may arise in following cases:
- a player can be best in more than one positions. In such a case the priority is given to the position starting from left to right (L->R, with highest priority to Left) and forward to defense (F->D, with highest priority to Forward)


An impasse may arise in following cases:
- a player with being the best in his position and playing that position in his previous career is not found
- the function used to find a player reaches a maximum recursion depth (for jupyter notebook depth being 1000)


**In above mentioned cases, the position of the player in the formation can be changed.**


_(*- positions are subject to change according to code requirements)_
