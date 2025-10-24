# Sparse CNN with Neutrinos

Neutrinos are named after two of their properties. 
1) Neutrinos are **neutral** in charge. Electrons and positrons have negative and positive charges, respectively. However, neutrinos are neutral and therefore do not interact with the electromagnetic force.
2) Neutrinos are very, VERY **small**. At least a million times smaller than electrons!

Where do neutrinos come from?
- The sun is the largest natural source of neutrinos, created during the nuclear fusion reactions in its core.
- 400 billion neutrinos from the sun go through each person on Earth every second!
- Naturally, you might think, what happens when they go through our bodies? __Absolutely nothing!__
<div align="center">
<img width="400" alt="es86_1" src="https://github.com/user-attachments/assets/f3caa0a4-68e2-4508-a882-eeec6911f3f5" />
</div>


Well, if nothing happens, how do we detect them?
- Since neutrinos have no electric charge, it makes it very **difficult** to detect or measure them.
- Not only that, neutrinos go through almost **all matter** without interacting with it! 
- To detect these very _elusive_ particles, we create giant detectors to increase our chances of detecting them. One of which is called the [NOvA](https://novaexperiment.fnal.gov/) experiment.
- NOvA is an 810 km long-baseline neutrino detector experiment spanning from the Near Detector at Fermi National Accelerator Laboratory to the Far Detector at Ash River, MN.
<div align="center">
<img width="400" src="https://github.com/user-attachments/assets/fd8c6541-db21-404e-8fc0-840e4e43ff03" />
</div>

What happens in the detectors?
- With an incoming neutrino, a 'head-on' collision occurs with the nucleus of the atoms in our detectors.
- But, we don't even see the incoming neutrino. Instead, we see the outcome of the 'head-on' collision.
- The interaction between the neutrino and the nucleus produces electrically charged particles such as 
- In the case of a 'head-on' collision with an incoming neutrino and atoms in our detectors, we actually don't even see the incoming neutrino. What we do see is the outcome of the 'head-on' collision. The interaction between the neutrino and the atoms in our detectors produces electrically charged particles such as electrons, muons, or taus. So we look for these charged particles rather than the neutrino itself.
- The interaction between the neutrino and the nucleus produces electrically charged particles such as electrons, muons, or taus. So we detect the charged particles rather than the neutrino itself.
<div align="center">
<img width="400" height="340" alt="argoneut-electron-neutrino-interaction" src="https://github.com/user-attachments/assets/696065a3-db46-463f-8695-76c38aaba9c1" />
</div>

Three "flavors" of neutrinos!
- The three outgoing charged particles, electrons, muons, or taus, are produced with respect to the neutrino flavor.
- For example, with an incoming muon neutrino, a muon and other particles would be produced in the interaction.
<div align="center">
<img width="1000" height="934" alt="Screenshot 2025-10-24 at 11 13 03 AM" src="https://github.com/user-attachments/assets/7d97b2ea-d421-4af7-9a9d-1484befc7a26" />
</div>

How does Machine Learning play in?
- We use machine learning algorithms to identify the particles in ~6 billion Monte Carlo detector images.
- High-energy physics detectors are globally sparse and locally dense. Which means all of our images are mostly 0 pixels. Therefore, we propose an alternative algorithm to the traditional dense neural network called the **Sparse Convolutional Neural Network**.
- The sparse CNN performs convolutions only on the non-zero pixels. This way, we can save time and GPU computational resources during training without sacrificing performance metrics.
- Previous [studies](https://arxiv.org/abs/1903.05663) of sparse CNN have shown to reduce computational cost and wall-time while still improving particle identification accuracy. 

In this GitHub repository...
- Here, a modified Siamese version of the [FishNet](https://github.com/kevin-ssy/FishNet) architecture was developed to ingest two 2D images for the NOvA experiment images.
- Continue onto src/SparseCNN directory for model details!
