# Amplitude Envelope

**Amplitude envelope** refers to the changes in the amplitude of a sound over time. It is a highly influential property because it significantly affects our **perception of timbre**.

This is one of the most important properties of sound — it is what allows us to effortlessly **identify** and **uniquely distinguish** different sounds from one another.

## How the Amplitude Envelope is Computed

The amplitude envelope of an audio file is computed using the concept of **framing**:

1. The audio signal is divided into a number of small time frames.
2. For each frame, a single amplitude value is calculated based on an **aggregation feature** (most commonly the **maximum** value within the frame).
3. This process is repeated for every frame across the entire audio signal.

The result is a time series that roughly represents the **loudness contour** or **amplitude contour** of the sound.

![Amplitude Envelope Example](figure1)  
*(Figure 1: Example of an amplitude envelope extracted from an audio signal)*

## Summary Definition

The **amplitude envelope** is a **time-domain audio feature** extracted from the raw audio waveform.  
It describes **fluctuations in amplitude over time** and is essential because it strongly influences our auditory perception of **timbre**.

It enables us to **quickly detect and distinguish** different sounds.  
The envelope is typically formed by taking the **maximum amplitude value** among all samples in each frame — providing a rough estimation of **loudness**.

## Applications

This feature has been widely used in:

- **Onset detection**
- **Music genre classification**

## Comparison with RMS Energy

Although very useful, the **maximum-based amplitude envelope** is **more sensitive to outliers** (sudden spikes/clicks/noise) than the **RMS (Root Mean Square) energy** feature.  
→ For this reason, **RMS energy** is often preferred in many audio analysis tasks.

![Flowchart](flowchart)  
*(Flowchart: Process of computing the amplitude envelope from raw audio)*

## Two Main Types of Amplitude Envelopes

### 1. Percussive Envelopes
- Characterized by:
  - **Abrupt onset** (very fast attack)
  - **Immediate exponential decay**
- Typical of **impact/attack-based sounds**:
  - Two wine glasses clinking
  - Hitting a drum
  - Slamming a door
  - Plucking a string, etc.

### 2. Flat Envelopes
- Characterized by:
  - **Abrupt onset**
  - **Indefinite / relatively long sustain** period
  - **Abrupt offset** (sudden end)
- Common in sounds with steady-state portions (e.g. sustained notes on wind instruments, bowed strings, organ tones, etc.)

![Amplitude Envelope Types](figure2)  
*(Figure 2: Comparison of percussive vs. flat amplitude envelopes)*