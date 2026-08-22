# Spatial vs. Time-Resolved Images: Understanding the Difference

**Author:** Deborah Akuoko Minka

---

When we talk about images in computer vision and sensing, there are two main ways to capture information: spatial resolution and time resolution. Understanding the difference between these two approaches is key to understanding how modern vision systems work.

Think of it this way: **spatial images** tell you *where* things are, while **time-resolved images** tell you *when* things happen and how they change over time.

## Spatial Images: The "Where"

Spatial images are what we're most familiar with — regular photographs. A spatial image captures information about the position and appearance of objects in space at a single moment in time.

### Characteristics of Spatial Images

- **They show location** — You can see where objects are positioned relative to each other
- **They capture appearance** — Colors, textures, shapes, and patterns are all visible
- **They're like a snapshot** — They freeze a moment in time
- **High detail** — Modern cameras can capture millions of pixels, showing fine details

### Examples

- A regular photograph from your phone
- An X-ray image showing bone structure
- A satellite image of Earth
- A microscope image of cells

## Time-Resolved Images: The "When"

Time-resolved images capture information about how things change over time. Instead of just showing where something is, they show how it moves, changes, or evolves.

### Characteristics of Time-Resolved Images

- **They show temporal changes** — You can see how things move or transform
- **They capture dynamics** — Motion, decay, growth, and other time-based phenomena
- **They're like a movie** — Multiple snapshots over time create a sequence
- **Temporal precision** — Can capture events happening in nanoseconds or even faster

### Examples

- A video showing a ball bouncing
- A time-lapse of a plant growing
- A sequence showing how light travels through a material
- SPAD sensor data showing photon arrival times

## Why Both Matter

The real power comes from combining both types of information.

### Spatial Images Are Great For

- **Recognizing objects** — "That's a cat" or "That's a car"
- **Understanding structure** — Seeing how parts fit together
- **Detecting patterns** — Finding shapes, textures, or arrangements
- **Navigation** — Knowing where you are and what's around you

### Time-Resolved Images Are Great For

- **Understanding motion** — How fast something is moving, in what direction
- **Detecting changes** — What's different from one moment to the next
- **Material properties** — How light interacts with materials over time
- **Depth sensing** — Using time-of-flight to measure distances

## The Challenge: Why Not Just Use Spatial Images?

Some information simply can't be captured in a single spatial snapshot:

- **Depth information** — A regular photo is flat; you can't tell how far away things are
- **Material properties** — Transparency, reflectivity, and scattering often need temporal data
- **Motion** — A single photo can't show speed
- **Hidden features** — Some properties only reveal themselves over time

## How They Work Together: Spatiotemporal Detection

Modern vision systems combine both approaches. In material classification:

- **Spatial features** might tell you: "This looks like a ceramic bowl"
- **Temporal features** might tell you: "Light reflects off this surface in a specific pattern over time"
- **Together**, they support robust material-aware detection

See the live demonstration on [SPAD for Vision](https://huggingface.co/spaces/mvplus/spad_for_vision) (spatiotemporal detection and material classification demos).

## Real-World Applications

- **Quality control** — Surface defects (spatial) plus material response over time (temporal)
- **Autonomous systems** — Cameras plus time-resolved depth sensors
- **Medical imaging** — Structure plus flow and motion
- **Security** — Identity (spatial) plus behaviour over time (temporal)

## Technology Behind It

**Spatial imaging:** CCD/CMOS cameras, high-resolution sensors, multi-spectral imagers.

**Time-resolved imaging:** SPAD sensors (single-photon timing), time-of-flight sensors, high-speed cameras, picosecond-scale detectors.

## Conclusion

Spatial images tell us *where* things are and *what* they look like. Time-resolved images tell us *when* things happen and *how* they change. The most capable vision systems use both together — as demonstrated in SPAD-based material detection research.
