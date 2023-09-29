## Some Robotics Projects I've Worked On

### Trajectory Tracking with Baxter
<iframe width="560" height="315" src="https://www.youtube.com/embed/-fLwfQ-J4Og?si=EuU70OBeg7r0AyiB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Trajectory tracking with Baxter (by Rethink Robotics with seven degree-of-freedom arm) with the construction of three different controllers: workspace velocity, jointspace velocity, and jointspace torque. In order to effectively test the differences between our controllers, we drove our manipulator arm using a number of distinct controller paradigms, each of which we created and tuned by hand. These included (A) a purely feed-forward controller, (B) a tuned jointspace-velocity controller, (C) a tuned workspace-velocity controller, (D) a jointspace torque controller, and finally, (E) a controller provided by the MoveIt! library, a professional control library to serve as an experiment control. With each controller, we ran a set of three trajectories, which included (1) a linear motion between two points in space, (2) a circular motion around a predefined central point, and (3) a polygonal trajectory consisting of a linked set of linear trajectories.


### Nonholonomic Control: Skrrt skrrt we're driving!
Can I parallel park? Not really. How well can a robot accomplish one? Let's see.
                
In this project, we implement and compare three different methods and modalities of planning algorithm in order to compare their results on a number of simulated and real-world tasks. 
These planners include a trajectory cost-optimization planner, a sampling-based planner (RRT), and a nonholonomic sinusoidal steering algorithm (steering with sinusoids).
We tested planners on three simple point-to-point navigation tasks (a forward motion, sideways ”parallel park” path, and a three-point turn), as well as two obstacle avoidance environments.
Below are visualizations of each planner’s concrete performance on each task, demonstrating each model’s approach to solving an environment. 
This analysis allows us to demonstrate the applicability of each individual algorithmic approach to a variety of different motion planning tasks, and more intelligently choose a planner for any specific task.

Note: Middle graph demonstrates RRT--planned path is in green, and the alternate paths explored by the algorithm are in yellow.