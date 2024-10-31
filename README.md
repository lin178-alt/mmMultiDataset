# mmMultiDataset

Human Activity Recognition (HAR) technology is vital in fields such as healthcare, elder care, security monitoring, and human-computer interaction. Its effectiveness largely relies on accurate sensor data collection. Millimeter wave (mmWave) radar stands out in HAR applications due to its ability to penetrate non-metallic materials and deliver high-resolution sensing. However, traditional HAR methods utilizing point cloud data from sensors like LiDAR or mmWave face significant challenges when recognizing multiple independent activities or interactions among several individuals.

To tackle these challenges, we present the mmMultiDataset, an innovative dataset designed to capture both macro and micro human movements in multi-person environments. This dataset records 11 distinct activities performed by seven subjects across three different settings, encompassing not only single-user actions but also scenarios involving multiple participants.

The mmMultiDataset is organized in point cloud format, with each activity meticulously segmented into individual samples for ease of use by researchers. Data collection was conducted in controlled environments to ensure accuracy and reliability, covering a broad spectrum of scenarios, from single-user to multi-user activities.

The release of this dataset addresses a critical gap in HAR systems concerning the recognition of independent and interactive activities among multiple users. It provides a crucial resource for enhancing the robustness and accuracy of activity recognition using mmWave radar. We anticipate that the widespread application of mmMultiDataset will lead to more precise and efficient advancements in HAR technology across various fields.

### Sample Naming Format
- **Single-user actions:**  
  `$P_{i}-action-cnt.npz`
- **Multi-user independent actions:**  
  `$P_{i}^1,P_{i}^2-action1,action2-cnt.npz`
- **Multi-user interaction actions:**  
  `$P_{i}^1,P_{i}^2-action-cnt.npz`

### Dataset Features
Each dataset consists of point cloud data with the following features:

| **Feature**     | **Description**                                                                                                                                            |
| :-------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------- |
| rangeIdx        | Index corresponding to the range bin of the detected object, indicating its distance from the radar.                                                      |
| dopplerIdx      | Index corresponding to the Doppler bin, representing the relative velocity of the detected object.                                                         |
| peakVal         | The peak value of the detected signal, indicating the strength of the returned radar signal.                                                               |
| x_coord         | The x-coordinate of the detected object in the radar's coordinate system.                                                                                  |
| y_coord         | The y-coordinate of the detected object in the radar's coordinate system.                                                                                  |
| z_coord         | The z-coordinate of the detected object in the radar's coordinate system.                                                                                  |

You can access the collected dataset via this Google Drive link: [mmMultiDataset](https://drive.google.com/drive/folders/1UPL4JqCajLpDXpH0O481pyQQRZnk08Vz?usp=sharing).

--- 

Feel free to modify any part if you'd like!
