# CMPM163Labs
lab 2: https://drive.google.com/open?id=1_TnqecQWUwk1OoCeVVfCuX8CIy_TbgWd

![](lab2/lab2%20model%20scene%20screenshot.png)

lab 3: https://drive.google.com/file/d/1Pwv4xZxxUiEZv_Sw24143XEYQn1M42gX/view?usp=sharing

Cube 1 (Crimson): This cube was made with Three.js materials. I changed the color of this cube to crimson, and added a red specular value, along with increased shine.
Cube 2 (Turquoise and Red): This cube was built with my shaders, and I chose the colors turquoise and red for its interpolation.
Cube 3 (Default): This cube was made with Three.js materials. This cube was not changed from how it started (as intended by the lab instructions.)
Cube 4 (Blue and Green): This cube was built with my shaders, and I chose the colors blue and green for its interpolation.

lab 4:
https://drive.google.com/file/d/1PeRZodNdlyG-TQyRmuG3aizkzOYaMy4u/view?usp=sharing

24a. The formula would be x = ⌊u * 7⌋.
24b. The formula would be y = ⌊7 - (v * 7)⌋
24c. x = ⌊0.375 * 7⌋ = 2, y = ⌊7 - (0.25 * 7)⌋ = ⌊7 - 1.75⌋ = 5
   thusly, we sample the coordinate at (2,5), which is the color gray.
   
Cube 1: I used textures and normal maps from the lab's included drive folder for every cube. For cube 1, I used 156.jpg, and built it with the three.js built in texture functionality. This cube went on the left.
Cube 2: This cube was the same as the first, but I also used 156_norm.jpg as a normal map, matching the texture. This cube went in the middle, and used the three.js built in texture functionality.
Cube 3: For this cube, I used the three.js built in texture functionality, but I also used 151.jpg as a texture, and 152_norm.jpg as a normal map. This cube went above the others. (This cube is also labeled as cube4 in my code.)
Cube 4: For this cube, I loaded the texture 157.jpg with the supplied shaders, and moved the cube to the right. (This cube is also labeled as cube3 in my code.)
Cube 5: For this cube, I used texture 179.jpg, and tiled it in a 2x2 grid. My new shaders were created in seperate shader files, then loaded into lab4.html through code, as the others were. In vertexShader2.vert, I simply wrote "vUv = uv * 2.0;" instead of the default definition. Then, in fragmentShader2.frag, I changed the texture2D code to call "mod(vUv, 1.0)" instead of just "vUv" inside of the function arguments.
