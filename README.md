# Mamiya_etal_2023_Proprioceptor_selectivity_topographic_maps_Analysis_code

### Analysis code for data presented in Mamiya et al. (2023) "Origins of proprioceptor feature selectivity and topographic maps in the Drosophila leg" Neuron

## Brief description of the notebook/class
---
### Preprocessing_for_all_types_and_piezo_analysis_summary_20220927.ipynb
**Jupyter notebook containing the class and parameters for preprocessing all two-photon imaging data.**
* Read two-photon imaging data acquired by ScanImage, demultiplex the channels, filter and register images, align two-photon images with high-speed video images.
* Shows analyses examples.
---
### Tibia_tracking_20220921.ipynb
**Jupyter notebook containing the class, functions, and parameters for tracking the tibia in high-speed video images.**
* Read high-speed video images, detect tibia in the region of interest, track the tibia angle, and calculate the average tibia angle for each two-photon imaging frame.
* Shows analyses examples.
---
### Cell_tracking_20200920_v2.ipynb
**Jupyter notebook containg the class, functions, and parameters for tracking the cells in the two-photon fast-z-stack images.**
* Make z-projected image and use marker based watershed segmentation to segment cells. Then use the centroid of the previous frame's segmenation as a marker for the segment in the next frame. Initialize the cell segmentations from different starting frame and move forward/backwards to make multiple segmentations. Use the segmentations that is robust to the initial frame and movement direction.  
* Shows analyses examples. 
---
### Calculating_DRR_and_cell_movements_20220921.ipynb
**Jupyter notebook containing the functions and parameters for calculating the DR/R, based on the cell segmentation data and the fluorescence from tdTomato and GCaMP7.**
* Based on the cell segmentation data, calculate DR/R and show the activity vs position, activity vs tibia angle, etc.
* Shows analysis examples.
