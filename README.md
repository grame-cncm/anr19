# ANR Project 2019

## Notes on the call for projects

### Potential Categories

* 4.2 - Culture, création, patrimoine (prioritaire)
* 5.1 - Fondement du numérique : informatique, automatique, traitement du signal
* 8.6 - Révolution numérique : rapports au savoir et à la culture

## Thoughts on project

### Problems we're trying to address

* **Computational power/efficiency:** FPGAs should allow us to carry out more computation than traditional platforms for specific kind of DSP algorithms.
* **Low Latency:** FPGAs can process audio samples much faster than traditional platforms and have the potential and can help reduce audio latency.

### Examples of applications/fiels that would benefit directly from this type of research

#### Low latency synthesizers/audio effects

That's probably the most obvious application from our perspective. Audio latency is directly linked to the "reactivity" of digital musical instruments. Most acoustic musical instruments can produce sound instantaneously which is not the case of digital instruments. Musicians on stage need to have the lowest latency when using audio effects (i.e., guitar pedals, etc.) and sound synthesizer to be able to perform fast and expressively. FPGA-based synthesizer modules and effect processors could help to significantly decrease the latency of this type of systems.

#### Noise cancellation / active acoustic control

Active acoustic control is a developing field where the main idea is to actively modify the acoustical properties of a space using speakers and microphones. That space can be anything from a small box (e.g., passenger compartment in a car, etc.) to a large room (e.g., concert hall, etc.). The types of acoustic modifications can range from noise cancellation (i.e., to dampen the acoustics of the space) to the application the acoustical properties of another room. For example, one might want to suppress the sound of the engine or of the road in a car, dampen the sound of people talking in a loud restaurant, or on the contrary apply the acoustics of a church in a concert hall, etc. In order to do this, the system must be able to address a large number of microphones and speakers and to carry out computation extremely fast to "beat" the acoustical wavefront before it reaches the ears of people in the space. In other words, these systems should have a very low latency and should be highly parallelizable, that's where FPGAs come to play...

Still on the same topic, the "standard way" to apply the acoustics of a room onto another is by using convolution and impulse responses, etc. The problem of using convolution is that it makes the system completely static and impossible to change in real-time. Another approach consists in using a bank of IIR filters in parallel, each implementing a mode of resonance of the room to model. It allows for a high level of parametrization of the system and to "morph" between different room models for example. On the other hand, it is very computationally expensive. Since this type of algorithm is highly parallelizable (i.e., filters in parallel), it could greatly benefit from being implemented on an FPGA. 

Obviously, Stanford could be an excellent partner for such a project, but it's not necessarily simple in the framework of an ANR project.

#### Active control of musical instruments

The idea here is very close to the previous one but applied to musical instruments. The goal is to interact with the acoustical waves of the instrument to change its sound, etc. This can be useful to make hybrid musical instruments (partly virtual and partly physical), to make more "universal" instruments (i.e., an acoustic guitar that can sound like any acoustic guitar of any luthier and manufacturer, etc.) or to make mutes (i.e., a saxophone mute still allowing to hear the sound of the saxophone but in headphones: nice for practice and for neighbors, etc.).

#### Real-time high-fidelity physical modeling of musical instruments

High fidelity physical models of musical instruments are now being increasingly used on stage. However, they require a tremendous amount of computation out of reach to most personal computers or standard computing platforms for audio (i.e., DSPs, etc.). Algorithms used for physical modeling can be easily parallelized and could therefore benefit from FPGAs. 

