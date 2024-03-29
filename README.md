### Official Python Implementation
This work was conducted by Soeun Han, Wonjun Park, Kyumin Jeong, Taehoon Hong, and `Choongwan Koo (Corresponding Author)` | Paper

Affiliation: Construction Engineering & Management Lab, Incheon National University.

### Cite This:
Han, S., Park, W., Jeong, K., Hong, T., and `Koo, C.` (2024). “Utilizing synthetic images to enhance the automated recognition of small-sized construction tools”, Automation in Construction (under review). <br><br>

# Utilizing synthetic images to enhance the automated recognition of small-sized construction tools

### Abstract
Previous studies on vision-based classifiers often overlooked the need for detecting small-sized construction tools. Considering the substantial variations in these tools' size and shape, it is essential to train models using synthetic images that encompass diverse angles and distances. This study aimed to improve the performance of classifiers for small-sized construction tools by leveraging synthetic data. Three classifiers were proposed using YOLOv8 algorithm, varying in data composition: (i) 'Real-4000': 4,000 authentic images; (ii) 'Hybrid-4000': 2,000 authentic and 2,000 synthetic images; (iii) 'Hybrid-8000': 4,000 authentic and 4,000 synthetic images. To assess practical applicability, a test dataset of 144 samples for each type was collected directly from construction sites. Results revealed that the 'Hybrid-8000' model, utilizing synthetic images, excelled at 94.8% of mAP_0.5. This represented a significant 15.2% improvement, affirming its practical applicability. These classifiers hold promise for enhancing safety and advancing real-time automation and robotics in construction. <br><br>

### Keywords
Small-sized construction tools; Object detection and classification; Synthetic images; Practical applicability; Construction site <br><br>

### Research Framework and Dataset
**Figure 1.** Research framework

![Figure1](https://github.com/SenseableSpace/Utilizing-synthetic-images-to-enhance-the-automated-recognition-of-small-sized-construction-tools/assets/162809473/1afa48da-a6dc-4c52-9caf-e3ff537d737f) <br><br>

**Figure 2.** Representative examples of training and test dataset

![Figure2](https://github.com/SenseableSpace/Utilizing-synthetic-images-to-enhance-the-automated-recognition-of-small-sized-construction-tools/assets/162809473/d6a0af99-7ed6-4626-a7d7-f579fc7ee43c) <br><br>

### Results
**Figure 3.** Inference results - confidence scores of small-sized tools, ‘Hammer’

![Figure3](https://github.com/SenseableSpace/Utilizing-synthetic-images-to-enhance-the-automated-recognition-of-small-sized-construction-tools/assets/162809473/2dec8ec7-8313-426b-a5fa-d25c10064707) <br><br>

**Figure 4.** Inference results - confidence scores of small-sized tools, ‘Tacker'

![Figure4](https://github.com/SenseableSpace/Utilizing-synthetic-images-to-enhance-the-automated-recognition-of-small-sized-construction-tools/assets/162809473/58cb1a71-fad5-4ebe-9864-ff97a80a5f4d) <br><br>

### Code Definition
| Category                 | Description                                                                           |
| ------------------------ | --------------------------------------------------                                    |
| `ScreenshotCapture.cs`   | This code has been used to automatically generate a group of synthetic images by capturing the screen while incrementally changing the viewing angles of a 3D object's x and y axes from 0° to 360° by 15° increments. |
| `YOLOv8_open.ipynb`      | This code has been used to develop the proposed vision-based classifiers (i.e., 'Real-4000,' 'Hybrid-4000,' and 'Hybrid-8000') for the automated recognition of small-sized construction tools. |

### Data Availability Statements
Some or all of the data or code that support the findings of this study are available from the corresponding author upon reasonable request. <br><br>

### Download link
| Category                                | Total    | Link                                                                                 | Release Date |
| --------------------------------------- | -------- |  ----------------------------------------------------------------------------------  | ------------ |
| `Training dataset-[Real-4000]-images`   | 4,000    | https://drive.google.com/file/d/1oR4iLT82qBX_xiZD8yXkVHOjpNZ51gQr/view?usp=sharing   | 11 Mar 2024  |
| `Training dataset-[Real-4000]-labels`   | 4,000    | https://drive.google.com/file/d/1Z-TaXi1k6Mr5hyfd8eiyuY52kZWPkHOS/view?usp=sharing   | 11 Mar 2024  |
| `Training dataset-[Hybrid-4000]-images` | 4,000    | https://drive.google.com/file/d/1hwVtejkUj0JpTiv-q2jjtW3ZzgIdFl-L/view?usp=sharing   | 11 Mar 2024  |
| `Training dataset-[Hybrid-4000]-labels` | 4,000    | https://drive.google.com/file/d/1hwVtejkUj0JpTiv-q2jjtW3ZzgIdFl-L/view?usp=sharing   | 11 Mar 2024  |
| `Training dataset-[Hybrid-8000]-images` | 8,000    | https://drive.google.com/file/d/1hwVtejkUj0JpTiv-q2jjtW3ZzgIdFl-L/view?usp=sharing   | 11 Mar 2024  |
| `Training dataset-[Hybrid-8000]-labels` | 8,000    | https://drive.google.com/file/d/10Wl94qQ8DciSnBAyVLlLu1ZQdqOi4wCq/view?usp=sharing   | 11 Mar 2024  |
| `Test dataset-images`                   | 576      | https://drive.google.com/file/d/1y5yLGsyNBXmoyT1IUd4-qJqo6mXeTAoj/view?usp=sharing   | 11 Mar 2024  |
| `Test dataset-labels`                   | 576      | https://drive.google.com/file/d/1gPlacSloHKc422tVJdQgEpHhs5W7iT8k/view?usp=sharing   | 11 Mar 2024  |
