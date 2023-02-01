# The demo page of InstructTTS
Paper: https://arxiv.org/abs/2301.13662 <br>
Demo: http://dongchaoyang.top/InstructTTS/
### InstructTTS: Modelling Expressive TTS in Discrete Latent Space with Natural Language Style Prompt
## Introduction
For the first time, we study the modelling of expressive TTS with style prompt in natural language, where we meet with the following research problems: (1) how to train a language model that can capture semantic information from the natural language prompt and control the speaking style in the generated speech; (2) how to design an acoustic model to effectively model the challenging one-to-many learning problem of expressive TTS. In this paper, we will address these two challenges.

The main contributions of this study are summarized as follows:  <br>
(1) For the first time, we study the modelling of expressive TTS with natural language prompt, which brings us a step closer to achieve user-controllable expressive TTS. <br>
(2) We introduce a novel three stage training strategy to obtain a robust sentence embedding model, which can effectively capture semantic information from the style prompts. <br>
(3) Inspired by the success of large-scale language models, \textit{e.g.}, GPT3 and ChatGPT \cite{brown2020language}, we propose to model acoustic features in discrete latent space and cast speech synthesis as a language modeling task. Specifically, we train a novel discrete diffusion model to generate vector-quantized (VQ) acoustic feature rather than to predict the commonly-used mel-spectrogram. <br>
(4) We explore to model two types of VQ acoustic feature: mel-spectrogram based VQ features and waveform-based VQ features. We prove that the two types of VQ features can be effectively modeled by our proposed novel discrete diffusion model. We must state that our waveform-based modelling method only needs one-stage training and it is a non-autoregressive model, which is far different from our concurrent work AudioLM \cite{borsos2022audiolm}, VALL-E \cite{wang2023neural} and MusicLM \cite{borsos2023musiclm}. <br>
(5) We jointly apply mutual information (MI) estimation and minimization during acoustic model training to minimize style-speaker and style-content MI, which avoiding possible content and speaker information leakage from the style prompt. <br>
