# Fast Catmull-Rom

MPV user shader.  
Fast Catmull-Rom approximation using 5 samples by omitting corners.

**FastCatmullRom_MAIN.glsl**  
Hooks main texture and scales it to ouput resolution.

**FastCatmullRom_LUMA.glsl**  
Hooks luma texture and scales it to ouput resolution.

**FastCatmullRom_CHROMA.glsl**  
Hooks chroma texture and scales it to luma resolution.

## Usage
- If you place shader in the same folder as your `mpv.conf`, you can use it with (example for **FastCatmullRom_MAIN.glsl**) `glsl-shaders-append="~~/FastCatmullRom_MAIN.glsl"`.
- Requires `vo=gpu-next`.