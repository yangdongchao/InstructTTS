# <center> InstructTTS </center>

<center> Dongchao Yang*<sup>1</sup>, Songxiang Liu*<sup>2</sup>, Rongjie Huang <sup>3</sup>, Guangzhi Lei<sup>2</sup>, Chao Weng<sup>2</sup>, Helen Meng<sup>1</sup>, Dong Yu<sup>2</sup></center> 
 
<center> 1 Chinese University of Hong Kong </center>
<center> 2 Tencent AI Lab</center>
<center> 3 Zhejiang University</center>

## Abstract
Expressive text-to-speech (TTS) aims to synthesize different speaking style speech according to human's demands. Nowadays, there are two common ways to control speaking styles: (1) Pre-defining a group of speaking style and using categorical index to denote different speaking style. However, there are limitations in the diversity of expressiveness, as these models can only generate the pre-defined styles. (2) Using reference speech as style input, which results in a problem that the extracted style information is not intuitive or interpretable.
In this study, we attempt to use natural language as style prompt to control the styles in the synthetic speech, e.g., ''Sigh tone in full of sad mood with some helpless feelin''.
Considering that there is no existing TTS corpus which is proper to benchmark this novel task, we first construct a speech corpus, whose speech samples are annotated with not only content transcriptions but also style descriptions in natural language.
Then we propose an expressive TTS model, named as InstructTTS, which is novel in the sense of following aspects:
(1) We fully take the advantage of self-supervised learning and cross-modal metric learning, and propose a novel three-stage training procedure to obtain a robust sentence embedding model, which can effectively capture semantic information from the style prompts and control the speaking style in the generated speech.
(2) We propose to model acoustic features in discrete latent space and train a novel discrete diffusion probabilistic model to generate vector-quantized (VQ) acoustic tokens rather than the commonly-used mel spectrogram. 
(3) We jointly apply mutual information (MI) estimation and minimization during acoustic model training to minimize style-speaker and style-content MI, avoiding possible content and speaker information leakage from the style prompt.
Extensive objective and subjective evaluation has been conducted to verify the effectiveness and expressiveness of InstructTTS. Experimental results show that InstructTTS can synthesize high-fidelity and natural speech with style prompts controlling the speaking style.

## Introduction
This is a [demo](http://dongchaoyang.top/InstructTTS//) for our paper **_InstructTTS: Modelling Expressive TTS in Discrete Latent Space with Natural Language Style Prompt_**. In the following, we will show some generated samples by our proposed method. More Generated speech, please refer to https://github.com/yangdongchao/InstructTTS/tree/gh-pages


## Some Synthesized speech by InstructTTS.

| <center> Style prompt </center> | <center> Content Prompt </center> | <center> Generated Speech </center>|
| -----------     |  -----------     |
| 语调中带着嫌弃不满的情绪，彰显出说话着极度抱怨的情感 | 不用别人点她自己就炸了，你说你也是的，干吗要介绍一个这么花花公子的人给小萍啊？ | <audio src="InstructTTS_mel/tx_emulate_00_102_0003_000034.wav" controls preload></audio> |
| 语气中带着一点不自信，感觉不是很肯定的样子 | 也算情人吧。 | <audio src="InstructTTS_mel/tx_emulate_00_103_0001_000037.wav" controls preload></audio> |
| 语速较慢，一字一顿的感觉，语气非常得意 | 专家把我的也统计进去了，所以平均每个人多交了一个男朋友 | <audio src="InstructTTS_mel/tx_emulate_00_114_0002_000002.wav" controls preload></audio> |
| 很惊讶一件事情 | 天呐，跟着他快5年啦 | <audio src="InstructTTS_mel/tx_emotion_00309000228.wav" controls preload></audio> |
| 高声反问之中，表达了内心的谴责不满和激越愤懑之情，亦夹杂着明显的鄙夷和不齿之意。| 你甭身在曹营心在汉的，一天到晚想什么呢。 | <audio src="InstructTTS_mel/tx_emulate_02_242_0002_000071.wav" controls preload></audio> |
| 表明内心十分强烈坚决的意愿，流露出内心的冷漠和决绝 | 值得不值得是我自己事，你还是走吧。 | <audio src="InstructTTS_mel/tx_xiao_0100105000370.wav" controls preload></audio> |
| 话语带有一种诧异的心情，还有一点质疑的态度，夹杂着不满 | 她你也要请啊。 | <audio src="InstructTTS_mel/tx_emulate_02_255_0001_000067.wav" controls preload></audio> |
| 语气有些许不耐烦的感觉，说话仍然温和，只是有些疑惑 | 哎，阿良，你有没有听我说话，让我出去，你到底在干什么。 | <audio src="InstructTTS_mel/tx_xiao_0200106000561.wav" controls preload></audio> |
| 语调冷淡急促，内心充满鄙视和嘲讽 | 一群土老帽儿，说你们也不懂。 | <audio src="InstructTTS_mel/tx_emulate_02_256_0006_000059.wav" controls preload></audio> |
| 言语和语气都是嫌弃 | 切~~，有本事我们来个2对2的对决呀。 | <audio src="InstructTTS_mel/tx_emotion_00304000102.wav" controls preload></audio> |

## Links

[[Paper]()] [[Bibtex]()] [[Demo GitHub](http://dongchaoyang.top/PromptLM-TTS)] [[TencentAILab](https://ai.tencent.com/ailab/zh/index)] [[CUHK]()] [[code]()]

