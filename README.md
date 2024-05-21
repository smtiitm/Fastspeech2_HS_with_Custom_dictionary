# FastSpeech2_HS Inference with Custom Dictionary

This repository provides an updated preprocessing file and custom_dict for inference of the FastSpeech2_HS models using a custom dictionary to improve the pronunciation of domain-specific words and abbreviations that may be mispronounced by the trained model.

## Getting Started

### Clone the Repository

First, clone the original repository:

```bash
git clone https://github.com/smtiitm/Fastspeech2_HS
```

Alternatively, you can download and copy the above files and paste it into the already cloned repo.

### Update the Text Preprocessing File

Replace the `text_preprocess_for_inference.py` file in the original repository with the updated version provided.

### Add the Custom Dictionary

Place your `Custom_dict` file inside the `phone_dict` folder in the repository.

### Usage

With the custom dictionary in place, the inference process will proceed as follows:
1. The code will first check for words in the `Custom_dict`.
2. If a word is not found in the `Custom_dict`, it will then check the original dictionary.
3. If the word is not found in either dictionary, the unified parser will parse the word and add it to the dictionary.

This process helps ensure that domain-specific words,symbols and abbreviations etc. are pronounced correctly as per the users requirements.

### Note

The code is in the initial stages and requires testing with a more number of end test cases.

TODO:

- [] Update code for handling VTT/subtitles

## Thank You

Thank you for using this repository. Your feedback and contributions are welcome to help improve the model and its performance.
