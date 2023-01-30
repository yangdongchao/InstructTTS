# <center> NoreSpeech </center>

<center> Dongchao Yang<sup>1</sup>, Songxiang Liu<sup>2</sup>, Jianwei Yu<sup>2</sup>, Helin Wang<sup>3</sup>, Chao Weng<sup>2</sup>, Yuexian Zou<sup>1</sup></center> 
 
<center> 1 Peking University </center>
<center> 2 Tencent AI Lab</center>
<center> 3 Johns Hopkins University</center>

## Introduction
This is a [demo](http://dongchaoyang.top/NoreSpeech_demo//) for our paper **_Learning to speak by learning to generate: deep style features generation by diffusion model for noisy-robust expressive TTS_**. Code and Pre-trained model can be found on [github](https://github.com/yangdongchao/NoreSpeech). In the following, we will show some generated samples by our proposed method. If you want to find more samples, please refer to our [github](https://github.com/yangdongchao/NoreSpeech).

## The comprarison between generated sample by other SOTA models and our NoreSpeech

#### # Reference/Target Text: we must tread softly and talk low as we go through the land of the jolliginki

| <center>Reference (clean)</center> | <center>Reference (noisy)</center> | <center>FS2 (nosiy) </center> | <center>Styler </center> | <center>GenerSpeech (clean) </center> | <center>GenerSpeech (noisy) </center>| <center>GenerSpeech (denoise) </center> | <center> NoreSpeech </center>|
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
|<audio src="sample4/101_126859_000006_000000_ref_clean.wav" controls preload></audio> | <audio src="sample4/101_126859_000006_000000_ref_noise.wav" controls preload></audio> | <audio src="sample4/101_126859_000006_000000_fs2.wav" controls preload></audio> | <audio src="sample4/101_126859_000006_000000_styler.wav" controls preload></audio> |<audio src="sample4/101_126859_000006_000000_gener_clean.wav" controls preload></audio> | <audio src="sample4/101_126859_000006_000000_gener_noise.wav" controls preload></audio> | <audio src="sample4/101_126859_000006_000000_gener_denoise.wav" controls preload></audio> | <audio src="sample4/101_126859_000006_000000_nore.wav" controls preload></audio> |

##### Reference/Target Text: a king has a great opportunity to make himself loved .

| <center>Reference (clean)</center> | <center>Reference (noisy)</center> | <center>FS2 (nosiy) </center> | <center>Styler </center> |<center>GenerSpeech (clean) </center> | <center>GenerSpeech (noisy) </center>| <center>GenerSpeech (denoise) </center> | <center> NoreSpeech </center>|
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
|<audio src="sample1/1025_75365_000002_000002_ref_clean.wav" controls preload></audio> | <audio src="sample1/1025_75365_000002_000002_ref_noise.wav" controls preload></audio> | <audio src="sample1/1025_75365_000002_000002_FS2.wav" controls preload></audio> | <audio src="sample1/1025_75365_000002_000002_styler.wav" controls preload></audio> | <audio src="sample1/1025_75365_000002_000002_gener_clean.wav" controls preload></audio> | <audio src="sample1/1025_75365_000002_000002_gener_noise.wav" controls preload></audio> | <audio src="sample1/1025_75365_000002_000002_gener_denoise.wav" controls preload></audio> | <audio src="sample1/1025_75365_000002_000002_nore.wav" controls preload></audio> |

##### Reference/Target Text: maybe they were out of boys of the brand you wanted 

| <center>Reference (clean)</center> | <center>Reference (noisy)</center> | <center>FS2 (nosiy) </center> | <center>Styler </center> | <center>GenerSpeech (clean) </center> | <center>GenerSpeech (noisy) </center>| <center>GenerSpeech (denoise) </center> | <center> NoreSpeech </center>|
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
|<audio src="sample2/103_1241_000012_000002_ref_clean.wav" controls preload></audio> | <audio src="sample2/103_1241_000012_000002_ref_noisy.wav" controls preload></audio> | <audio src="sample2/103_1241_000012_000002_fs2.wav" controls preload></audio> | <audio src="sample2/103_1241_000012_000002_styler.wav" controls preload></audio> | <audio src="sample2/103_1241_000012_000002_gener_clean.wav" controls preload></audio> | <audio src="sample2/103_1241_000012_000002_gener_noise.wav" controls preload></audio> | <audio src="sample2/103_1241_000012_000002_gner_denoise.wav" controls preload></audio> | <audio src="sample2/103_1241_000012_000002_nore.wav" controls preload></audio> |

##### Reference/Target Text: the rock was not much larger than their great bed , but of course they all knew how not to take up much room , and they were dozing , or at least lying with their eyes shut , and pinching occasionally when they thought wendy was not looking

| <center>Reference (clean)</center> | <center>Reference (noisy)</center> | <center>FS2 (nosiy) </center> | <center>Styler </center> | <center>GenerSpeech (clean) </center> | <center>GenerSpeech (noisy) </center>| <center>GenerSpeech (denoise) </center> | <center> NoreSpeech </center>|
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
|<audio src="sample3/1012_133424_000008_000001_ref_clean.wav" controls preload></audio> | <audio src="sample3/1012_133424_000008_000001_ref_noise.wav" controls preload></audio> | <audio src="sample3/1012_133424_000008_000001_fs2.wav" controls preload></audio> | <audio src="sample3/1012_133424_000008_000001_styler.wav" controls preload></audio> | <audio src="sample3/1012_133424_000008_000001_gener_clean.wav" controls preload></audio> | <audio src="sample3/1012_133424_000008_000001_gener_noise.wav" controls preload></audio> | <audio src="sample3/1012_133424_000008_000001_gener_denoise.wav" controls preload></audio> | <audio src="sample3/1012_133424_000008_000001_nore.wav" controls preload></audio> |

### Non-Parallel Transfer
In non-parallel style transfer, the TTS system must transfer prosodic style when the source and target text are completely different. 

##### (1) Reference Text: when it was all done he put it on the table beside me , and at first i did nt know whether i was the live rabbit or the toy rabbit , we were so much alike 

| Reference audio |
| -----------     |
| <audio src="non_pa/sample1/100_121674_000026_000003.wav" controls preload></audio> |

##### Target Text: well , his grill has a plating of gold , and his twistings are greatly admired

| <center> Styler </center> | <center> GenerSpeech </center> | <center> NoreSpeech </center>|
| -----------     |  -----------     |
| <audio src="non_pa/sample1/100_121674_000026_000003[Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample1/[000001][100_121674_000026_000003][Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample1/[000001][100_121674_000026_000003][Generalize]Y.wav" controls preload></audio> |

##### (2) Reference Text: chapter eight the mermaids lagoon

| Reference audio |
| -----------     |
| <audio src="non_pa/sample2/1012_133424_000001_000000.wav" controls preload></audio> |

##### Target Text: to be more accurate , i should have said to the northeast

|  <center> Styler </center> | <center> GenerSpeech </center> | <center> NoreSpeech </center>|
| -----------     |  -----------     |
| <audio src="non_pa/sample2/1012_133424_000001_000000[Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample2/[000005][1012_133424_000001_000000][Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample2/[000005][1012_133424_000001_000000][Generalize]Y.wav" controls preload></audio> |

##### (3) Reference Text: some of the reverend frank milveys brethren had found themselves exceedingly uncomfortable in their minds , because they were required to bury the dead too hopefully 

| Reference audio |
| -----------     |
| <audio src="non_pa/sample3/1027_125140_000008_000000.wav" controls preload></audio> |

##### Target Text: but there was a passenger dropped off for you a little girl

| <center> Styler </center> | <center> GenerSpeech </center> | <center> NoreSpeech </center>|
| -----------     |  -----------     |
| <audio src="non_pa/sample3/1027_125140_000008_000000[Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample3/[000027][1027_125140_000008_000000][Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample3/[000027][1027_125140_000008_000000][Generalize]Y.wav" controls preload></audio> |

##### (4) Reference Text: baron conrad and his men at arms sat foot in stirrup , the milk white horse that had been brought for otto stood waiting for him beside his fathers great charger. 

| Reference audio |
| -----------     |
| <audio src="non_pa/sample4/1028_133393_000002_000001.wav" controls preload></audio> |

##### Target Text: she would invoke the past , recall old recollections ; she would supplicate him by the remembrance of guilty , yet happy days.

| <center> Styler </center> |<center> GenerSpeech </center> | <center> NoreSpeech </center>|
| -----------     |  -----------     |
| <audio src="non_pa/sample4/1028_133393_000002_000001[Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample4/[000031][1028_133393_000002_000001][Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample4/[000031][1028_133393_000002_000001][Generalize]Y.wav" controls preload></audio> |

##### (5) Reference Text: the morrow brought a very sober looking morning , the sun making only a few efforts to appear , and catherine augured from it everything most favourable to her wishes 

| Reference audio |
| -----------     |
| <audio src="non_pa/sample5/14_208_000001_000000.wav" controls preload></audio> |

##### Target Text: the store is on a corner about which coveys of ragged plumed , hilarious children play and become candidates for the cough drops and soothing syrups that wait for them inside.

| <center> Styler </center> | <center> GenerSpeech </center> | <center> NoreSpeech </center>|
| -----------     |  -----------     |
| <audio src="non_pa/sample5/14_208_000001_000000[Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample5/[000045][14_208_000001_000000][Generalize]X.wav" controls preload></audio> | <audio src="non_pa/sample5/[000045][14_208_000001_000000][Generalize]Y.wav" controls preload></audio> |

## Links

[[Paper]()] [[Bibtex]()] [[Demo GitHub](https://github.com/yangdongchao/NoreSpeech_demo)] [[TencentAILab](https://ai.tencent.com/ailab/zh/index)] [[PKU](https://www.pku.edu.cn/)] [[code](https://github.com/yangdongchao/NoreSpeech)]

