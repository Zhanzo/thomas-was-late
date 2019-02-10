LIBS = -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio
CXX = g++
DEPS = Engine.h TextureHolder.h
OBJ = Draw.o Engine.o Input.o Main.o TextureHolder.o Update.o

all: ThomasWasLate

%.o: %.cpp $(DEPS)
	$(CXX) -c $< -o $@

ThomasWasLate: $(OBJ)
	$(CXX) -o $@ $^ $(LIBS)

clean:
	@echo "Removing files"
	rm -rf ThomasWasLate *.o
