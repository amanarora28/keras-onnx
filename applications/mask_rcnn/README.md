# Introduction
The original Keras project of Masked RCNN is: <https://github.com/matterport/Mask_RCNN>. Follow the 'Installation' section in README.md to set up the model.
There is also a good [tutorial](https://github.com/matterport/Mask_RCNN#step-by-step-detection) to learn about the object detection.

The conversion supports since opset 10, And the converted model need to be working with ONNXRuntime latest version which supports ONNX opset 10 and contrib ops needed by this model.

# Convert and Run the model.
```
cd <mask_rcnn directory>
pip install -e .
cd <keras2onnx directory>/applications/mask_rcnn
# convert the model to onnx and test it with an image.
python mask_rcnn.py <image_file_path>
```
