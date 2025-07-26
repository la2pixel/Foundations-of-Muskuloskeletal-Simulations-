# Processing surface EMG signals
Other helpful resources : [(1)](https://github.com/emckiernan/electrophys/blob/master/EMG/README-EMG.md) , [(2)](https://www.biopac.com/wp-content/uploads/EMG-Guide.pdf), [(3)](https://www.researchgate.net/figure/EMG-signal-process-recommended-Green-The-raw-signal-no-treatment-was-applied-until_fig2_258344784)

## Physiology Behind the signal
> This section is for people with minimal biology background who want to understand what EMG measures, and how it relates to your intention to move translating into muscle activity. We do not dive deep into all aspects of this topic, but just enough to understand EMG signal processing.

##### Brain initiates the command
- Every voluntary movement starts with intention: "I want to take a step". This decision originates in the *motor cortex*, a part of the brain responsible for planning and controlling voluntary movements.
- So once the brain has formed this movement plan, it sends instructions through the Central Nervous System (CNS):
    - Motor cortex encodes the command and passes a signal via motor neurons, which are deisgned to control motor units (= group of muscle fibers)
    - Signal travels down the spinal cord via upper motor neurons, which is then passed down to lower (or alpha) motor neurons that carry the signal from spinal cord to muscle fibers of the intended part of your body.

##### What are these signals?
- The electrical signals we just talked about, are called *action potential*, which is like a wave of electrical charge that travels down neuron's length (i.e., the axon). It helps to remember this term as "potential to move/act" for this particular usecase.
- It is very fast : ~1-2 milliseconds per spike, and can travel upto ~100m/s !
- Just imagine how much of this our body is doing while we type, talk (hand gestures) etc.
- Action potential is an "all (1) or nothing (0) event" that carries the signal:
    - A neuron at rest maintains a voltage difference of about 70mV, called resting potential.
    - When the neuron fires, sodium (Na+) ions rush in, briefly making the inside more positive
    - This event triggers a chain reaction which helps us identify the spikes.

#### Signals reach the muscle
- Once action potential reaches the end of motor neuron, it causes neuron to release *acetylcholine (ACh)*, which is a chemical signal.
- ACh crosses the gap (= synapse) and binds to receptors on the muscle fiber membrane, triggering a new action potential here.
- This event marks the transition from electrical signaling in the nervous system to electrical excitation of mucle tissues.

#### Muscle Fiber Excitation and Contraction
- Once the action potential propogates along the muscle membrane, it travels through the sarcolemma (= muscle cell membrane) and into the T-tubules, responsible for muscle contraction.
- This stimulates release of calcium ions (Ca+) inside the muscle and this is what causes contraction.

This is the electrical acivity that surfacr EMG electrodes detect and record!

> EMG doesn't record the movement itself, as explained above. They measure the electrical noise that muscles produce when they're activated (= sum of all action potentials under the skin).
> EMG ≈ electrical fingerprints of muscle activation, not force or intent.

