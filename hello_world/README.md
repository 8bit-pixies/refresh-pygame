# Hello World

```
import pygame, sys
from pygame.locals import *

pygame.init()
DISPLAYSURF = pygame.display.set_mode((400, 300))
pygame.display.set_caption("Hello World!")

while True:
    for event in pygame.event.get():
        if event.type == QUIT:
            pygame.quit()
            sys.exit()
    pygame.display.update()
```

From the analogous "Hello World" example, running this will generate an empty window with "Hello World" in the title.

## `pygame.display.set_mode()`

This creates the window with the size determined by the argument (the tuple).

## `pygame.display.set_caption()`

This method willadd the text that is at the top of the window.



