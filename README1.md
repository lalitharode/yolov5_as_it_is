# git clone the repo.
git clone https://github.com/ultralytics/yolov5.git
cd yolov5

# create environment using python 3.8 or 3.9 then activate it
conda create --prefix envname python=3.8.0
conda activate ./envname

# install liabraries
pip install -r requirements.txt

# download yolov5s.pt model weights from link given in readme.md

# run for camera
python detect.py --source 0 --weights yolov5s.pt --conf-thres 0.5 --view-img



# Alternative we can also use our cv2 and torch to do the same detection.
# for this follow detect1.py which only need to run like 
python detect1.py

