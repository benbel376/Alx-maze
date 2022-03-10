
### Creating a 3D maze with raycasting

**How to Compile and Run**
- [SDL2](https://www.libsdl.org/download-2.0.php) and [SDL2_image](https://www.libsdl.org/projects/SDL_image/) are required to compile and use this program
- Compile with `gcc 4.8.4` with the following flags:
    ``gcc -O2 -g -Wall -Werror -Wextra -pedantic -Isrc/headers *.c -lSDL2 -lSDL2_image -lm -o maze `sdl2-config --cflags --libs` `` OR `make -f Makefile`
- Run the maze: `./maze` or `./maze maps/<map_name>`
- Disable textures: `./maze no_tex` or `./maze maps/<map_name> no_tex`

-----

**Summary**

This 3D maze uses raycasting to draw the maze walls, utilizing [LodeV's](http://lodev.org/cgtutor/raycasting.html) method of using vectors to calculate ray length. By default the maze uses textures but textures can be disabled at execution.

** Resources**

- [LodeV Raycasting Tutorial](http://lodev.org/cgtutor/raycasting.html)