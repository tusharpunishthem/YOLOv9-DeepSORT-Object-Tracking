<H1 align="center">
YOLOv9 Object Detection with DeepSORT Tracking(ID + Trails) </H1>

### New Features
- Added Label for Every Track
- Code can run on Both (CPU & GPU)
- Video/WebCam/External Camera/IP Stream Supported

## Ready to Use Google Colab
[`Google Colab File`](https://colab.research.google.com/drive/1IivrmAtnhpQ1PSmWsp-G6EnqsUOol9v8?usp=sharing)

## Steps to run Code

- Clone the repository
```
git clone https://github.com/MuhammadMoinFaisal/YOLOv9-DeepSORT-Object-Tracking.git
```
- Goto the cloned folder.
```
cd YOLOv9-DeepSORT-Object-Tracking
```
- Install requirements with mentioned command below.
```
pip install -r requirements.txt
```
- Download the pre-trained YOLOv9 model weights
[yolov9](https://github.com/WongKinYiu/yolov9/releases/download/v0.1/yolov9-c.pt)

- Downloading the DeepSORT Files From The Google Drive 
```
https://drive.google.com/drive/folders/1kna8eWGrSfzaR6DtNJ8_GchGgPMv3VC8?usp=sharing
```
- After downloading the DeepSORT Zip file from the drive, unzip it. 

- Download sample videos from the Google Drive
```
gdown "https://drive.google.com/uc?id=115RBSjNQ_1zjvKFRsQK2zE8v8BIRrpdy&confirm=t"
gdown "https://drive.google.com/uc?id=1rjBn8Fl1E_9d0EMVtL24S9aNQOJAveR5&confirm=t"
```
# for detection only
python detect.py --weights yolov7.pt --source "your video.mp4"

# for detection and tracking
python detect_and_track.py --weights yolov7.pt --source "your video.mp4"

# for WebCam
python detect_and_track.py --weights yolov7.pt --source 0

# for External Camera
python detect_and_track.py --weights yolov7.pt --source 1

# For LiveStream (Ip Stream URL Format i.e "rtsp://username:pass@ipaddress:portno/video/video.amp")
python detect_and_track.py --source "your IP Camera Stream URL" --device 0



### Watch the Complete Step by Step Explanation

- Video Tutorial Link  [`YouTube Link`](https://www.youtube.com/watch?v=9jRRZ-WL698)


[![Watch the Complete Tutorial for the Step by Step Explanation](https://img.youtube.com/vi/9jRRZ-WL698/0.jpg)]([https://www.youtube.com/watch?v=StTqXEQ2l-Y](https://www.youtube.com/watch?v=9jRRZ-WL698))

