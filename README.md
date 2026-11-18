# French Speech Dataset

Free sample recordings from Spirelight's off-the-shelf French speech dataset. 1,131 hours of unscripted French recorded in January and February 2026, mostly by speakers in Algeria, Madagascar, Morocco, Rwanda and Benin: 1,012 hours of two-person conversation, each speaker on their own channel, and 118 hours of single-speaker recordings, with machine transcripts and word-level timestamps. Download access within 24 hours of a signed order.

**Full dataset, pricing and quotes:** [spirelight.ai/datasets/french-france](https://www.spirelight.ai/datasets/french-france?src=github-french-france)

## Listen

Short excerpts, as played on the dataset page, are in [`excerpts/`](excerpts/):

- [`excerpts/french-conversation-excerpt.mp3`](excerpts/french-conversation-excerpt.mp3)
- [`excerpts/french-monologue-excerpt.mp3`](excerpts/french-monologue-excerpt.mp3)

The complete sample recordings (FLAC, with transcripts and a `datasets` loader) are on Hugging Face: [huggingface.co/datasets/SpeechDataAI/french-speech-dataset](https://huggingface.co/datasets/SpeechDataAI/french-speech-dataset). Their uncorrected machine transcripts, as TXT and JSON with word-level timestamps, are also in [`transcripts/`](transcripts/) here.

## Full sample recordings (on Hugging Face)

3 complete recordings, 78 minutes in total. The audio is unedited and compressed losslessly to FLAC on Hugging Face; buyers receive WAV plus one file per speaker for conversations. Each recording has its uncorrected machine transcript as TXT and JSON.

| File | Type | Length | Audio |
| --- | --- | --- | --- |
| [`conversation/french-conversation-01.flac`](https://huggingface.co/datasets/SpeechDataAI/french-speech-dataset/blob/main/conversation/french-conversation-01.flac) | Conversation | 31 min | 48 kHz, 16-bit, stereo |
| [`monologue/french-monologue-01.flac`](https://huggingface.co/datasets/SpeechDataAI/french-speech-dataset/blob/main/monologue/french-monologue-01.flac) | Monologue | 21 min | 48 kHz, 24-bit, mono |
| [`monologue/french-monologue-02.flac`](https://huggingface.co/datasets/SpeechDataAI/french-speech-dataset/blob/main/monologue/french-monologue-02.flac) | Monologue | 25 min | 48 kHz, 24-bit, mono |

On Hugging Face, each audio folder has a `metadata.csv` with the full transcript text, so the dataset viewer and `datasets` can read it directly. Word-level timestamps are in the JSON files under `transcripts/`.

```python
from datasets import load_dataset

ds = load_dataset("SpeechDataAI/french-speech-dataset", "conversation", split="train")
print(ds[0]["text"][:300])
```

## The full dataset

| Recording type | Recordings | Hours | Average length |
| --- | ---: | ---: | ---: |
| Conversation, business topics | 919 | 505.9 | 33 min |
| Conversation, open topics | 936 | 506.4 | 32 min |
| Monologue | 221 | 109.4 | 30 min |
| Single speaker, type not labelled | 12 | 8.9 | 44 min |

Recordings from France make up 27 hours. If you need speakers from France, Belgium, Switzerland or Canada, we can record them to order.

| Speaker location | Hours |
| --- | ---: |
| Algeria | 487 |
| Madagascar | 202 |
| Morocco | 139 |
| Rwanda | 105 |
| Benin | 95 |
| France | 27 |
| Côte d'Ivoire | 25 |
| Senegal | 13 |
| Burundi | 12 |
| Other or not stated | 26 |

Speakers' home regions include Antananarivo, Algiers, Béjaïa, Batna and Casablanca.

- **Speakers:** 82 registered contributors, 27 of whom recorded monologues. Their conversation partners were not registered, so there are more than 82 distinct voices; that number is not counted.
- **Recorded:** 2026-01-24 to 2026-02-26
- **Audio:** 48 kHz WAV. Conversations: stereo, one speaker per channel, plus one file per speaker. Single-speaker recordings: mono. Bit depth is 16 or 24 depending on the recording.
- **Devices and setting:** 96% recorded on a laptop or PC and about 4% on a phone, in quiet indoor settings.
- **Transcripts:** Machine transcripts with speaker labels, segment start and end times and word-level timestamps, as TXT and JSON, for 1,129 of the 1,131 hours. Not human-reviewed.
- **Topics:** More than 1,700 distinct topic labels, from business meetings, interviews and sales to football, music, religion and daily life.
- **Licence:** commercial use under a written licence; voice cloning is excluded.
- **Price:** $35 per audio hour for all 1,131 hours ($39,585); a part of the dataset is quoted.
- **Delivery:** download access within 24 hours of a signed order.

## Good for

- Training and evaluating French ASR (speech recognition) on unscripted speech rather than read sentences.
- Speaker diarization: in the conversations each speaker has their own channel, so turns and overlaps can be read from the channels.
- Voice agents and turn-taking research: real interruptions, backchannels and topic changes.

Not for voice cloning or imitating a speaker.

## How the samples differ from free corpora

Common Voice and FLEURS are short sentences read aloud, and MLS is audiobooks read aloud. These recordings are unscripted conversation and monologue, 32 minutes per recording on average.

## Licence for this sample

The files in this repository are free to download and use to evaluate whether the full dataset fits your project. Training on them, redistributing them and voice cloning are not permitted. See [LICENSE.md](LICENSE.md). The full dataset is licensed commercially: [request a quote or the full sample pack](https://www.spirelight.ai/datasets/french-france?src=github-french-france#request-samples).

## About

Published by SpeechData.ai, part of Spirelight (Spire Light ApS, Denmark), which records, transcribes and licenses speech data for teams building voice AI. Browse every dataset at [spirelight.ai/datasets](https://www.spirelight.ai/datasets?src=github-french-france).
