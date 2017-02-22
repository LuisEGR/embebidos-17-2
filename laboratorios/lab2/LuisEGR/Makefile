#Archivo Makefile simplea
#PROYECTO=muestreo --> Variable, usar así: $(PROYECTO)
#Variables automáticas
#	$@ -> hace referencia al nombre del objetivo
#	$< -> hace referencia a la primer dependencia de una regla
#	$^ -> hace referencia a todas las dependencia de una regla
#	$? -> Lista de espacio delmitado de todas las dependencias de una
#       regla que son más nuevas que el objetivo
PROYECTO=muestreo
DESTDIR=/usr/local/bin
CFLAGS=-Wall
LDFLAGS=-lm
CC=gcc
OBJS=$(patsubst %.c,%.o,$(wildcard *.c))

all:$(PROYECTO)

%.o: %.c
	$(CC) -c $< $(FLAGS)
# Esta linea de arriba sustituye los objetivos de abajo (.o)
# muestreo.o:muestreo.c
# 	$(CC) -c muestreo.c $(CFLAGS)
#
# procesamiento.o:procesamiento.c
# 	$(CC) -c procesamiento.c $(CFLAGS)
#
# archivos.o:archivos.c defs.h
# 	$(CC) -c archivos.c $(CFLAGS)

### BUSCAR COMO GENERALIZAR ESTA LINEA: (WILDCARD)
$(PROYECTO): $(OBJS)
	$(CC) $^ -o $@ $(LDFLAGS)
	#$(CC) muestreo.o procesamiento.o archivos.o -o $(PROYECTO) $(LDFLAGS)

.PHONY: clean

install: all
	if	[ ! -d $(DESTDIR)	]; then \
		sudo	mkdir $(DESTDIR); \
	fi; \
	sudo cp $(PROYECTO) $(DESTDIR)

uninstall:
	sudo rm $(DESTDIR)/$(PROYECTO)

clean:
	rm -f *.o m
