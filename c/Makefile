OBJS = zpr.o zprdemo.o
CC = gcc
DEBUG = #-g
CFLAGS =  -c -w $(DEBUG) -O3 
LFLAGS =  $(DEBUG) -lm -lGL -lGLU -lglut #-framework Cocoa -framework GLUT -framework OpenGL
zpr: $(OBJS)
	$(CC)	$(OBJS)	-o	zpr	$(LFLAGS)
zpr.o: zpr.c  zpr.h
	$(CC)	$(CFLAGS)	zpr.c
zprdemo.o:	zprdemo.c	zpr.h	zpr.c
	$(CC)	$(CFLAGS)	zprdemo.c
