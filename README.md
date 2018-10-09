# Robocode
CamPiqBot is a simple robot programmed in java for [robocode](https://robocode.sourceforge.io)

## Main features
These are the main features that CamPiqBot has

### Wall Avoidance
To avoid hit the limits of the battlefield, the robot has two points in front of it, fixed at 45 degrees of amplitude on each side. In this way, when one of the two points leaves the battlefield, it knows that it must turn in the opposite direction. If the two points are outside the battlefield, it means that the robot is perpendicular to a wall or approaches a corner, in which case it will turn around.

### Firepower decision
Each shot that does not hit the enemy is a waste of energy. For this reason, environmental variables are taken into account, such as the distance to the enemy to be fired, the energy of the enemy, the energy of our own robot and the necessary turning angle of our weapon. It is thus tried to reduce the loss of energy in the shots.

### Scanning strategy
The robot's radar sweeps 360 degrees to search for enemies. When the robot finds one, try to fix it in the spotlight and not lose it. In this way we have the necessary data to adjust the angle of our weapon and shoot.

### Movement
The movement when no event is activated is in a straight line by default. If the robot is near a wall, make a sufficient turn in the direction indicated by its sensors to avoid it. If the robot has detected an enemy, try to move in circles around it, to avoid losing it and increase the chances of hitting it with a bullet.

### Other features
* Change its movement speed depending on the number of robots on the battlefield
* When it is hit by a bullet it changes his trajectory
* When it hits a robot, it checks if it can shoot and then moves away

## Author

* **Luis Cambero** - [lcambero](https://github.com/lcambero)

## Last update

October 9, 2018

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
