# Build Teaser++ in docker container and dockerize  
## step 1 : Windows install WSL + Docker deskstop
[follow this yt](https://www.youtube.com/watch?v=f63h-se6JOU)

## step 2 : create Ubuntu:22.04 container
於wsl中輸入
docker create -i -t --name [container name] [image name]   
image的部分在設置時使用ubuntu:22.04 image來創建  

## step 3 : install PCL in container

有在docker hub 當中找到關於設置point cloud library(pcl) env的image  
[連結在此](https://hub.docker.com/r/pointcloudlibrary/env)  
    
但是安裝PCL的部分是跟著
[Ubuntu22.04安裝PCL](https://blog.csdn.net/u012660296/article/details/132450862)的方式安裝  
(因container只有ubuntu2204因此需額外安裝vim g++ git)  
apt-get install vim  
apt-get install g++  
apt-get install gcc   
apt-get install git  

## step 4 : Registration on 3DMatch with FPFH + TEASER + ICP
[follow this link](https://github.com/MIT-SPARK/TEASER-plusplus/tree/master/examples/teaser_python_fpfh_icp) 



