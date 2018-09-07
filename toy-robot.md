# Toy Robot Task 
You have a toy robot on a table top, a grid of 5 x 5 units, there are no obstructions. You can issue commands to your robot allowing it to roam around the table top. But be careful, don't let it fall off!

## Commands
The robot should be able to process the following commands.

### `PLACE X,Y,FACING`

* Puts the toy robot on the table in position X,Y and facing NORTH, SOUTH, EAST or WEST.
* The origin (0,0) can be considered to be the SOUTH WEST most corner.
* The first valid command to the robot is a PLACE command, after that, any sequence of commands may be issued, in any order, including another PLACE command.
* The application should discard all commands in the sequence until a valid PLACE command has been executed.

### `MOVE`

Moves the toy robot one unit forward in the direction it is currently facing.

### `LEFT`

Will rotate the robot 90° anticlockwise without changing the position of the robot.

### `RIGHT`

Rotate the robot 90° clockwise without changing the position of the robot.

### `REPORT`

Outputs the X,Y and F of the robot. This can be in any form, but standard output is sufficient.

## Constraints
* The robot is free to roam around the surface of the table, but must be prevented from falling to destruction. 
* Any movement that would result in the robot falling from the table must be prevented, however further valid movement commands must still be allowed.
* Input can be from a file, or from standard input, as the developer chooses.
* You need to provide test data/results for the app & its logic.


## Example Input & Output

* `place 0,0,NORTH`
* `move`
* `report` 
    *  `0, 1, NORTH`
* `place 0, 0, NORTH`
* `left`
* `report` 
    *  `0, 0, WEST`
* `place 1,2,EAST`
* `move`
* `move`
* `left`
* `move`
* `report`
    *  `3, 3, NORTH`



## Our Expectations

* Be sure to write comments and a README. Provide instructions on how to run the project and any notes about your solution.
* Feel free to use any .NET framework past 4.6 (most projecs here are 4.6, 4.7 & .NET Core).
* We're most interested to see problem solving and your approach.
* Keep it simple, keep it DRY, but don't over complicate or over engineer, comment and test as much as possible.
* Commit your code to a public Git repository and provide us with the URL.
* Don't spend days on this, but do let us know what you think is missing and what you'd add given more time.
#
[![Part of Zone Backend][zone-be-image]][zone-be-url]


[zone-be-image]: https://img.shields.io/badge/-backend-lightgrey.svg?logo=data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTMgMTQiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayI+ICAgIDxwb2x5Z29uIGlkPSJTaGFwZSIgZmlsbD0iI0ZGRkZGRiIgZmlsbC1ydWxlPSJub256ZXJvIiBwb2ludHM9IjYuMjc3NjY4NzEgMTAuNzU0MjMzMSAxMi45OTU5NTA5IDAgMi43MzMwMDYxMyAwIDAuNzMwMDYxMzUgMy4xOTc2Njg3MSA2LjcxOTE0MTEgMy4xOTc2Njg3MSAwIDEzLjk1MTA0MjkgMTAuMjU5NTA5MiAxMy45NTEwNDI5IDEyLjI2MzMxMjkgMTAuNzUxNjU2NCI+PC9wb2x5Z29uPjwvc3ZnPg==&longCache=true&style=flat-square&colorA=2C2B39&colorB=1010E5
[zone-be-url]: https://github.com/zone/
