# 🩻 DicoVision: DICOM Explorer

![DicoVision Logo](https://github.com/Kareem-Taha-05/DicoVision/blob/main/Logo%20and%20Illustrative%20visuals/Logo/DicoVision%20Logo.jpeg)

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

### 1. 📥 Install Dependencies

Make sure you have Python 3.8 or above installed. Then run:
    ``` 
    pip install -r requirements.txt
    ```
### 2. 🏁 Launch the Application
    ``` 
    python Task4.py 
    ```

---

## 🧭 How to Use

### 🖼️ Image Viewer Tab
- Load DICOM images from your system.
- Supports both static and animated DICOM formats (multi-frame).

### 🧬 Metadata Viewer Tab
- Explore full DICOM metadata.
- Search and anonymize fields with one click.

### 🧱 3D Viewer Tab
- Visualize stacks of DICOM slices in a tile grid.
- Zoom in/out to focus on specific areas.

### ⚠️ Error Handling
- Selecting invalid files/folders prompts a clean error message.
- No crashes—just smooth user experience.

---

## 📸 Screenshots

![Image](https://github.com/user-attachments/assets/ad3e585e-7e48-4332-bc1d-c18c357c0e79)  
![Image](https://github.com/user-attachments/assets/a1686fa3-6620-4132-b182-fb643e130fc3)  
![Image](https://github.com/user-attachments/assets/64925f23-379e-40f4-af7c-1613fd3b7dfd)  
![Image](https://github.com/user-attachments/assets/9cf5170a-fb1d-458b-a091-30d758540de2)  
![Image](https://github.com/user-attachments/assets/073f8bb3-c159-4a62-8735-571cfd487a72)  
![Image](https://github.com/user-attachments/assets/eb18211b-25c8-460b-a352-6b9423ea1279)

---

## 🎥 Demo Video

👉 [Watch Demo Video](https://github.com/user-attachments/assets/93210dcb-44cd-4bd6-a2e9-d3d591be0d9d)

---

## 📄 License

This project is licensed under the **[MIT License](../LICENSE.txt)**.

---

# Contributors
1. [Kareem Taha](https://github.com/Kareem-Taha-05)
2. [Omar Gamal](https://github.com/OmarGamalH)
3. [Kareem Hassan](https://github.com/karimhassan-808)
4. [Omar Amein](https://github.com/OmarAmein)

---

## 💬 Feedback & Contributions

Contributions, issues, and feature requests are welcome! Feel free to open an issue or pull request on GitHub.

---
