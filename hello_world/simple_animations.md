# Simple Animations

```
import pygame, sys
from pygame.locals import *

pygame.init()

DISPLAYSURF = pygame.display.set_mode((500, 400))
BLACK = (0, 0, 0)
BLUE = (0, 0, 255)
rect_x = 10
rect_y = 10

clock = pygame.time.Clock()

while True:
    for event in pygame.event.get():
        if event.type == QUIT:
            pygame.quit()
            sys.exit()

    # to animate, we have to reset the screen
    DISPLAYSURF.fill(BLACK)
    pygame.draw.rect(DISPLAYSURF, BLUE, (rect_x,rect_y, 50, 50))

    # move the rect
    rect_x += 1
    rect_y += 1

    # force 20 frames
    clock.tick(120)

    pygame.display.flip()
```

Here is a simple way to animate a rectangle. The logic is as follows:

1. Draw a new screen `DISPLAYSURF.fill(BLACK)`.
2. Draw a rectangle, shifting its coordinates.
3. Repeat


