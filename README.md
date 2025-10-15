# Video Mosaic App

A C++/QML desktop application for synchronizing multiple video files and tabular data (CSV/XLSX) to generate a composite video mosaic for technical analysis.

---

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

![Main Workspace](assets/02_main_workspace.png)
*(**Tvoj zadatak:** Postavi sliku `main.qml` koja prikazuje sve učitane klipove u gridu i na timeline-u)*

---

### 3. Interactive Synchronization & Analysis

The core task is achieving precise temporal alignment. The application offers several powerful tools for this:

-   **Drag & Drop:** Clips can be moved directly on the timeline by dragging them with the mouse.
-   **Numerical Offset:** For fine-tuning, the time offset for each clip can be entered numerically.
-   **Zoom View:** For critical synchronization points, the user can open a dedicated **Zoom View**. This window displays a selected video stream in high resolution, making it easy to spot subtle details and fast-moving events.

![Synchronization in Action](assets/03_sync_and_zoom.png)
*(**Tvoj zadatak:** Postavi sliku koja prikazuje pomjeren klip na timeline-u, sa otvorenim `ZoomView` prozorom iznad)*

---

### 4. Exporting the Final Video Mosaic

Once synchronization is complete, the final step is to generate the video mosaic. The Export Window offers a range of options to customize the final output.

-   **Pre-defined Layouts:** Choose from standard layouts like a grid.
-   **Custom Layout Mode:** Users have complete creative control, allowing them to define the exact X/Y position and width for each video stream. A live preview of the layout is shown instantly.
-   **Layout Management:** Custom layouts can be saved to a text file and reloaded later, streamlining work on similar projects.
-   **Time Overlay:** An optional digital clock can be burned into the final video, displaying the elapsed time in milliseconds.

![Export Window](assets/04_export_window.png)
*(**Tvoj zadatak:** Postavi sliku `ExportWindow.qml` sa odabranim "Custom" layoutom, gdje se vide X,Y,W polja i preview)*

---

### 5. Example Outputs

The flexibility of the layout system allows for the creation of both uniform and complex visual displays, tailored to the specific needs of the analysis.

![Example Outputs](assets/05_final_renders.png)
*(**Tvoj zadatak:** Napravi kompozitnu sliku koja prikazuje dva primjera finalnog videa, npr. jedan sa Grid layoutom i jedan sa Custom layoutom, jedan pored drugog)*

---

## Technology Stack

-   **Framework:** [Qt 6](https://www.qt.io/)
-   **Languages:** C++, QML
-   **Core Libraries:**
    -   [OpenCV](https://opencv.org/): For all backend video processing tasks.
    -   [QXlsx](https://github.com/QtExcel/QXlsx): For parsing Microsoft Excel (`.xlsx`) data files.
    -   [QCustomPlot](https://www.qcustomplot.com/): For rendering scientific charts and generating hodogram visuals.

## Source Code Access

The source code for this project is private. If you are a potential employer, academic collaborator, or have a genuine interest in the technical implementation of this project, I would be happy to provide access to the source code upon request.

## Contact

Maid Nezović - **maid.nezovic@email.com**
