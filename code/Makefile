LIBS = -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio
CXX = g++
DEPS = Bob.h Engine.h Hud.h LevelManager.h PlayableCharacter.h SoundManager.h TextureHolder.h Thomas.h
OBJ = Bob.o DetectCollisions.o Draw.o Engine.o Hud.cpp Input.o LevelManager.o LoadLevel.o Main.o PlayableCharacter.o PopulateEmitters.o SoundManager.o TextureHolder.o Thomas.o Update.o

all: ThomasWasLate

%.o: %.cpp $(DEPS)
	$(CXX) -c $< -o $@

ThomasWasLate: $(OBJ)
	$(CXX) -o $@ $^ $(LIBS)

clean:
	@echo "Removing files"
	rm -rf ThomasWasLate *.o
