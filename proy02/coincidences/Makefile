CPP = g++
CC = gcc
CFLAGS = -Wall $(shell root-config --cflags) -O3
LIBS = -lm $(shell root-config --glibs) 
GLIBS = 
GLIBS += 
OBJECTS = coincidences.o 
HEADERS = 

ALL : coincidences.exe
	echo "Listo!"

coincidences.exe : $(OBJECTS)
	$(CPP) $(OBJECTS) -o coincidences.exe $(LIBS) $(GLIBS) $(CFLAGS)

coincidences.o : coincidences.cc $(HEADERS)
	$(CPP) -c coincidences.cc -o coincidences.o $(CFLAGS)

clean:
	rm -f *~ *.o *.exe
