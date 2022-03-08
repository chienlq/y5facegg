<h4 align="center">
  pip install y5facegg
</h4>

## <div align="center">Use from Python</div>


<details open>
<summary>Usage</summary>

```python
import cv2
from y5facegg import Y5FACE

# set model params
model_path = "y5facegg/weights/yolov5s-face.pt"
device = "cuda:0" # or "cpu"

# init yolov5 model
model = Y5FACE(model_path, device)

# load an image
image_path = 'https://github.com/ultralytics/yolov5/blob/master/data/images/bus.jpg'

# perform inference
bgr_image = cv2.imread(image_path)
res_img = model.predict(bgr_image)
cv2.imwrite('result.jpg', res_img)

```

<details closed>

