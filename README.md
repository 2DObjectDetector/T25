# T2.5 EigenCAM interpretability

Uses EigenCAM to generate heatmaps from two layers of the best fine-tuned YOLO model, showing which image regions influence its detections. Part of [2D Object Detector](https://github.com/2DObjectDetector).

**Layers used:** layer 4 (early backbone, frozen during fine-tuning) and layer 21 (deeper, adapted during fine-tuning). Neither heatmap highlighted the detected objects: layer 4 fired on edges and shadows, layer 21 on broad background regions, suggesting localisation comes from several layers working together rather than one.

**Run:** Outputs are saved in the notebook, so the results are visible without running it. To rerun: use a Colab GPU runtime and add the `kitti3k_yolo` dataset (not included) and update its path.
