# Primitive Drawings


```
import pygame, sys
from pygame.locals import *

pygame.init()

DISPLAYSURF = pygame.display.set_mode((500, 400))
BLUE = (0, 0, 255)
pygame.draw.rect(DISPLAYSURF, BLUE, (100,100, 50, 50))

while True:
    for event in pygame.event.get():
        if event.type == QUIT:
            pygame.quit()
            sys.exit()
    pygame.display.update()
```


## `pygame.draw`

This lets you draw objects on the screen. In this example, we have drawn a rectangle, where the 2nd argument is the colour, and 3rd argument is the location of the top left vertices of the rectangle, and the width and length of the rectangle.

Remember that pixel numbers are considered from the origin being the top left, where positive "x" goes in the right direction and "y" goes in the downward direction.

There are other shapes and objects you can draw including, cicles, ellipses, lines and polygons.

