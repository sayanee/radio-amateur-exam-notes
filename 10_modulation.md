# 10. Modulation

## Definitions

- In **Frequency Modulation**, the speech causes the frequency of the carrier to go up and down
- **Narrow Band Frequency Modulation (NBFM)** means the bandwidth of an transmission must be no more than the `6kHz` permitted on AM
- The **amplitude of the modulating frequency** controls the amount that the carrier swings up and down (deviates) from nominal.
- The **frequency of the modulating frequency** controls the rate at which the carrier swings up and down from nominal.
- **Capture effect**, or **FM capture effect**, is a phenomenon associated with FM reception in which only the stronger of two signals at, or near, the same frequency or channel will be demodulated
- **CW** is "Carrier Wave" and sometime for "Continuous Wave"
- **BFO** Beat Frequency Oscillator
- **Splatter interference** is caused by over-modulation of a transmitter
- **Spurious emission** is any radio frequency not deliberately created or transmitted, especially in a device which normally does create other frequencies. 

## Diagrams

- AM and FM

  ![](img/am-fm.gif)

## Circuit diagrams

## Formula

- Lower sideband = `Fc - Fm` where `Fc` is the carrier frequency, `Fm` is the modulating frequency
- Upper sideband = `Fc + Fm` where `Fc` is the carrier frequency, `Fm` is the modulating frequency
- `Modulation index = Deviation from carrier centre frequency / Audio frequency producing this deviation`
- `Deviation Ratio = Maximum Deviation of the Carrier / Maximum modulating frequency`

## Graphs

## Notes

### Over modulation

- Avoid over modulation
- distort the amplitude modulated signal and cause undue bandwidth and interference
- results in spurious emissions by the modulated carrier, and distortion of the recovered modulating signal
- If over-modulation does occur the carrier is chopped up and the modulation no longer resembles its modulating signal
- will have an increased bandwidth
- will be rich in unwanted harmonics

Prevent over-modulation:

- an indication is given when the depth of modulation exceeds, say, 80%
  - monitoring the output with an oscilloscope or by a modulation meter
  - a lamp or LED lights when a predetermined level is exceeded
- By automatic means, whereby the modulating signal is prevented from exceeding an amplitude that would result in over-modulation

### Problems with AM

- Large audio amplifiers and high power modulators are required
- not an efficient method of communication as the "speech content" of the total signal is small
- the speech power is split between the upper and lower sidebands
- possible to do away with the carrier and one of the sidebands - Single Side Band (SSB)
  - all the permitted power is concentrated into one speech side band

### Frequency modulators

- Most important component is the variable capacitor diode:
  - connected across the tuned circuit of an oscillator
  - reverse biased to a linear part of the Volts/Capacitance curve
  - A conducting diode would damp the tuned circuit and may stop the oscillator

### Interference in AM / FM

- unwanted spikes of interference modulating the amplitude of the carrier
- the clipper can remove all of the unwanted amplitude modulation and leave the carrier intact
- changing frequency of the carrier contains all the necessary information to give an undistorted
interference free audio output

### Weak FM

- an FM signal has to be reasonably strong to attain the advantage of "interference free reception"
- a very weak FM signal, will sound much noisier than an AM signal of the same strength

*An FM signal, having **constant amplitude**, is less likely to cause Interference to nearby television and radio receivers.*

### Morse transmission

- Simple transmitters for `A1A`:
  - When the Morse key is pressed `down` a carrier (a single frequency) is `transmitted`
  - When the Morse key is `released` then the carrier is switched off and `nothing` is transmitted
  - This signal requires a receiver with a BFO (Beat Frequency Oscillator) to receive it
- Complex transmitters for `SSB`:
  - send a carrier continuously but connect the Morse Key to an audio oscillator
  - When the Morse Key is `pressed` the carrier is Amplitude modulated with this audio tone
  - When the key is `released` the tone is switched off but the carrier wave continues
- `A2A`
  - leave the audio tone modulating the carrier all the time
  - switch the whole modulated signal on and off using the Morse Key
  - Where a tone is added (often referred to as a "sub carrier") then this is given the code A2A
  - an A2A transmission uses a modulating signal which is keyed by a tone or sub-carrier resulting in a double side band amplitude modulated signal
  - can be received with an ordinary receiver, with out the need for a BFO
