# speech

Lightweight collection of Jupyter notebooks for audio / speech experiments: Whisper transcription & fine-tuning demos, feature extraction, and quick experiments.

Detected files
- fine_tune_whisper.ipynb — notebook showing steps to fine-tune a Whisper-style model
- whisper_transcription.ipynb — notebook demonstrating transcription/inference with Whisper

Quickstart

1. Clone
   git clone https://github.com/jumanewton/speech.git
   cd speech

2. Create environment
   python3 -m venv .venv
   source .venv/bin/activate  # macOS / Linux
   .venv\Scripts\activate     # Windows PowerShell

3. Install dependencies
   pip install -r requirements.txt

4. Run notebooks
   jupyter lab
   or
   jupyter notebook

Notes about the notebooks
- Open each notebook and run the top cells first — they declare file paths and (sometimes) small configuration cells.
- The Whisper notebooks expect audio files and may reference small dataset directories. Check the first cells for the expected paths.
- Fine-tuning notebooks may need GPU and additional setup (accelerate / transformers). Use small subsets when experimenting.

Data suggestions
- Use small sample datasets for quick iteration (e.g., a handful of WAV files).
- If using larger corpora (LibriSpeech / Common Voice), pre-download and point the notebooks at the local paths.

Recommended additions (helpful later)
- Add a LICENSE
- Add small sample data or a script to download a tiny example dataset
- Add a short CONTRIBUTING.md with how to add new notebooks and dependency rules

Contact
- Open an issue for questions or describe what you want added and I can adjust the README and requirements accordingly.
