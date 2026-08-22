# Time-of-Flight Sensors: A Simple Guide

**Author:** Deborah Akuoko Minka

---

A time-of-flight (ToF) sensor measures distance by timing how long it takes for light to travel to an object and bounce back — like echolocation, but with light.

The sensor sends out a pulse of light, waits for it to return, and calculates distance from travel time. Because light speed is constant (~300,000 km/s), range follows directly from elapsed time.

## How Do They Work?

### Direct Time-of-Flight (dToF)

Direct ToF sensors measure the actual round-trip time of a light pulse:

**Distance = (Speed of Light × Time) ÷ 2**

The division by two accounts for the round trip to the object and back.

### Indirect Time-of-Flight (iToF)

Indirect ToF uses continuous waves and measures phase difference between emitted and returned light — suited to video-rate depth maps.

## What Makes Them Special?

- **Fast** — Many measurements per second for real-time use
- **Compact** — Modern ToF can fit on a single chip
- **Robust lighting** — Often works in dim conditions
- **Per-pixel depth** — A depth value for every pixel in the scene

## Where Are They Used?

- **Smartphones** — Portrait mode, AR, gestures
- **Gaming** — Body tracking and motion control
- **Autonomous vehicles** — Obstacle ranging and navigation
- **Robotics** — Mapping and manipulation
- **Industry** — Quality control and dimensional inspection

## SPAD Arrays

Advanced ToF systems use **Single-Photon Avalanche Diode (SPAD)** arrays that detect individual photons with sub-nanosecond timing — enabling millimetre accuracy at useful ranges and supporting SPAD-based vision research demos on [SPAD for Vision](https://huggingface.co/spaces/mvplus/spad_for_vision).

### CMOS ToF

Consumer ToF often uses integrated CMOS chips for cost-effective, compact depth sensing.

## Limitations

- **Range** — Best at short to medium distances (often up to ~10 m)
- **Specular surfaces** — Mirrors and shiny materials can confuse returns
- **Bright ambient light** — Can saturate or interfere with active illumination
- **Power** — Active illumination uses more energy than passive cameras

## Why They Matter for Vision Research

ToF adds depth that RGB alone cannot provide. Combined with spatial imaging, it supports:

- Better object recognition and segmentation
- Material-aware sensing when fused with time-resolved transients
- Safer autonomous and robotic systems
- Improved manufacturing inspection

## Conclusion

Time-of-flight sensors turn the speed of light into distance maps. Paired with spatial cameras and SPAD timing, they underpin modern spatiotemporal and material-classification pipelines — explore working examples on the [SPAD for Vision demo space](https://huggingface.co/spaces/mvplus/spad_for_vision).
