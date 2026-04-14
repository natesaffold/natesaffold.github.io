---
title: "Ultra-Low-Noise Silicon Imagers: Skipper-CCDs and SiSeROs"
date: 2025-10-21
layout: default
summary: "Developing sub-electron-noise imaging sensors for dark matter and astrophysics experiments."
image: /images/skipperpeaks.png
tags: [Skipper-CCD, SiSeRO, Oscura, SENSEI, DarkNESS]
---

I develop and characterize silicon imaging sensors capable of resolving individual electrons, enabling a new class of low-threshold detectors for dark matter searches and precision astrophysics.

### Skipper-CCDs

**Skipper-CCDs** replace the standard floating-diffusion output stage of a CCD with a floating-gate amplifier that allows the charge packet in each pixel to be sampled non-destructively many times. By averaging N samples, the readout noise is reduced as 1/√N, ultimately reaching sub-electron noise. This single-electron sensitivity enables detection of dark matter particles as light as a few MeV, which would deposit only a few electrons in the detector. Skipper-CCDs form the basis of the **SENSEI** and **Oscura** dark matter experiments and the **DarkNESS CubeSat**.


<figure class="research-figure" style="max-width: 700px; margin: 1.5rem auto;">
  <img src="{{ '/images/skipperpeaks.png' | relative_url }}"
       alt="Charge histogram showing single-electron peaks"
       style="width: 100%; height: auto; display: block;">
  <figcaption style="margin-top: 0.5rem; font-style: italic; text-align: center;">
    Example single-electron charge spectrum from a low-noise silicon imager.
  </figcaption>
</figure>

SENSEI Collaboration (2023), [arXiv:2312.13342](https://arxiv.org/abs/2312.13342)

### SiSeRO-CCDs

**SiSeRO** (Single-electron Sensitive Readout) is a complementary readout architecture that addresses a key limitation of the Skipper-CCD: readout speed. Rather than dumping charge onto a floating gate, the SiSeRO integrates a double-gate n-type MOSFET amplifier directly into the CCD readout line. The CCD p-channel is junction-coupled to the MOSFET's internal gate, so that charge modulates the transistor drain-source current without being transferred or destroyed. This high-sensitivity amplifier design provides non-destructive readout with lower single-sample noise than Skipper-CCDs, enabling sub-electron noise at faster readout speeds.

<figure class="research-figure" style="max-width: 700px; margin: 1.5rem auto;">
  <img src="{{ '/images/sisero.png' | relative_url }}"
       alt="Schematic of SiSeRO readout stage."
       style="width: 100%; height: auto; display: block;">
  <figcaption style="margin-top: 0.5rem; font-style: italic; text-align: center;">
    Schematic of SiSeRO-CCD readout stage.
  </figcaption>
</figure>

Together, Skipper-CCD and SiSeRO technology define a versatile toolkit for ultra-low-noise detection.

*Relevant publications:*  
Sofo-Haro et al. (2023), [arXiv:2310.13644](https://arxiv.org/abs/2310.13644)  
Cuevas-Zepeda, Noonan, Chavez, Sofo-Haro, **Saffold** et al. (2026), [arXiv:2604.02272](https://arxiv.org/abs/2604.02272)
