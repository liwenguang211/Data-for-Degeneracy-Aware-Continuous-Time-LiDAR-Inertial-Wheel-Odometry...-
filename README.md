# Data for "Degeneracy-Aware Continuous-Time LiDAR-Inertial-Wheel Odometry Using Geometric Planelet Normal Statistics"

This repository contains the processed data and evaluation results supporting the manuscript (Reference: MST-137694.R2).

## 1. Directory Structure

The dataset is organized into 12 main folders: 6 for processed evaluation data and 6 for keyframe point clouds.

| Folder Name | Category | Description |
|-------------|----------|-------------|
| `bridge_data` | Processed Data | Evaluation results for the bridge scene. |
| `town_data` | Processed Data | Evaluation results for the town scene. |
| `Roundabout_data` | Processed Data | Evaluation results for the roundabout scene. |
| `mixed_data` | Processed Data | Evaluation results for the mixed indoor scene. |
| `parking_data` | Processed Data | Evaluation results for the parking indoor scene. |
| `workshop_data` | Processed Data | Evaluation results for the workshop indoor scene. |
| `keyframe_bridge` | Keyframe Data | Keyframe point clouds for the bridge scene. |
| `keyframe_town` | Keyframe Data | Keyframe point clouds for the town scene. |
| `keyframe_roundabout` | Keyframe Data | Keyframe point clouds for the roundabout scene. |
| `keyframe_mixed` | Keyframe Data | Keyframe point clouds for the mixed indoor scene. |
| `keyframe_parking` | Keyframe Data | Keyframe point clouds for the parking indoor scene. |
| `keyframe_workshop` | Keyframe Data | Keyframe point clouds for the workshop indoor scene. |

## 2. File Types

- `*_ape.csv`: Per-pose absolute pose error series.
- `ape_overall_statistics.csv`: Aggregate APE statistics.
- `*_rotation_error.csv`: Rotation error series.
- `xyz_direction_errors.csv` / `xy_direction_errors.csv`: Directional error records.
- `groundtruth_reconstructed.csv`: Reconstructed reference trajectory.
- `used_config.json`: Configuration and deterministic processing parameters.
- `.pcd` / `.ply`: Keyframe point cloud files.
- `.png` / `.pdf`: Exported figures.

## 3. Data Availability

The processed data and evaluation results (CSV, JSON, figures) are available in this GitHub repository:
https://github.com/liwenguang211/Data-for-Degeneracy-Aware-Continuous-Time-LiDAR-Inertial-Wheel-Odometry

The large keyframe point cloud data (MSI) are available from Baidu Netdisk:
- Link: 通过网盘分享的文件：MSI
链接: https://pan.baidu.com/s/1hSi9edQWFfeE5L3LVcT3Dw 提取码: 5577 
--来自百度网盘超级会员v8的分享
- Extract code: 5577
- Root folder: MSI



## 4. Reproducibility Notes

1. Keep the relative folder structure unchanged when using the exported paths in analysis scripts.
2. Use the CSV files for numerical analysis and the PNG/PDF files only for visual checking.
3. Check `used_config.json` before regenerating a plot; smoothing, axis choice, and random seed affect the exported directional-error curves.
4. HeLiPR scenes (bridge, town, roundabout) use LiDAR+IMU only; indoor scenes (mixed, parking, workshop) use LiDAR+IMU+wheel/steering when available.

## 5. License and Citation

License: CC-BY 4.0.

Suggested citation:
Li, W. et al. (2026). Data for "Degeneracy-Aware Continuous-Time LiDAR-Inertial-Wheel Odometry Using Geometric Planelet Normal Statistics" [Data set]. GitHub.
https://github.com/liwenguang211/Data-for-Degeneracy-Aware-Continuous-Time-LiDAR-Inertial-Wheel-Odometry
Keyframe MSI mirror: Baidu Netdisk (Extract code: 5577).