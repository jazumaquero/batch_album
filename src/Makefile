# Compiler and compiling/linking options
CC=g++
CFLAGS=-c -Wall
LDFLAGS=

# Source code, objects and executables filenames
SOURCES=main.cpp
OBJECTS=$(SOURCES:.cpp=.o)
EXECUTABLE=hello

# Compile all and link them into main executable
all: $(SOURCES) $(EXECUTABLE)
	@echo "Build success!"

# Clean all generated resources
clean:
	@echo "Cleaning Objects..."
	rm $(OBJECTS)
	@echo "Cleaning executables..."
	rm $(EXECUTABLE)
	@echo "Cleaning success!"

# Link all sources
$(EXECUTABLE): $(OBJECTS)
	$(CC) $(LDFLAGS) $(OBJECTS) -o $@

# Compile all sources
.cpp.o:
	$(CC) $(CFLAGS) $< -o $@
