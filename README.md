# 🩻 DicoVision: DICOM Explorer

**DicoVision** is an intuitive and interactive application for loading, visualizing, and exploring DICOM medical images. Built with **PyQt5**, **pydicom**, and **NumPy**, the viewer supports rich metadata interaction, anonymization, and 3D tiled visualization of DICOM slices.

---

## 📦 Features

### 🖼️ Image Viewer
- **Load and display DICOM images**
  - Supports both **single-frame** and **multi-frame (M2D)** DICOM files.
- **Play DICOM videos**
  - Multi-frame files are played as videos with adjustable playback speed.
- **Error Handling**
  - Displays user-friendly messages for unsupported or invalid files.

### 🧠 Metadata Viewer
- **Explore Metadata**
  - Displays DICOM tags, patient details, pixel data, study info, modality, and physician information.
- **Search Functionality**
  - Search for specific DICOM tags or keywords.
- **Anonymization Tool**
  - Easily anonymize sensitive fields (e.g., patient name, ID) using a custom prefix.

### 🧱 3D Viewer
- **3D Tiled Visualization**
  - Displays DICOM slices in a tiled layout for better spatial understanding.
- **Zoom Controls**
  - Zoom in and out of specific regions for enhanced analysis.

---

## 🗂️ File Content

### 📘 Main Class
- `DicomViewer`: Implements the GUI and all core functionalities.

### 🔧 Key Functions

#### 🖼️ Image Loading and Display
- `load_dicom_file()`:
  - Loads a DICOM file and initializes the image and metadata.
- `display_image()`:
  - Displays static images or plays video if multi-frame.
- `stop_video()`:
  - Stops video playback.
- `play_m2d_video()`:
  - Plays multi-frame (M2D) DICOM files as looping videos.
- `display_2d_image(pixel_array)`:
  - Normalizes pixel values and prepares for display.

#### 🧠 Metadata Handling
- `display_dicom_tags()`:
  - Shows all DICOM metadata in a tabular format.
- `display_patient_info()`:
  - Displays patient-specific information.
- `anonymize_dicom()`:
  - Anonymizes personal data with a given prefix.

#### 🧱 3D Viewer
- `display_3d_tiles()`:
  - Renders 3D DICOM slices in a grid.
- `eventFilter()`:
  - Adjusts tile quality during zoom interactions.

---

## 🚀 Getting Started
