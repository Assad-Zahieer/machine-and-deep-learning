# Data
## Types
1. Tabular
2. Unstructured data
### 1. Tabular Data
* Excel, CSV (comma seperated values) etc.
* Row - record or data points
    * age, gender etc. = *features* of a record
    * Features can be calculate (engineered) or measured (n.o. times I visited the bathroom)
* Data Types
    * Descrete - categorical data e.g. eye colour
    * Continuous - measured e.g. height, speed etc.
### 2. Unstructed Data
* Images, sound etc. can be represented in tables via **feature engineering**
#### Images
* Table of pixels
    * Each pixel has a RGB value
* Use PIL library to import image class
    * **from PIL import Image**
    * **img = Image.open('xxxxx')**
* Use *Convolutional Neural Networks*
    * Deep learning algorythm takes images as input assign importance to specific features (identifiers) of the image and use these to differentiate.
#### Sound
* Key value stored in associative array
* Use scipy.io to import wavfile class
    * **from scipy.io import wavfile**
* Return sample rate and data from a WAV file
    * **rate, snd = wavfile.read(filename = 'xxxxx')**
    * from IPython.display import Audio
    * Audio(data=snd, rate=rate)
