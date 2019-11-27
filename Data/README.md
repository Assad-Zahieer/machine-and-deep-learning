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
* Images, sound etc. can be represented in tables vua **feature engineering**
#### Images
* Table of pixels
    * Each pixel has a RGB value
* Use PIL library to import image class
    * **from PIL import Image**
    * **img = Image.open('xxxxx')**
* Use *Convolutional Neural Networks*
