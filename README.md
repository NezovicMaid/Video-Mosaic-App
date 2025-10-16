# Video Mosaic App

A C++/QML desktop application for synchronizing multiple video files and tabular data (CSV/XLSX) to generate a composite video mosaic for technical analysis.

---
## Technology Stack

-   **Framework:** [Qt 6](https://www.qt.io/)
-   **Languages:** C++, QML
-   **Core Libraries:**
    -   [OpenCV](https://opencv.org/): For all backend video processing tasks.
    -   [QXlsx](https://github.com/QtExcel/QXlsx): For parsing Microsoft Excel (`.xlsx`) data files.
    -   [QCustomPlot](https://www.qcustomplot.com/): For rendering scientific charts and generating hodogram visuals.

## About The Project

In modern engineering and scientific analysis, understanding high-speed, complex events often requires recording a scene from multiple angles. However, the true value of such multi-camera footage is only unlocked through **precise temporal synchronization**. 

**Video Mosaic App** was built to bridge this gap. It is a specialized desktop tool designed for engineers and researchers, providing an intuitive workflow to not only synchronize multiple videos but also to convert sensor data into a dynamic video representation (**hodogram**) for a comprehensive, multi-modal analysis.

## Features Walkthrough

The application guides the user through a logical workflow, from project setup to the final export.

### 1. Project Setup & Configuration

The process begins in the Project Setup window. Here, the user defines all input sources and global parameters for the project.

-   **Load Videos:** Users can load multiple video files simultaneously. For each video, the acquisition period can be specified to ensure correct temporal resampling.
-   **Load Data Files:** The application supports loading tabular data from `.csv` and `.xlsx` files. For each file, the user specifies whether the first column represents **time** (with units s, ms, µs) or **frame number**, ensuring the data is interpreted correctly for hodogram generation.

![Project Setup Window](https://github.com/user-attachments/assets/00f135a7-3a0c-46fc-9bc9-bd1e87ae95f8)


### 2. Main Workspace: The Synchronization Hub

After configuration, the user enters the main workspace. The interface is split into two key areas: a video preview grid and an interactive timeline. The preview grid provides a simultaneous view of all video streams, while the timeline below is the central tool for synchronization.

![Main Workspace](https://github.com/user-attachments/assets/18bc3ca6-d5ca-45ed-b097-50edcb8f861c)


### 3. Interactive Synchronization & Analysis

The core task is achieving precise temporal alignment. The application offers several powerful tools for this:

-   **Drag & Drop:** Clips can be moved directly on the timeline by dragging them with the mouse.
-   **Numerical Offset:** For fine-tuning, the time offset for each clip can be entered numerically.
-   **Zoom View:** For critical synchronization points, the user can open a dedicated **Zoom View**. This window displays a selected video stream in high resolution, making it easy to spot subtle details and fast-moving events. The zoom window can be moved and resized by the user.

![Synchronization in Action](https://github.com/user-attachments/assets/85e0e235-29cb-44c1-a9d2-8e1cfc7e7a89)

### 4. Exporting the Final Video Mosaic

Once synchronization is complete, the final step is to generate the video mosaic. The Export Window offers a range of options to customize the final output.

-   **Pre-defined Layouts:** Choose from standard layouts like a grid.
-   **Custom Layout Mode:** Users have complete creative control, allowing them to define the exact X/Y position and width for each video stream. A live preview of the layout is shown instantly.
-   **Layout Management:** Custom layouts can be saved to a text file and reloaded later, streamlining work on similar projects.
-   **Time Overlay:** An optional digital clock can be burned into the final video, displaying the elapsed time in milliseconds.

![Export Window](https://github.com/user-attachments/assets/f6204fcf-fa16-4512-8d26-9581055e06dd)


### 5. Example Outputs

The flexibility of the layout system allows for the creation of both uniform and complex visual displays, tailored to the specific needs of the analysis.

![Example Output](https://github.com/user-attachments/assets/7cf72eeb-d3d4-4fbc-b17f-2434dcebf68d)

**For a demonstration of the final generated videos in motion, please see the examples at the following link:**
[**View Example Videos on Google Drive**](https://drive.google.com/drive/folders/1c-LTPQgP8VDiT4myTBIjfsBrCC_Kq4sB?usp=sharing)


## Source Code Access

The source code for this project is private. If you are a potential employer, academic collaborator, or have a genuine interest in the technical implementation of this project, I would be happy to provide access to the source code upon request.

## Contact

Maid Nezović - **mnezovic1@gmail.com**
