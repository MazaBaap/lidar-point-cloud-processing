# LiDAR Point Cloud Processing

This project processes LiDAR point cloud data from the KITTI dataset using Open3D. The pipeline includes:
- Loading the raw point cloud
- Downsampling with a voxel grid
- Filtering noise using statistical outlier removal
- Segmenting ground vs. objects using RANSAC
- Clustering obstacles using DBSCAN
- Labeling clusters as "Car" or "Pedestrian" based on size
- Processing a sequence of frames
- **Unique Feature**: 3D bounding boxes for object detection

## Screenshots
- **Raw Point Cloud**  
  ![Raw Point Cloud](raw.png)
- **Downsampled Point Cloud**  
  ![Downsampled Point Cloud](downsampled.png)
- **Filtered Point Cloud**  
  ![Filtered Point Cloud](filtered.png)
- **Ground vs. Objects**  
  ![Segmented Point Cloud](segmented.png)
- **Clustered Obstacles**  
  ![Clustered Obstacles](clustered.png)
- **Sequence Frame 0**  
  ![Frame 0](Frame_0.png)
- **Sequence Frame 4**  
  ![Frame 4](Frame_4.png)
- **3D Bounding Boxes**  
  ![3D Bounding Boxes](bounding_boxes.png)

## Requirements
- `Python 3.x`
- `open3d`
- `numpy`

## Setup
1. Clone this repository:

      git clone https://github.com/MazaBaap/lidar-point-cloud-processing.git

      cd lidar-point-cloud-processing

3. Install dependencies:

      pip install -r requirements.txt

4. Download the KITTI dataset and place the `.bin` files in a `kitti/` directory within the project.
5. Run the notebook:

      lidar_processing.ipynb
