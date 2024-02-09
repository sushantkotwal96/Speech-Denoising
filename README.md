# Exploring Speech Denoising

## Overview
Welcome to the Speech Denoising. This project is an exciting exploration into the realm of speech signal processing and deep learning. We aim to tackle the challenge of cleaning up noisy speech recordings, transforming them into crisp, clear audio free from unwanted background noise.

[//]: # ()
[//]: # (## Problem Statement)

[//]: # (The task involves taking a noisy speech spectrum &#40;speech plus chip-eating noise&#41; as input and producing a cleaned-up speech spectrum as output. The project provides datasets consisting of noisy and clean speech recordings for training and evaluation.)

[//]: # (## Technologies Utilized)

[//]: # (- **Python**)

[//]: # (- **TensorFlow** )

[//]: # (- **Librosa** )

[//]: # ()
[//]: # ()
[//]: # ()
[//]: # (## Concepts Explored)

[//]: # (### Short-Time Fourier Transform &#40;STFT&#41;)

[//]: # (STFT comes to our rescue, breaking down the complex signal of speech and chip munching into manageable chunks. This technique allows us to analyze the frequency content of the audio over short, overlapping time windows, giving us the spectrograms we need for denoising.)

[//]: # ()
[//]: # (### Spectrograms)

[//]: # (Spectrograms are the visual representation of the frequency content of a signal over time. Think of them as heat maps for audio, showing us where the energy lies in the signal at different points in time.)

[//]: # ()
[//]: # (### Deep Learning Architectures)

[//]: # (We're diving deep into the world of neural networks, exploring both Fully-Connected Deep Neural Networks and Convolutional Neural Networks &#40;1D and 2D variants&#41; to unravel the mysteries hidden within our noisy recordings.)

[//]: # ()
[//]: # (### Signal-to-Noise Ratio &#40;SNR&#41;)

[//]: # (SNR serves as our guiding light, helping us measure the effectiveness of our denoising efforts. A higher SNR means cleaner, crisper audio and happier listeners.)

[//]: # ()
[//]: # (## Implementation Strategy)

[//]: # (### 1. Fully-Connected Deep Neural Network)

[//]: # (We're building a robust deep neural network with multiple hidden layers to learn the intricate patterns between noisy and clean speech spectra. With careful architecture design and training, we aim to produce impressive denoising results.)

[//]: # ()
[//]: # (### 2. 1D CNN for Speech Denoising)

[//]: # (Embracing the power of convolutional neural networks, we're unleashing a 1D variant to process our spectrograms along the frequency axis. By harnessing the spatial relationships within the spectrograms, we're poised to achieve remarkable denoising capabilities.)

[//]: # ()
[//]: # (### 3. 2D CNN for Enhanced Denoising)

[//]: # (Taking it up a notch, we're exploring the world of 2D CNNs to tackle the denoising challenge from a different angle. By extracting overlapping frames from our spectrograms and leveraging the power of convolution in two dimensions, we're pushing the boundaries of denoising excellence.)

[//]: # ()
[//]: # (## Evaluation and Validation)

[//]: # (We're not just stopping at building models; we're rigorously evaluating their performance. From reconstructing cleaned-up speech signals to calculating SNR values, we're leaving no stone unturned in ensuring the quality and effectiveness of our denoising solutions.)

[//]: # (# Speech Denoising Project README)

[//]: # ()
[//]: # (## Overview)

[//]: # (Welcome to the Speech Denoising Project README! This project focuses on utilizing deep learning techniques to address the challenge of cleaning up noisy speech recordings, ultimately enhancing the clarity and intelligibility of the audio.)

## Problem Statement
The task involves developing algorithms capable of removing unwanted background noise, such as the sound of chip munching, from speech recordings. By leveraging Short-Time Fourier Transform (STFT) and deep learning architectures, we aim to extract clean speech signals from noisy inputs.

## Technologies Utilized
- **Python**
- **TensorFlow**
- **Librosa:** Python package for music and audio analysis. It provides the building blocks necessary to create music information retrieval systems. Here we are using it for audio processing and STFT computation.

## Concepts Explored
### Short-Time Fourier Transform (STFT)
STFT is employed to analyze the frequency content of speech signals over short, overlapping time windows, facilitating the transformation of audio into spectrograms for further processing.

### Spectrograms
Spectrograms are the visual representation of the frequency content of a signal over time. Think of them as heat maps for audio, showing us where the energy lies in the signal at different points in time.

### Deep Learning Architectures
We explore Fully-Connected Deep Neural Networks, 1D Convolutional Neural Networks (CNN), and 2D CNN to learn the mapping between noisy and clean speech spectra, enabling effective denoising.

### Signal-to-Noise Ratio (SNR)
SNR serves as a quantitative metric to evaluate the denoising performance of the models, providing insights into the quality of the reconstructed speech signals.

## Implementation Approach
### 1) Fully-Connected Deep Neural Network
-   Convert noisy and clean speech recordings into spectrograms using STFT.
-   Train a fully-connected deep neural network to predict clean magnitude spectra from noisy input spectra.
-   Utilize appropriate activation functions and initialization schemes.
- Evaluate performance by reconstructing cleaned speech signals and calculating SNR.


### 2) 1D CNN for Speech Denoising
-   Preprocess data by transposing magnitude spectrograms.
-   Implement a 1D CNN architecture to perform convolution operations along the frequency axis.
-   Use appropriate kernel sizes and strides to manage dimensionality.
-   Apply activation functions and optimization techniques.
-   Assess results qualitatively by listening to the denoised signals.

### 3) 2D CNN for Enhanced Denoising
-   Extract image representations from spectrograms with overlapping frames.
-   Design a 2D CNN to process these images and predict cleaned-up spectra.
-   Augment input data to match output dimensionality.
  - Evaluate denoising performance and report results.
## Evaluation and Validation
The performance of the models is evaluated by reconstructing cleaned-up speech signals and calculating SNR values. Additionally, qualitative assessment through listening tests ensures the perceptual quality of the denoised audio.

## Conclusion
In conclusion, the Speech Denoising Project represents a significant endeavor at the intersection of deep learning and signal processing. By leveraging advanced techniques and methodologies, we aim to advance the state-of-the-art in speech denoising, ultimately enhancing the usability and intelligibility of audio recordings in noisy environments.

---

## Limitations
While our models show promising results, it's important to acknowledge their limitations. They may not perform optimally in all scenarios, especially in cases where the noise characteristics are significantly different from our training data.

## Getting Started
To get started with the Speech Denoising Project, follow these steps:
1. Clone the repository: `git clone [repository_url]`
2. Install dependencies: `pip install -r requirements.txt`
3. Explore the Jupyter notebooks and scripts to understand the implementation details.
4. Experiment with different model architectures and parameters to fine-tune performance.

## Acknowledgement
This project would like to thank the developers of TensorFlow, and Librosa for providing the tools and libraries for Deep Learning and Speech Processing that made this project possible.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
