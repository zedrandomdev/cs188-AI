[CS188 course] (http://ai.berkeley.edu/home.html) at UC Berkely
#Intro to Artificial Intelligence
The purpose of this repository is to showcase projects I have been working on. Due to the honor code we are not allowed to post full code solutions to the problems and as such I will ***only*** present strategies and small demos.

I would recommend this course to anyone interested in an introduction to artificial intelligence and its applications. Particularly, the course does a very good job of tying together several related areas. For a full description please visit the [website] (http://ai.berkeley.edu/course_policies.html).

###Projects:
- [x] Search
- [x] MultiAgent Search
- [x] Reinforcement Learning
- [x] Hidden Markov Models
- [ ] Classification (machine learning)



#Search Project:
![alt text](https://github.com/ced92/cs188-AI/raw/master/Screenshots/searchProject.gif "A* Search")

* Goal: To take the optimal path in order to eat all the food pellets
* Solution: Implemented A* search with a heuristic aimed at measuring:
 * The distance to the closest food
 * The distance from that food to the most distant (if any) other food

#MultiAgent Project:
![alt text](https://github.com/ced92/cs188-AI/raw/master/Screenshots/multiAgent.gif "Expectimax Search and Evaluation function")

* Goal: To get highest score possible and avoid being eaten
* Solution: Implemented Expectimax pacman agent with a depth of two. Used an evaluation function for estimating the value of terminal states. Evaluation function consisted of a linear combination of variables such as:
 * Distance to the closest food
 * Location of power pellets
 * Ghost scared/not scared

#HHM Project:
![alt text](https://github.com/ced92/cs188-AI/raw/master/Screenshots/particleFilter.gif "HHM")

###Details:
In this project pacman is not able to "see" the ghosts but must sense them using a ***noisy sensor***.
The brightness of the colors reflect the probability that a ghost is in a particular location. There is one unique color per ghost.

* Goal: To track and eat all the ghosts
* Solution: Implemented an approximate solution for a hidden markov model (i.e. a particle filter) to track the location for each ghost + a greedy agent for agent 'action' choice.
