# Rir
import pygame
from pygame.draw import *

pygame.init()

FPS = 30
screen = pygame.display.set_mode((400, 400))

rect(screen, (0, 255, 255), (0, 0, 400, 200))

rect(screen, (0, 255, 0), (0, 200, 400, 400))
ellipse(screen, (127,127,127), (50, 190, 40, 60))
circle(screen, (235,245,255), (70, 180), 20)
ellipse(screen, (127,127,127), (290, 190, 40, 60))


circle(screen, (235,245,255), (150, 180), 20)
circle(screen, (235,245,255), (230, 180), 20)
circle(screen, (235,245,255), (310, 180), 20)
polygon(screen, (255,100,180), [(153,200),(147,200),
                               (125,250), (175,250)], )
polygon(screen, (255,100,180), [(235,200),(225,200),
                               (205,250), (260,250)], )

polygon (screen, (0,0,0), [(85,200),(110,220), (85,200)])
polygon (screen, (0,0,0), [(147,200),(110,220), (147,200)])
polygon (screen, (0,0,0), [(235,200),(265,220), (235,200)])
polygon (screen, (0,0,0), [(295,200),(265,220), (295,200)])
polygon (screen, (0,0,0), [(325,200),(360,220), (325,200)])
polygon (screen, (0,0,0), [(55,200),(30,220), (55,200)])
polygon (screen, (0,0,0), [(225,200),(200,220), (225,200)])
polygon (screen, (0,0,0), [(225,200),(200,220), (225,200)])
polygon (screen, (0,0,0), [(153,200),(180,220), (153,200)])
polygon (screen, (0,0,0), [(190,210),(180,220), (190,210)])
polygon (screen, (0,0,0), [(190,210),(200,220), (190,210)])
polygon (screen, (0,0,0), [(190,150),(190,210), (190,150)])
polygon (screen, (0,0,0), [(190,150),(190,210), (190,150)])
polygon (screen, (255,200,0), [(165,100),(190,150), (220,100)])

circle(screen, (100,40,0), (180, 100), 12)
circle(screen, (255,0,0), (204, 100), 12)
circle(screen, (255,255,255), (190, 85), 12)

polygon (screen, (0,0,0), [(80, 285),(80, 245), (80,285)])
polygon (screen, (0,0,0), [(90, 285),(80, 285), (90,285)])
polygon (screen, (0,0,0), [(60, 285),(60, 245), (60,285)])
polygon (screen, (0,0,0), [(50, 285),(60, 285), (50,285)])

polygon (screen, (0,0,0), [(140, 285), (140, 250), (140,285)])
polygon (screen, (0,0,0), [(130, 285), (140, 285), (130,285)])

polygon (screen, (0,0,0), [(160, 285),(160, 250), (160,285)])
polygon (screen, (0,0,0), [(170, 285), (160, 285), (170,285)])


polygon (screen, (0,0,0), [(225, 285),(225, 250), (225,285)])
polygon (screen, (0,0,0), [(210, 285), (225, 285), (210,285)])

polygon (screen, (0,0,0), [(240, 285),(240, 250), (240, 285)])
polygon (screen, (0,0,0), [(255, 285), (240, 285), (255, 285)])

polygon (screen, (0,0,0), [(305, 285),(305, 250), (305,285)])
polygon (screen, (0,0,0), [(290, 285), (305, 285), (290,285)])

polygon (screen, (0,0,0), [(315, 285),(315, 250), (315,285)])
polygon (screen, (0,0,0), [(330, 285), (315, 285), (330,285)])

polygon (screen, (0,0,0), [(305, 285),(305, 250), (305,285)])
polygon (screen, (0,0,0), [(290, 285), (305, 285), (290,285)])


polygon (screen, (0,0,0), [(20,150), (30, 220), (20,150)])
polygon (screen, (255,0,0), [(0,130),(20,160), (40,130)])

circle(screen, (255,0,0), (12, 130), 12)
circle(screen, (255,0,0), (30, 130), 12)

polygon (screen, (255,200,0), [(360, 200 ), (360, 220), (375,205)])

circle(screen, (100,40,0), (365, 200), 5)
circle(screen, (255,0,0), (372, 201), 5)

circle(screen, (255,255,255), (369, 195), 5)



pygame.display.update()
clock = pygame.time.Clock()
finished = False

while not finished:
    clock.tick(FPS)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            finished = True

pygame.quit()