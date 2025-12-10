FILE EXTENSION: `.s3d`

FORMAT (binary data):
```
u32 num_verts | u32 num_indices | u32 texture_rgba_count |
<VERTICES> (f32 pos_x, f32 pos_y, f32 pos_z, f32 norm_x, f32 norm_y, f32 norm_z, f32 u, f32 v)... |
<INDICES> (u32)... |
<TEXTURE_RGBA> (u8 r, u8 g, u8 b, u8 a)...
```

Official C reader & writer lib: https://github.com/GeeTwentyFive/S3DLib

Official Python reader & writer lib: https://github.com/GeeTwentyFive/PyS3D

Official CLI converter: https://github.com/GeeTwentyFive/S3DConverter

Official runtime Godot loader: https://github.com/GeeTwentyFive/GodotS3DLoader


# Motive

If you don't want to do fancy-shmancy stuff like PBR, bump mapping, parallax, etc., then most existing 3D model file formats are quite... inconvenient...

Parsing them adds a bunch of code to one's application. Plus they tend to store textures as either paths or formatted data (PNG, JPG, ...), so that's another dependency and/or more code...

The Simple3D (.s3d) file format just gives you a mesh and its texture straight up
