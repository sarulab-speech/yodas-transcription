## Japanese datasets in [YODAS v1](https://huggingface.co/datasets/espnet/yodas)

## Directory
 - asr_text/: ASR (automatic speech recognition)-transcribed text. We used [Whisper-v3](https://huggingface.co/openai/whisper-large-v3).
    - Preprocess: speech enhancement by voicefixer
    - Resegmentation is not performed.
    - Any utterances identified as being other than “ja” were excluded.
 - nisqa/: [NISQA](https://github.com/gabrielmittag/NISQA)-predicted speech-quality scores
    - "mos", "noisiness", "discontinuity", "coloration", "loudness"
 - squim/: [torchaudio-squim](https://pytorch.org/audio/stable/tutorials/squim_tutorial.html)-predicted speech-quality scores
    - "stoi", "pesq", "si_sdr"

## Data statistics
Since we excluded other-language utterances, the data size is different from the official data size.

|         | # of samples | Sum. (h) | Ave. (s) | Max. (s) | Min. (s) |
|---------|---------|--------|------|-------|------|
| ja000_ja | 620709 | 821.6 | 4.8 | 30.0 | 0.1 |
| ja100_ja | 1895361 | 1914.8 | 3.64 | 30.0 | 0.1 |

## Contributors
- [Ryotaro Nagase / 永瀬 亮太郎](https://sites.google.com/view/ryotaronagase/home)
