# Niagara Ocean Tutorial
![Niagara Ocean Tutorial](https://ue-cdn.artstation.com/imgproxy/1kSRVkbimokkNDxfTFPOSonku4DPuw5wxHV2WwJcM5o/filename:OceanTutorial_Banner.png/resizing_type:fill/width:1600/height:200/aHR0cHM6Ly9kMWl2N2RiNDR5aGd4bi5jbG91ZGZyb250Lm5ldC9pbWFnZXMvMjc3ZmU4NTgtNTZlNS00NjE4LWEyYmYtYWRhNDA3YzljYmIwL29jZWFudHV0b3JpYWxfYmFubmVyLnBuZw)
This is a UE 5.3 fork of Niagara Ocean FX (GPU): very fast and realistic water.

Tutorial: https://dev.epicgames.com/community/learning/tutorials/qM1o/unreal-engine-ocean-simulation

Discussion: https://forums.unrealengine.com/t/community-tutorial-ocean-simulation/845453

## Notes:
To make "FX_OceanWater" shader compile, edit the shader:

1. In "WaterSim" node doubleclick "FX_OceanWater_Timestep", find "Custom Hlsl", in Details change "Absolute Include File Path" (3 dots) to your "OceanComplexMath.ush" file path,
2. Repeat: in  "FX_OceanWater_Rowpass" -> "OceanWater.ush",
3. Repeat: in "FX_OceanWater_Colpass" -> "OceanWater.ush",
4. Repeat: in "FX_OceanWater_ExportData" -> "OceanExport.ush",

If you're getting glitched ocean, find "OceanWater.ush" file
 and search for "groupshared float3 pingPongArray" there,
change "[256]" to something like "[128]" or "[64]".

## URLs:
https://dev.epicgames.com/community/learning/tutorials/qM1o/unreal-engine-ocean-simulation
https://forums.unrealengine.com/t/community-tutorial-ocean-simulation/845453/36