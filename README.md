# Garbage-detector with Mask R-CNN
A training project for detecting paper cup and shoe. More garbage may be added later.
The codes are based on implementation of Mask R-CNN by (https://github.com/matterport/Mask_RCNN) on Python 3, Keras, and TensorFlow. The model generates bounding boxes and segmentation masks for each instance of an object in the image.
This project was trained and tested in Google Colab.


Table of Contents
-----------------

  * [Requirements](#requirements)
  * [Usage](#usage)
  * [Contributing](#contributing)
  * [Support and Migration](#support-and-migration)
  * [License](#license)

Requirements
------------

The script requires the following to run:

  * Tensorflow version 1.x
  * Keras version 2.1.5
  

[python]: https://www.python.org/downloads/

Usage
-----

To run the code on Colab, You shoulf first create a new notebook. 

Clone Mask R-CNN and install it.

Add following classes

'GarbageConfig' : This class contains the default configurations. Modify the attributes for your training.

'GarbageDataset' : This class inherits from utils.Dataset which provides capability to train on new dataset without modifying the model.

example:
```sh
(base) C:\>python Compare_ID_Shenasa.py --index_directory C:Anahita\dataset\index --others_directory C:Anahita\dataset\others
--output_directory C:\Users\Anahita

```
Note : There is a space between each directory above.

The Script has the following inputs.

`index_directory` is the path of index folder, where the main pictures exist. 

`others_directory` is the path of others folder, where the copies of index pictures exist. 

`output_directory` is the path of output, where the two folders of "same" & "different" are created. 

### Error handling

The script will raise fallowing error if directories are not provided.

AttributeError: `NoneType` object

Contributing
-----

Not yet

Support and Migration
-----

Not yet

License
-----

Not yet
