There are a wide range of snake species that are native to India.  Many of them are venomous, such as cobras 
and kraits, while others, like keelbacks and pythons, are non-venomous. Snakes can often be found in human 
habitats, especially in villages. The classification of snakes is not easy because they often share similar features. 
It is essential to identify whether they are venomous or non-venomous, as this knowledge is crucial for reducing 
snakebite-related deaths by providing appropriate medicine in a timely manner [1]. An analysis of 60 articles, 
encompassing 363 victims, revealed that 88% of snakebites were from venomous snakes, while 12% were from 
non-venomous ones. When necrosis was present, 15.2% of cases reported no infection, even when antibiotics 
were not used, suggesting potential antibacterial properties in snake venom.  
Hence, in this work, we have proposed a deep learning model utilizing Xception [2] and the Convolutional 
Block Attention Module (CBAM) [3] to automatically categorize snakes by their species name and determine 
whether the snake is venomous or nonvenomous (Figure 1). We initially compiled a comprehensive dataset of 
Indian snakes, consisting of nearly 3000 images distributed across fifteen distinct classes and this dataset is used 
in the proposed model (Figure 2). Our proposed methodology demonstrated effectiveness in efficiently 
integrating information from the target domain, with a specific focus on extracting crucial features from 
significant regions. This enhancement significantly bolstered the model’s capability for feature extraction. This 
study presents significant contributions across three main areas: 1. It introduces an Indian snake dataset 
consisting of nearly 3000 images distributed among fifteen diverse classes. 2. Initially, a CNN model was 
developed from scratch. Subsequently, pre-trained models were utilized with fine-tuning for training purposes. 
This dataset was split into training and testing sets at an 85%:15% ratio, with 2482 images used for training and 
446 images reserved for testing. For classification tasks, we employed a deep learning model incorporating an 
Exception and CBAM architecture. The model was trained using the Adam optimizer with a learning rate set to 
0.0001, aiming to minimize the categorical cross entropy loss function. During training, data was processed in 
batches of 16 samples per iteration. Among the various pre-trained models evaluated, Xception was identified as 
the most suitable for our dataset. Additionally, unfreezing the last 5 blocks of Xception has yielded the best 
results. 3. The integration of Xception with CBAM, where the last 5 blocks of Xception are unfrozen, represents 
a novel approach. This allows the model to concentrate on relevant regions within input images, thereby 
enhancing its ability to discern intricate patterns and relationships. Table 1 describes the classification report 
which provides key metrics (precision, Recall, and F1 score) to evaluate the performance of our classification 
model. We’ve allocated unique numerical mappings to each snake species for classification purposes. For 
instance, BLACK HEADED ROYAL SNAKE NON-VENOUMOUS corresponds to class 0, while COBRA 
VENOUMOUS is associated with class 1 and so on. The model achieves an outstanding validation accuracy of 
86%, surpassing the state-of-the-art models listed in Table 2. This outcome underscores the efficacy of 
employing attention mechanisms in deep learning models for intricate classification tasks, such as distinguishing 
between diverse snake species. As our research contributes to the broader field of wildlife conservation and 
public safety, the findings pave the way for enhanced snake identification systems, facilitating timely and 
accurate responses in snake-related emergencies. Despite the notable success achieved, future endeavors could 
explore further optimizations and refinements to elevate the model’s performance, ensuring its robustness across 
various environmental conditions and species variations.   
