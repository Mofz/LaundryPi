OPTSO = -fpermissive -Wall -g -std=c++11 -o
OPTSC = -fpermissive -Wall -g -std=c++11 -c




main: main.o hardware.o GPIOClass.o
	g++ $(OPTSO) main main.o hardware.o GPIOClass.o Socket.o

main.o: main.cpp hardware.h
	g++ $(OPTSC) main.cpp

hardware.o: hardware.cpp hardware.h
	g++ $(OPTSC) hardware.cpp

GPIOClass.o: GPIOClass.cpp GPIOClass.h
	g++ $(OPTSC) GPIOClass.cpp