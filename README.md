# VirgoolInformal-Speech-Dataset

This repository contains a dataset of informal Persian audio and text chunks suitable for Automatic Speech Recognition (ASR) and Text-to-Speech (TTS) tasks. The dataset was created by crawling informal Persian text from [virgool.io](https://virgool.io) using the crawling scripts from [this repository](https://github.com/MahtaFetrat/Virgool-Informal-Posts-Crawler), recording their spoken forms, and processing the raw audio and text files into smaller, equivalent chunks.

## Dataset Description

The dataset includes:
- Raw audio files recorded from the crawled text.
- Raw text files crawled from the blog.
- Processed audio and text chunks, aligned for ASR and TTS tasks.
- A fully open processing pipeline documented in a Jupyter Notebook, detailing each step from raw data to processed output.

### Raw Data

The raw data consists of:
- Audio files in their original format.
- Text files in their original format.

### Processed Data

The processed data consists of:
- Audio files converted from m4a to mono mp3 format.
- Text files normalized, cleaned, and tokenized into sentences.
- Aligned audio-text chunks created using the forced alignment tool Aeneas.

## Processing Notebook

The processing of the raw data is documented in a Jupyter Notebook, which includes the following steps:
1. **Audio Processing**: Converting audio files from m4a to mono mp3.
2. **Text Processing**: Normalizing text, removing and substituting symbols, removing links and references, converting numbers to their spoken format, and removing extra spaces.
3. **Sentence Tokenization**: Splitting text files into sentences using a custom sentence tokenization script.
4. **Forced Alignment**: Creating aligned audio-text chunks using Aeneas.

### Running the Notebook

To run the processing notebook, place the raw data files into a folder named `raw-data` in the root directory. The processed audio and text files will be output to a directory named `processed-data`, and the forced alignment results will be written to `forced-aligned-data`.

For detailed instructions on environment setup, please refer to [the processing notebook](https://github.com/MahtaFetrat/VirgoolInformal-Speech-Dataset/blob/main/VirgoolInformal_Dataset_Processing.ipynb).

You can view and run [the processing notebook in Google Colab](https://colab.research.google.com/drive/1AjvrRisJYdqvNdSDKdSWfxge6S29mavm?usp=sharing).

## Usage

The dataset can be used to evaluate Persian ASR models in terms of Character Error Rate (CER). For example, see this repository (link to be updated) for an ASR evaluation setup.

## Links

- [Raw Data](link to be updated)
- [Processed Data](link to be updated)
- [Processing Notebook in Colab](https://colab.research.google.com/drive/1AjvrRisJYdqvNdSDKdSWfxge6S29mavm?usp=sharing)

## License

This project is licensed under the open MIT License for the code and under the open CC-0 License for the data. 


## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


---

Enjoy working with the VirgoolInformal-Speech-Dataset!
