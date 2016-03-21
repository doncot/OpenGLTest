GLEW_INCLUDE = /usr/local/Cellar/glew/1.13.0/include
GLEW_LIB = /usr/local/Cellar/glew/1.13.0/lib 

hello-gl: hello-gl.o util.o
	gcc -o hello-gl $^ -framework OpenGL -framework GLUT -L$(GLEW_LIB) -lglew

.c.o:
	gcc -c -o $@ $< -I$(GLEW_INCLUDE)

clean:
	rm -f hello-gl hello-gl.o util.o
