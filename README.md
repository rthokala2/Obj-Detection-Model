# Obj-Detection-Model

📊 Object Detection Model Evaluation Report

Model: SSD300 with VGG16 Backbone

* Pre-trained Weights: torchvision.models.detection.ssd300\_vgg16
* Dataset: Pascal VOC 2007 (Validation set)
* Evaluation Framework: torchmetrics.detection.MeanAveragePrecision
* Sample Size: 20 images (limited for low-memory environments)

## Evaluation Metrics

* mAP: 0.0000
* Precision: -1.0000
* Recall: 0.0000

Note: Results are based on a limited evaluation subset to ensure compatibility with low-memory systems.
Full dataset evaluation may show improved metrics if detection works correctly.

✍️ Experience Report

🌟 What I Did

* Implemented an object detection pipeline using SSD300 with VGG16 backbone.
* Used Pascal VOC 2007 validation split for evaluation.
* Evaluated using MeanAveragePrecision from torchmetrics, limited samples due to constraints.

🚧 Challenges Faced

* Memory issues caused Colab kernel crashes; limited evaluation to 1 image at a time (20 total).
* Parsing Pascal VOC annotations from XML was difficult.
* Model inference returned no correct detections, resulting in zero scores.

🤖 Use of AI Tools

* Used ChatGPT for debugging memory issues, optimizing code, and drafting reports.
* Used AI to explore evaluation techniques with torchmetrics.

📘 What I Learned

* Structure of object detection pipelines using pre-trained models.
* Parsing Pascal VOC annotation format.
* Calculating mAP, precision, recall with torchmetrics.

😲 What Surprised Me

* Evaluation metrics are sensitive to label mismatches or missing detections.
* Pre-trained models can fail without proper preprocessing/label alignment.

🤝 Coding & AI Balance

* AI used for low-level bug fixes and optimization.
* Manual control of architecture, data parsing, and evaluation logic.

💡 Suggestions to Improve Assignment

* Recommend small backbones (e.g., MobileNet) for low-resource systems.
* Provide sample annotation parsers.
* Allow simplified datasets for first evaluations.
* Add label mapping tips to avoid zero-score confusion.

Prepared by: Rohith Thokala
For: Object Detection Internship Assignment – Final Submission
