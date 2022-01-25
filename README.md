# CarlaObjectCordinateDecetion
This code detects pedesterians and vehicle in carla simulation enviroment and save their location as objectparam.txt. ( it is working dynamically, so it means it delete .txt and create new .txt file using pedesterian and vehicle coordinate, which is seen by camera of carla car.

Algoritm Logic:
Sementic Segmentation----> Threshold applly to detect (pedesterian and vehicles)---->erosion---> regionprops and labeling-----> matching with point cloud 
Dense Map ----> transform it to point cloud using inverse transformation (FOV=90) ----> Point cloud

Running code:
./CarlaUE4.sh  -windowed -carla-server -fps=30
~/CarlaSimulator/PythonClient$ python3 main.py


You can watch this video:
https://www.youtube.com/watch?v=Pr8TqUzFU_w
https://www.youtube.com/watch?v=nqkrxs6cCwY

