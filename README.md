![Object Detection in Images and Video](assets/banner.svg)

> Finds and labels everyday objects, from people to bicycles, in both images and video.

**Training project · IoT & Computer Vision track**  
**Tools:** Python, OpenCV DNN, NumPy, Matplotlib

## The challenge

The same detection model should work on still images and on moving video, and show results clearly in both.

## The data

Pretrained on the COCO classes. Tested on a sample image and a sample video.

## How it works

![How it works](assets/pipeline.svg)

1. Loaded a pretrained model trained on the COCO classes through OpenCV.
2. Ran it on a test image, then frame by frame on video.
3. Drew boxes and labels, measured frames per second, and saved the output video.

## A closer look

- **Model:** a pretrained detector loaded through OpenCV's deep learning module.
- **Images:** one pass, with boxes and labels drawn on the result.
- **Video:** frame-by-frame detection with a live speed counter, saved to a new video.

## Key decisions

- Using one pipeline for images and video keeps behavior consistent between them.

## Results

| Measure | Result |
|---|---|
| Classes | **COCO** |
| Speed on the test machine | **About 2 frames per second** |
| Input | **Image and video** |

## Programming skills

- Python programming
- Running pretrained models with OpenCV DNN
- Image and video input and output
- Filtering detections by confidence
- Measuring frames per second
- Drawing boxes and labels

## Good to know

- The speed comes from one test run on CPU. No detection accuracy score was recorded.

## What I would do next

- Compare faster models, to go beyond 2 frames per second.
- Measure accuracy on a labelled set.

<details dir="rtl"><summary><strong>بالعربي: كشف الأجسام في الصور والفيديو</strong></summary>

يجد الأجسام اليومية ويسميها في الصور والفيديو بنموذج جاهز على فئات COCO.

**ملاحظة:** السرعة نحو إطارين في الثانية من تجربة واحدة، ولا توجد درجة دقة مسجلة.

**المهارات البرمجية:** Python programming، Running pretrained models with OpenCV DNN، Image and video input and output، Filtering detections by confidence، Measuring frames per second، Drawing boxes and labels.

الكود خاص، وهذه الصفحة تعرض فكرة المشروع وطريقة عمله ونتائجه.

</details>


---

**About the source code:** the code for this project is private. This page presents what it does, how it works, and its results. To talk about the work, contact me through my [GitHub profile](https://github.com/SamerAlTaki97).
