####BB84 Protocol:
In the first phase, Alice will communicate to Bob over a quantum channel.
Alice begins by choosing a random string of bits and for each bit, Alice will randomly choose a
basis, rectilinear or diagonal, by which to encode the bit. She will transmit a photon for each bit
with the corresponding polarization, as just described, to Bob.
For every photon Bob receives, he will measure the photon’s polarization by a randomly chosen
basis. If, for a particular photon, Bob chose the same basis as Alice, then in principle, Bob should
measure the same polarization and thus he can correctly infer the bit that Alice intended to send.
If he chose the wrong basis, his result, and thus the bit he reads, will be random.
In the second phase, Bob will notify Alice over any insecure channel what basis he used to
measure each photon. Alice will report back to Bob whether he chose the correct basis for each
photon. At this point Alice and Bob will discard the bits corresponding to the photons which Bob
measured with a different basis.
Provided no errors occurred or no one manipulated the photons, Bob and Alice should now both
have an identical string of bits which is called a sifted key.
The example above shows the bits Alice chose, the bases she encoded them in, the bases Bob
used for measurement, and the resulting sifted key after Bob and Alice discarded their bits as just
mentioned.








Alice and Bob agree upon a random subset of the bits to compare to ensure consistency. If the bits
agree, they are discarded and the remaining bits form the shared secret key. In the absence of noise
or any other measurement error, a disagreement in any of the bits compared would indicate the
presence of an eavesdropper on the quantum channel. This is because the eavesdropper, Eve, were
attempting to determine the key, she would have no choice but to measure the photons sent by Alice
before sending them on to Bob. This is true because the no cloning theorem assures that she cannot
replicate a particle of unknown state. Since Eve will not know what bases Alice used to encoded
the bit until after Alice and Bob discuss their measurements, Eve will be forced to guess. If she
measures on the incorrect bases, the Heisenberg Uncertainty Principle ensures that the information
encoded on the other bases is now lost. Thus when the photon reaches Bob, his measurement will
now be random and he will read a bit incorrectly 50 percentage of the time. Given that Eve will
choose the measurement basis incorrectly on average 50 percentage of the time, 25 percentage of
Bob’s measured bits will differ from Alice . If Eve has eavesdropped on all the bits then after n bit
comparisons by Alice and Bob, they will reduce the probability that Eve will go undetected to ¾n.
The chance that an eavesdropper learned the secret is thus negligible if a sufficiently long sequence
of the bits are compared.

