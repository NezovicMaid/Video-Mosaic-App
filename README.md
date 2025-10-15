# Video Mosaic App

A C++/QML desktop application for synchronizing multiple video files and tabular data (CSV/XLSX) to generate a composite video mosaic for technical analysis.

---

![Video Mosaic App Showcase](assets/showcase.gif)
*(**Napomena za tebe:** Snimi kratak GIF (5-10 sekundi) koji prikazuje rad aplikacije – pomjeranje klipova na timeline-u, otvaranje zoom prozora, itd. Postavi ga u `assets` folder i provjeri da li je putanja ispravna. Ovo je **jako** važno za prvi utisak!)*

## About The Project

In modern engineering and scientific analysis, understanding high-speed, complex events often requires recording a scene from multiple angles. However, the true value of such multi-camera footage is only unlocked through **precise temporal synchronization**. Without it, correlating events between different streams becomes impossible.

Furthermore, commercial video editing software (like Adobe Premiere Pro or DaVinci Resolve) is primarily designed for creative and cinematic purposes. These tools lack the specialized features needed for technical analysis, particularly the ability to integrate and synchronize numerical sensor data with visual footage.

**Video Mosaic App** was built to bridge this gap. It is a specialized desktop tool designed from the ground up for engineers, researchers, and technicians. It provides an intuitive workflow not only for synchronizing multiple video files but also for converting tabular data from sensors into a dynamic video representation (**hodogram**), which can then be synchronized alongside the other video streams.

## Key Features

-   **Multi-Source Processing:** Simultaneously load and process multiple independent video files and tabular data files (`.csv`, `.xlsx`).

-   **Interactive Timeline:** A powerful and intuitive timeline for frame-level manual synchronization. Users can drag-and-drop video clips or input numerical offsets for precise alignment.

-   **Advanced Hodogram Generation:** A unique module that automatically converts numerical data into a video representation of a graph. It supports two critical data formats:
    -   **Time-based data:** Plots signal values over time, automatically normalizing time units (s, ms, µs).
    -   **Frame-based data:** Creates an X-Y plot for visualizing positional data or trajectories, where each row of data corresponds to a single video frame.

-   **High-Performance Proxy Workflow:** To ensure a fluid user experience even with high-resolution videos (e.g., 4K), the application automatically generates low-resolution "proxy" versions for editing. The original high-quality files are used only for the final rendering.

-   **Customizable Video Mosaic:** Generate a final composite video with flexible layout options:
    -   Pre-defined layouts (e.g., Grid, Main + Thumbnails).
    -   A fully **Custom Layout** mode where the user can define the exact X/Y position and width for each video stream.

-   **Layout Management:** Save and load custom layout configurations to a text file, significantly speeding up work on similar projects.

-   **Precision Tools:**
    -   **Zoom View:** A dedicated window for a high-resolution, magnified view of a selected video stream, perfect for identifying key synchronization points.
    -   **Time Overlay:** An optional digital clock can be burned into the final video, displaying the elapsed time in milliseconds for precise analysis.

## Technology Stack

The application is built using a hybrid C++/QML model to leverage the strengths of each technology.

-   **Framework:** [Qt 6](https://www.qt.io/)
-   **Languages:** C++, QML
-   **Core Libraries:**
    -   [OpenCV](https://opencv.org/): For all backend video processing tasks, including decoding, encoding, and frame manipulation.
    -   [QXlsx](https://github.com/QtExcel/QXlsx): For robust parsing of Microsoft Excel (`.xlsx`) data files.
    -   [QCustomPlot](https://www.qcustomplot.com/): For rendering scientific charts and generating hodogram visuals.

## Source Code Access

The source code for this project is private and not publicly available in this repository. This decision was made to protect the intellectual property and potential for future commercial or academic development.

If you are a potential employer, academic collaborator, or have a genuine interest in the technical implementation of this project, I would be happy to provide access to the source code upon request.

## Contact

Maid Nezović - **mnezovic1@gmail.com**

Project Link: [https://github.com/NezovicMaid/Video-Mosaic-App](https://github.com/NezovicMaid/Video-Mosaic-App)
