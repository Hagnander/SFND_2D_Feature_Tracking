# SFND 2D Feature Tracking Mid Term Project

This is the Submission for the Mid Term Project in Sensor Fusion Nano degree by Udacity

#### Task MP.7 Performance Evaluation 1
> Count the number of keypoints on the preceding vehicle for all 10 images and take note of the distribution of their neighborhood size. Do this for all the detectors you have implemented.

|         |1  |2  |3  |4  |5  |6  |7  |8  |9  |10 |
|---------|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
|SHITOMASI|125|118|123|120|120|113|114|123|111|112|
|HARRIS   |50 |54 |53 |55 |56 |58 |57 |61 |59 |57 |
|FAST     |149|152|150|155|149|149|156|150|138|143|
|BRISK    |264|282|282|277|297|279|289|272|266|254|
|ORB      |92 |102|106|113|109|125|130|129|127|128|
|AKAZE    |166|157|161|155|163|164|173|175|177|179|
|SIFT     |138|132|124|137|134|140|137|148|159|137|

---

#### Task MP.8 Performance Evaluation 2
> Count the number of matched keypoints for all 10 images using all possible combinations of detectors and descriptors. In the matching step, the BF approach is used with the descriptor distance ratio set to 0.8.

|Detector-Descriptor|2  |3  |4  |5  |6  |7  |8  |9  |10 |
|-------------------|---|---|---|---|---|---|---|---|---|
|SHITOMASI-BRISK    |84 |80 |73 |77 |74 |70 |79 |81 |72 |
|SHITOMASI-BRIEF    |96 |93 |92 |89 |92 |93 |85 |91 |85 |
|SHITOMASI-ORB      |87 |82 |87 |90 |83 |77 |84 |86 |89 |
|SHITOMASI-FREAK    |68 |69 |64 |64 |63 |61 |62 |62 |62 |
|SHITOMASI-SIFT     |112|109|104|103|99 |101|96 |106|97 |
|HARRIS-BRISK       |37 |36 |41 |39 |36 |36 |45 |45 |40 |
|HARRIS-BRIEF       |42 |42 |43 |45 |41 |48 |46 |47 |49 |
|HARRIS-ORB         |43 |38 |39 |42 |44 |44 |43 |51 |48 |
|HARRIS-FREAK       |36 |32 |31 |30 |30 |35 |35 |39 |35 |
|HARRIS-SIFT        |46 |46 |50 |52 |51 |48 |52 |59 |55 |
|FAST-BRISK         |80 |91 |85 |94 |71 |83 |92 |86 |94 |
|FAST-BRIEF         |88 |102|88 |102|94 |98 |112|107|92 |
|FAST-ORB           |95 |102|87 |94 |88 |95 |104|96 |98 |
|FAST-FREAK         |64 |80 |60 |74 |58 |79 |78 |80 |84 |
|FAST-SIFT          |118|123|110|119|114|119|123|117|103|
|BRISK-BRISK        |138|144|133|144|139|155|137|150|158|
|BRISK-BRIEF        |138|166|129|141|148|155|158|161|148|
|BRISK-ORB          |97 |103|91 |92 |82 |117|109|108|114|
|BRISK-FREAK        |112|123|109|118|102|127|135|133|131|
|BRISK-SIFT         |182|193|169|183|171|195|194|176|183|
|ORB-BRISK          |60 |65 |65 |76 |72 |83 |83 |73 |72 |
|ORB-BRIEF          |37 |38 |37 |53 |42 |64 |58 |62 |59 |
|ORB-ORB            |40 |52 |46 |54 |53 |65 |68 |65 |72 |
|ORB-FREAK          |39 |33 |38 |41 |33 |40 |42 |39 |44 |
|ORB-SIFT           |67 |79 |78 |79 |82 |95 |95 |94 |94 |
|AKAZE-BRISK        |126|112|121|117|114|119|134|140|127|
|AKAZE-BRIEF        |108|116|110|109|116|129|133|135|131|
|AKAZE-ORB          |102|91 |97 |86 |95 |114|107|112|118|
|AKAZE-FREAK        |104|104|92 |101|97 |111|124|117|116|
|AKAZE-SIFT         |134|134|130|136|137|147|147|154|151|
|SIFT-BRISK         |57 |63 |58 |61 |55 |52 |54 |63 |73 |
|SIFT-BRIEF         |63 |72 |64 |66 |52 |57 |72 |67 |84 |
|SIFT-FREAK         |58 |63 |53 |63 |50 |50 |46 |52 |65 |
|SIFT-SIFT          |82 |81 |85 |93 |90 |81 |82 |102|104|

---

#### Task MP.9 Performance Evaluation 3
> Log the time it takes for keypoint detection and descriptor extraction. The results must be entered into a spreadsheet and based on this data, the TOP3 detector / descriptor combinations must be recommended as the best choice for our purpose of detecting keypoints on vehicles.

|Detector-Descriptor|Average nr. of keypoints detected|Average time needed to extract detectors and descriptors [ms]|
|-------------------|---------------------------------|-------------------------------------------------------------|
|SHITOMASI-BRISK    |77                               |1.97                                                         |
|SHITOMASI-BRIEF    |91                               |1.97                                                         |
|SHITOMASI-ORB      |85                               |3.00                                                         |
|SHITOMASI-FREAK    |64                               |7.11                                                         |
|SHITOMASI-SIFT     |103                              |3.79                                                         |
|HARRIS-BRISK       |39                               |5.08                                                         |
|HARRIS-BRIEF       |45                               |4.18                                                         |
|HARRIS-ORB         |44                               |5.48                                                         |
|HARRIS-FREAK       |34                               |13.03                                                        |
|HARRIS-SIFT        |51                               |6.78                                                         |
|FAST-BRISK         |86                               |0.44                                                         |
|FAST-BRIEF         |98                               |0.47                                                         |
|FAST-ORB           |95                               |1.18                                                         |
|FAST-FREAK         |73                               |4.95                                                         |
|FAST-SIFT          |116                              |2.26                                                         |
|BRISK-BRISK        |144                              |2.38                                                         |
|BRISK-BRIEF        |149                              |2.17                                                         |
|BRISK-ORB          |101                              |4.08                                                         |
|BRISK-FREAK        |121                              |4.52                                                         |
|BRISK-SIFT         |183                              |2.84                                                         |
|ORB-BRISK          |72                               |2.24                                                         |
|ORB-BRIEF          |50                               |3.10                                                         |
|ORB-ORB            |57                               |4.84                                                         |
|ORB-FREAK          |39                               |10.59                                                        |
|ORB-SIFT           |85                               |5.32                                                         |
|AKAZE-BRISK        |123                              |4.66                                                         |
|AKAZE-BRIEF        |121                              |5.14                                                         |
|AKAZE-ORB          |102                              |6.30                                                         |
|AKAZE-FREAK        |107                              |7.04                                                         |
|AKAZE-SIFT         |141                              |5.14                                                         |
|SIFT-BRISK         |60                               |12.95                                                        |
|SIFT-BRIEF         |66                               |11.06                                                        |
|SIFT-FREAK         |56                               |17.36                                                        |
|SIFT-SIFT          |89                               |13.06                                                        |

This leads to the following Top 3:

|Detector-Descriptor|Average nr. of keypoints detected|Average time needed to extract detectors and descriptors [ms]|
|-------------------|---------------------------------|-------------------------------------------------------------|
|FAST-BRISK         |86                               |0.44                                                         |
|FAST-BRIF          |98                               |0.47                                                         |
|FAST-ORB           |95                               |1.18                                                         |


Motivation
They are much faster than the the other combinationes of keypoint detection/descriptior extration while still finding the same number of keypoints in the images.

