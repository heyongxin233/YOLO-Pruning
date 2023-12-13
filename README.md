# YOLO-Pruning
Easy Training Official YOLOv8、YOLOv7、YOLOv6、YOLOv5  and Prune all_model using Torch-Pruning!

You can use this code like [ultralytics for yolov8](https://github.com/ultralytics/ultralytics) 
```
pip install torch-pruning 
pip install -r requirements.txt
```

prune yolo like this
```
from ultralytics import YOLO
model = YOLO('yolov7m.yaml')
results = model.train(data='coco.yaml', epochs=10, imgsz=1280, batch=8, device=[3],name='yolov7',prune=True,prune_ratio=0.66874,prune_iterative_steps=1)

```
