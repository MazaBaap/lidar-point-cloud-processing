# LiDAR Point Cloud Processing

This project processes LiDAR point cloud data from the KITTI dataset using Open3D. The pipeline includes:
- Loading the raw point cloud
- Downsampling with a voxel grid
- Filtering noise using statistical outlier removal
- Segmenting ground vs. objects using RANSAC
- Clustering obstacles using DBSCAN
- Labeling clusters as "Car" or "Pedestrian" based on size
- Processing a sequence of frames

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

## Requirements
- `Python 3.x`
- `open3d`
- `numpy`

## Setup
1. Clone this repository:

      git clone https://github.com/MazaBaap/lidar-point-cloud-processing.git

      cd lidar-point-cloud-processing

3. Install dependencies:

      pip install open3d numpy

4. Download the KITTI dataset and place the `.bin` files in a `kitti/` directory within the project.
5. Run the notebook:

      lidar_processing.ipynb
