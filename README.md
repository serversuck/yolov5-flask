# Yolov5 object detection model deployment using flask
This repo contains example apps for exposing the [yolo5](https://github.com/ultralytics/yolov5) with custom object detection model(sea.pt)

## Web app
Simple app consisting of a form where you can upload an image, and see the inference result of the model in the browser. Run:

`$ python webapp.py --port 5000`

or

`$ python3 webapp.py --port 5000`


then visit http://localhost:5000/ in your browser:

<p align="center">
<img src="https://github.com/serversuck/yolov5-flask/blob/main/upload.png" width="450">
</p>

<p align="center">
<img src="https://github.com/serversuck/yolov5-flask/blob/main/result.png" width="450">
</p>

The example json result
```
[{'xmin': 47.1176986694, 
'ymin': 221.4556274414, 
'xmax': 401.8820495605, 
'ymax': 557.4293823242, 
      'confidence': 0.7438420057, 
      'class': 1, 
      'name': 'stingray'}, 
```



## Run & Develop locally
Run locally and dev with anaconda :
* `conda create -n python37 python=3.7`
* `conda activate python37`
* `git clone https://github.com/serversuck/yolov5-flask.git`
* `(python37) $ pip install -r requirements.txt`
* `(python37) $ python webapp.py --port 5000`

## YoloV5 model training by
mr sorapong somsorn sorapon@varee.ac.th

## reference
- https://github.com/ultralytics/yolov5
- https://github.com/jzhang533/yolov5-flask (this repo was forked from here)
- https://github.com/avinassh/pytorch-flask-api-heroku
