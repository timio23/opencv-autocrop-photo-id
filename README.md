# OpenCv - Face Crop : Autodetect & crop faces out of an image (Node.js)

<!-- ![CI](https://github.com/arghyadeep-k/opencv-autocrop-photo-id/workflows/CI/badge.svg?branch=master)
![codecov.io](https://codecov.io/github/arghyadeep-k/opencv-autocrop-photo-id/coverage.svg?branch=master)
![npm](https://img.shields.io/npm/v/opencv-autocrop-photo-id)
![npm bundle size](https://img.shields.io/bundlephobia/min/opencv-autocrop-photo-id)
![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/npm/opencv-autocrop-photo-id)
![Depfu](https://img.shields.io/depfu/arghyadeep-k/opencv-autocrop-photo-id)
![Snyk Vulnerabilities for npm package](https://img.shields.io/snyk/vulnerabilities/npm/opencv-autocrop-photo-id)
![npm](https://img.shields.io/npm/dt/opencv-autocrop-photo-id)
![NPM](https://img.shields.io/npm/l/opencv-autocrop-photo-id?color=blue) -->


This package automatically detects faces in a picture and crops them for use as Photo ID.

## Installation

<!-- [![NPM](https://nodei.co/npm/opencv-autocrop-photo-id.png)](https://nodei.co/npm/opencv-autocrop-photo-id/) -->

**Install from command line:**

`npm install --save opencv-autocrop-photo-id`



## Basic Usage
```javascript
const facecrop = require('opencv-autocrop-photo-id');

facecrop('./image-file.jpg', './dest/output.jpg', "image/jpeg", 0.95, 0.25);

/* Outputs image with file name output.jpg in 'dest' folder with the face cropped out.

If multiple faces are detected, the files will be automatically renamed to output-1.jpg, output-2.jpg and so on.
*/
```

## Results

Original Image:



<br><br>
Cropped Image:



## API
**facecrop(input_filename, output_filename, type, quality, factor)**

- **input_filename**: Input String containing file name with relative/absolute filepath.

- **output_filename**: (Optional) Requires a string value which will contains the output file name.

- **type**: (Optional) Requires String value which will tell the format of the output image.

- **quality**: (Optional) Requires a float value between 0 to 1 which stands for the quality index of the output file compares to the input file. Set 1 for no reduction in quality.

- **factor**: (Optional) Percentage by which the area of cropping of the face should be increased to add more details.

## Defaults 

 - **input_filename**: Mandatory parameter
 - **output_filename**: "./output.jpg"
 - **type**: 'image/jpeg'
 - **quality**: 0.95
 - **factor**: 0


## License

OpenCV Autocrop Photo ID is published under the Public GNU license. For more information, see the accompanying LICENSE file. 

<br>

---

<br>
