# NeRF Relighting & Compositing
NeRF-RC builds on the work of [NeRF-OSR](https://github.com/r00tman/NeRF-OSR) and [SAMURAI](https://github.com/google/samurai) to develop a solution that integrates 3D mesh objects into a volumetric scene generated by the NeRF (Neural Radiance Field) model. The solution will also allow for adjusting global lighting in a way that affects both the NeRF environment and the embedded 3D meshes. The integration of 3D meshes into NeRF scenes will likely result in more realistic and dynamic environments. The ability to adjust global lighting will further enhance the realism of the overall scene. The use of NeRF and NeRF Relighting has gained significant attention in both the computer vision and computer graphics communities in recent years due to its impressive results in reconstructing and relighting 3D scenes.

## Pipeline
1. NeRF-OSR to extract scene illumination
2. SAMURAI to extract object shape and BRDF
3. Combine -> novel lightning + novel viewpoint
4. Render the result
