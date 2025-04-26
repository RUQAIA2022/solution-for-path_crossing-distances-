# solution-for-path_crossing-distances-

1.Initialize the starting position at (0, 0).

2.Save the starting point (0, 0) in a set called visited.

3.Define the movement directions:

Up: (0, 1)

Left: (-1, 0)

Down: (0, -1)

Right: (1, 0)

4.Initialize dir_idx = 0 to track the current direction (starts with Up).

5.For each distance in the distances list:

*Get the direction (dx, dy) based on dir_idx.

*Move one step at a time:

*Update the current position: x += dx, y += dy.

*Check if the new position (x, y) is already in visited:

*If yes, return True (path crosses itself).

*Otherwise, add the new position (x, y) to visited.

*After moving, update dir_idx to the next direction clockwise:

(dir_idx + 1) % 4.

6.If all moves complete without revisiting any point, return False (path does not cross).

