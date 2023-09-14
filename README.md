# Niagara Ocean Tutorial
![Niagara Ocean Tutorial](https://ue-cdn.artstation.com/imgproxy/1kSRVkbimokkNDxfTFPOSonku4DPuw5wxHV2WwJcM5o/filename:OceanTutorial_Banner.png/resizing_type:fill/width:1600/height:200/aHR0cHM6Ly9kMWl2N2RiNDR5aGd4bi5jbG91ZGZyb250Lm5ldC9pbWFnZXMvMjc3ZmU4NTgtNTZlNS00NjE4LWEyYmYtYWRhNDA3YzljYmIwL29jZWFudHV0b3JpYWxfYmFubmVyLnBuZw)
This is a UE 5.3 fork of Ocean Niagara FX (GPU): very fast and realistic looking water.

## Video sample
https://vimeo.com/814697784

## Notes:
If you're getting glitched ocean, find `AwesomeShaders/OceanWater.ush` file
uncomment `#define THREADGROUP_SIZE 256` and
change `256` to something like `128` or `64` (it's GPU dependent, I guess).

## URLs:
Tutorial: https://dev.epicgames.com/community/learning/tutorials/qM1o/unreal-engine-ocean-simulation
Discussion: https://forums.unrealengine.com/t/community-tutorial-ocean-simulation/845453

## Thanks
* `DeathreyCG` for the awesome Niagara FX
* `Evil_Pee` for USH relative path project
