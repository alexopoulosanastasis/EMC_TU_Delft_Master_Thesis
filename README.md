# EMC_TU_Delft_Master_Thesis
The current repository contains the code files I created during my master thesis project with the title "Do AI-based MRI features influence the early detection of knee OA"


The main goal of my master thesis project is the early detection of knee osteoarthritis through MRI scans. 
The input data are acquired from the publicly available dataset of OsteoArthritis Initiative (OAI). 

In order to create the dataset that is going to be used as input to the detection deep learning algorithms the different MRI features were examined,
and after the application of multiple conditions the final control and progression datasets were created. Due to lack of features availability for 
a long period of months, the early prediction of knee OA progression is studied between baseline and 24 months.

The second step of my approach is to construct a semi-automated method to extract the knee joint region. In order to achieve this, 
initially a U-Net was trained for DESS MRI sequences bone segmentation. The created DESS bone masks were then registered in the IW-TSE MRIs
in order to have a clearer approach to detect minimum and maximum tibia and femur coordinates and from them create the cropping box.

The next step is to create the two Deep Learning methods, a 3D DenseNet and a 3D Autoencoder, for the purpose of early detection of 
knee OA from MRI scans.
