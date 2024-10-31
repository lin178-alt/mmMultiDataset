# mmMultiDataset

Human Activity Recognition (HAR) technology plays a central role in healthcare, elder care, security monitoring, and human-computer interaction, with its accuracy highly dependent on precise sensor data collection. Millimeter wave (mmWave) radar demonstrates exceptional performance in the HAR field due to its ability to penetrate non-metallic materials and provide high-resolution sensing. However, while traditional HAR methods using point cloud data from sensors such as LiDAR or mmWave can effectively capture information about single-user activities, they still face significant challenges when handling scenarios involving multiple independent activities or interactions among multiple individuals.

To address these challenges, this study introduces the innovative mmMultiDataset, designed to capture both macro and micro human movements in multi-person environments. This dataset records 11 different activities performed by seven subjects in three distinct environments, encompassing not only single-user actions but also scenarios where multiple individuals are engaged simultaneously.

The data in mmMultiDataset is stored in point cloud format, with each action precisely segmented into individual samples for ease of use by researchers. Data collection was meticulously conducted in controlled environments to ensure accuracy and reliability, covering a wide range of scenarios from single-user to multi-user activities.

The release of this dataset fills a critical gap in HAR systems concerning the recognition of independent and interactive activities among multiple users, providing an indispensable resource for enhancing the robustness and accuracy of activity recognition using mmWave radar. With the widespread application of mmMultiDataset, we anticipate that HAR technology will achieve more precise and efficient applications and developments across various fields.

The naming format for dataset samples is as follows:
Single-user actions:
- $P_{i}-action-cnt.npz$
Multi-user independent actions:
- $P_{i}^1,P_{i}^2-action1,action2-cnt.npz$
Multi-user interaction actions:
- $P_{i}^1,P_{i}^2-action-cnt.npz$


Each dataset consists of point cloud data and includes the following features:
| **Feature**     | **Description**                                                                                                                                            |
| :-------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------- |
| rangeIdx        | Index corresponding to the range bin of the detected object. It indicates the distance of the  object from the radar.                                      |
| dopplerIdx      | Index corresponding to the Doppler bin, which represents the relative velocity of the detected object.                                                     |
| peakVal         | The peak value of the detected signal, indicating the strength of the returned radar signal.                                                               |
| x\_coord        | The x-coordinate of the detected object in the radar's coordinate system.                                                                                  |
| y\_coord        | The y-coordinate of the detected object in the radar's coordinate system.                                                                                  |
| z\_coord        | The z-coordinate of the detected object in the radar's coordinate system.                                                                                  |

You can obtain the dataset we have collected by accessing this Google Drive link：https://drive.google.com/drive/folders/1UPL4JqCajLpDXpH0O481pyQQRZnk08Vz?usp=sharing
