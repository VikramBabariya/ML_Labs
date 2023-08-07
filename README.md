# Chandrayan 🚀

> You can control the chandrayan by giving sequence of commands.


## Project Functionality

Spacecraft has position cordinates in 3d galaxy as (x, y, z) and it is facing one of six direction North(N), South(S), West(W), East(E), Up(U) or Down(D).

Spacecraft has mainly 2 functionalities
  1. Move the Spacecraft forward(f) or backward(b).
  2. turn the Spacecraft 90 degree to left(l), right(r), up(u), down(d)

*Note: f, b, l, r, u, d represents commands.*

### Move Function
After every move command spacecraft position will change. One of its cordinated will be incremented or decremented by 1. See below cases to understand move better.
Assume initial position as (x, y, z).
- Facing Direction = N and Command = f  --> new position (x, y+1, z)
- Facing Direction = N and Command = b  --> new position (x, y-1, z)
- Facing Direction = S and Command = f  --> new position (x, y-1, z)
- Facing Direction = S and Command = b  --> new position (x, y+1, z)
- Facing Direction = E and Command = f  --> new position (x+1, y, z)
- Facing Direction = E and Command = b  --> new position (x-1, y, z)
- Facing Direction = W and Command = f  --> new position (x-1, y, z)
- Facing Direction = W and Command = b  --> new position (x+1, y, z)
- Facing Direction = U and Command = f  --> new position (x, y, z+1)
- Facing Direction = U and Command = b  --> new position (x, y, z-1)
- Facing Direction = D and Command = f  --> new position (x, y, z-1)
- Facing Direction = D and Command = b  --> new position (x, y, z+1)


### Turn Function
After every turn command spacecraft facing direction will change. See below cases to understand turn better.
- Facing Direction = N and Command = l --> new Direction = W
- Facing Direction = N and Command = r --> new Direction = E
- Facing Direction = N and Command = u --> new Direction = u
- Facing Direction = N and Command = d --> new Direction = d
...

  

## TechStack
- Backend: Python 
- Unit Testing Framework: unittest


## Follow Below steps to run the project.

1. Clone this repo in your github account.
2. Download the source code on your machine.
3. Make sure you have python installed on your machine.
4. Open this project in your favorite ide.
5. Run this command in command prompt of ide to execute the tests.  -->   "python test_spacecraft.py"
