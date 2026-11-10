# Demonstration-Free Skill Composition for Navigation and Manipulation

*Australasian Conference on Robotics and Automation (ACRA 2026)*

We study how reinforcement learning policies trained on individual skills can be combined and reused to solve longer tasks without expert demonstrations.

- **Navigation in MiniGrid FourRooms.** A manually specified plan combines two learned skills, `GoTo` and `CrossDoor`. Across 10 previously unseen layouts, the combined skills achieve 55.5% mean success, compared with 2.0% for a flat DQN given the doorway coordinates.

- **Manipulation in Robosuite.** The `Reach` → `Grasp` → `Lift` chain picks up and lifts a cube in 85.8% of 450 evaluation trials. Keeping these three policies frozen and training only an additional `Place` skill gives 71.6% success on cube stacking.
