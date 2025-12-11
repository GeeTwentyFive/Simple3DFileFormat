**CURRENTLY WIP**

FILE EXTENSION: `.s3d`

FORMAT (binary data):
```
u32 num_verts | u32 num_indices |
<VERTICES> (f32 pos_x, f32 pos_y, f32 pos_z, f32 norm_x, f32 norm_y, f32 norm_z, f32 col_red, f32 col_green, f32 col_blue)... |
<INDICES> (u32)...
```

Official C reader & writer lib: https://github.com/GeeTwentyFive/S3DLib

Official Python reader & writer lib: https://github.com/GeeTwentyFive/PyS3D

Official CLI converter: https://github.com/GeeTwentyFive/S3DConverter

Official runtime Godot loader: https://github.com/GeeTwentyFive/GodotS3DLoader


# Motive

If you don't want to do fancy-shmancy stuff like PBR, bump mapping, parallax, etc., then most existing 3D model file formats are quite... inconvenient...

The Simple3D (.s3d) file format just gives you a mesh straight up
