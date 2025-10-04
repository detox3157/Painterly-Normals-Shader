# Painterly Normals Shader
Available for free on Unity Asset Store

## Showcases
![detoxx3157-screenshot-2025-07-05-at-16-35-56-png](https://github.com/user-attachments/assets/2b2e30e0-0cc6-44f6-a430-b2121a5ded5c)
![detoxx3157-screenshot-2025-07-05-at-16-38-11-png](https://github.com/user-attachments/assets/fd179013-f6f9-41c0-8a92-718cea437234)
![detoxx3157-screenshot-2025-07-05-at-16-48-12-png](https://github.com/user-attachments/assets/3d400869-d7b0-4d76-9aac-3cc6e0e0aac2)
![detoxx3157-screenshot-2025-07-05-at-16-43-53-png](https://github.com/user-attachments/assets/650cf89a-f857-43f6-8537-493bd3994616)

## Principle of work
The shader as simple as it can be. We take the standard Object Space normals.

![detoxx3157-screenshot-2025-09-19-at-23-53-15](https://github.com/user-attachments/assets/c8686507-7510-4e15-bdf9-13cd6fdb6306)

Transform them using Voronoi 3D noise

![detoxx3157-screenshot-2025-09-19-at-23-53-31](https://github.com/user-attachments/assets/e7df87aa-2d18-4498-a62a-5180cbf91b14)

Add some simple small-fraction blending noise

![detoxx3157-screenshot-2025-09-19-at-23-53-48](https://github.com/user-attachments/assets/d01476b5-5fb0-477e-aeee-f20d7b6ab95b)

## Potential Improvement
Potential improvement can be baking the noise as a high N-resolution texture for N*N vectors evenly distributed on a unit sphere, then sampling this texture in shader. This method can give a small improvement in performance, although makes the noise easier to recognize and less flexible overall.

