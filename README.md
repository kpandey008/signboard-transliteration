The code organization is WIP at the moment. Will update the repo after it is ready to be checked in.

# Signboard transliteration
A project to perform transliteration on commercial signboard images.

The project involves 3 stages:

1) Text Detection: To detect text regions in signboard images
2) Text Recognition: To decipher the hindi text in the regions detected in Step 1
3) Text transliteration: To convert the hindi text recognized in Step2 to English.

The project contains 4 ipython notebooks written in PyTorch. The notebooks can be described as follows:

1) `proj_station_detection_preprocess.ipynb`: Used to correct bounding box annotations provided by the dataset. This is a preprocessing step before the object detection step.

1) `proj_station_detection_od.ipynb`: Used to finetune a Faster-RCNN model to detect text regions in Signboard images

1) `project_station_td_preprocess.ipynb`: Used to tokenize the text labels provided in the Text Recognition dataset. This is a preprocessing step before the Text Recognition step.

1) `project_station_td_recognition.ipynb`: Used to train a Text Recognition systems using an encoder decoder model inspired by the paper `Show and Tell`.

1) Text Transliteration: [WIP]

## Author

Kushagra Pandey / @kpandey008