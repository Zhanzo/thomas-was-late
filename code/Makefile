LIBS = -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio
CXX = g++
DEPS = Bob.h Engine.h PlayableCharacter.h TextureHolder.h Thomas.h
OBJ = Bob.o Draw.o Engine.o Input.o Main.o PlayableCharacter.o TextureHolder.o Thomas.o Update.o

all: ThomasWasLate

%.o: %.cpp $(DEPS)
	$(CXX) -c $< -o $@

ThomasWasLate: $(OBJ)
	$(CXX) -o $@ $^ $(LIBS)

clean:
	@echo "Removing files"
	rm -rf ThomasWasLate *.o
