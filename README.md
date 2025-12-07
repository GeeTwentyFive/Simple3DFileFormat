FILE EXTENSION: `.s3d`

FORMAT (binary data):
```
i32 num_verts | i32 num_indices | i32 texture_width | i32 texture_height
<VERTICES> (f32 pos_x, f32 pos_y, f32 pos_z, f32 norm_x, f32 norm_y, f32 norm_z, f32 u, f32 v)... |
<INDICES> (i32)... |
<RGBA_TEXTURE_DATA> (u8 r, u8 g, u8 b, u8 a)...
```
