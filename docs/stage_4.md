### `Build volumetric mesh`
This step generates a 3D tetrahedral mesh (interior filled with tetrahedra, not empty)
-	Make sure the four important parameters are correct
    - `Z-scaling`: um/pixel in Z
    - `XY-scaling`: um/pixel in XY
    - `E`: Young’s modulus in kPa
    - `Nu`: Poisson’s ratio

> how thick is the material?  
> We can also set that if needed (advanced mesh options - thickness)

### Click the `>`
This solves the finite element model. Two results will be automatically saved at the same folder as the input image.
-	`{FileName}.vtu`
-	`{FileName}.all.vtu`

They are essentially the same except the “all” one saves the entire box and the other one saves only one surface (the surface with the mesh we care about).
