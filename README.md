# Worker Safety Detection using YOLOv8

## Introduction
This repository houses a YOLOv8 classification model tailored to bolster worker safety at construction sites. The model's primary function is to detect and classify the presence of essential safety gear, including hardhats, safety vests, nose masks, and goggles, worn by workers.

## Features
- **YOLOv8 Architecture**: Employs the YOLOv8 architecture renowned for its precision and efficiency in object detection tasks.
- **Real-time Detection**: Capable of instantaneous detection, enabling swift response to safety violations.
- **Multi-class Classification**: Provides multi-class classification to identify various safety gear items worn by workers.
- **Customizable Configurations**: Offers flexibility in configurations for seamless integration into diverse construction site environments.
- **Integration Compatibility**: Supports integration with existing safety monitoring systems for enhanced functionality.

## Advantages
1. **Enhanced Safety**: Accurately detects compliance with safety regulations, thereby mitigating the risk of accidents and injuries.
2. **Operational Efficiency**: Real-time detection facilitates prompt intervention, improving overall site safety and productivity.
3. **Cost-effectiveness**: Automates safety monitoring tasks, reducing the need for manual inspections and associated costs.
4. **Scalability**: Adaptable to construction sites of varying sizes and complexities, ensuring scalability and versatility.
5. **Compliance Assurance**: Ensures adherence to safety standards and regulations, safeguarding against legal and reputational risks.

## Installation
To use this model, follow these steps:
1. Clone the repository: `git clone https://github.com/EugeneDenteh/Worker_Safety_Detection_Using_YoloV8.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Place the `best.pt` file in the root directory of the repository. This can be found here (https://drive.google.com/file/d/116nVZJDYAmUJ9IfP0jJJIu_RPOZ8O6w6/view?usp=drive_link)
4. Run the detection script.

## Usage
```python
from worker_safety_detection import YOLOv8WorkerSafetyDetector

# Initialize detector
detector = YOLOv8WorkerSafetyDetector()

# Load image or video
image = "path/to/image.jpg"

# Detect worker safety
results = detector.detect(image)

# Process results
for result in results:
    print(result)
