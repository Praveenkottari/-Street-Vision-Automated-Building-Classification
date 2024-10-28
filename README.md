# Are you in a safe building: Street Vision based Automated Building Classification
Managing earthquake risks is essential due to the high potential for loss of life and economic damage. To mitigate building collapses, structural stability is a critical focus. Our project addresses the challenge of identifying potentially unsafe buildings in large urban areas by leveraging technology and data from street-view images. Traditional building-by-building inspections are impractical at scale, but advancements in machine learning offer a solution.This project aims to develop a supervised ML model to classify buildings by structural safety risk. We tackle challenges inherent in street-view imagery, such as noise and uneven distribution, through meticulous data cleaning and robust model development. Our objective is to enable accurate, scalable risk assessment for urban environments, contributing to safer cities.


## Dataset
The dataset for this project includes 2,516 grayscale images, each with a resolution of 300x400 pixels. These images represent five distinct building classes, differentiated by materials and structural characteristics as outlined in Table. Captured from various streets, the images offer diverse perspectives and building conditions, with each class exhibiting unique texture patterns related to its structural properties. Despite these distinctions, common features across classes increase the classification complexity. Annotations highlight key structural features to guide model training, but the dataset includes misclassified samples and class imbalances, necessitating rigorous data cleaning.

Descriptions of these defect classes along with the number of image samples available for each:

| Class  | Description                                                                    | Number of Images |
|--------------|--------------------------------------------------------------------------------|-----------------:|
| **Class 1 (SteelBuildings)**    |  Steel Buildings, large presence of glass, significant slenderness.        | 282            |
| **Class 2 (Concrete)** | Concrete, boxy aspect, smooth texture, persistent opening.                                            | 320             |
| **Class 3 (Masonry)** |  Masonry, bricks exposed, no soft story, decorative patterns.                                               | 575             |
| **Class 4 (Woodenframed)**  | Wooden framed, wooden bow windows, slanted roof.                                           | 700          |
| **Class 5 (panel buildings)** | Steel with panel, industrial/retail, max 2 floors, non-slanted roof.                                        | 298            |

## Sample Images

<table border="0" style="text-align: center;">
  <tr>
    <td style="text-align: center;"><img src="sample data/1/17_A.jpg" width="200" /><br><b>(a) Algae</b></td>
    <td style="text-align: center;"><img src="sample images/class_images/major crack/cls01_020.jpg" width="200" /><br><b>(b) Major Crack</b></td>
    <td style="text-align: center;"><img src="sample images/class_images/minor crack/cls02_031.jpg" width="200" /><br><b>(c) Minor Crack</b></td>
  
  </tr>
  <tr>
    <td style="text-align: center;"><img src="sample images/class_images/spalling/cls05_013.jpg" width="200" /><br><b>(e) Spalling</b></td>
    <td style="text-align: center;"><img src="sample images/class_images/stain/cls06_082.jpg" width="200" /><br><b>(f) Stain</b></td>
  </tr>
</table>


## Dataset preparation

The image dataset collection began by inspecting and identifying building structures that were in a maintained condition. More than 50 buildings, constructed at different times and with ages ranging from 10 to 60 years, were visited. For image capture, we used a smartphone with a high-resolution camera, and all samples were taken approximately 1 meter away from the walls. The images were collected both indoors and outdoors across various campus buildings, which had different material surfaces such as concrete and stone. Afterward, the collected data were assembled for preprocessing and cleaning. Annotation was then performed with respect to the specific defect classes, generating the final dataset.


![Flowchart](https://github.com/Praveenkottari/BD3-Dataset/blob/3d45ea59b1c514bea5e6a3c52c103986a5953b36/sample%20images/markdown_images/flow-chart3.png)

<p align="center"><i>Figure : Dataset preparation work-flow</i></p>



## Benchmarking

