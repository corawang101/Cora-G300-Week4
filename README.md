- Two paddles controlled by keyboard input
  - Left Player: W / S
  - Right Player: I / K
- A physics-based ball that moves and bounces off paddles and walls
- Custom physical material with high restitution and no friction
- Score zones on both sides of the board
- Score tracking using a custom Game Instance
- Ball automatically respawns after a player scores

## Destroyable Obstacle System
I added a `CanDestroy` boolean to the Pong ball. Normally, this value is false. When the ball passes through the Destroy Power Zone, `CanDestroy` becomes true. If the ball then hits a destroyable obstacle, the obstacle is destroyed and `CanDestroy` is changed back to false. This means the ball must pass through the power zone again before it can destroy another obstacle.

## Bonus Score
Bonus score zones that give more points than normal score zones.
