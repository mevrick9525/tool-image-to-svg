# Tool: Image to SVG Converter

This Python tool converts raster images (PNG, JPG, JPEG) in the current folder into black & white SVG vector files using OpenCV and Potrace.

---

## Prerequisites

1. Python 3.x installed
2. OpenCV Python package: install with
   ```bash
   pip install opencv-python
   ```
3. Potrace download:
   - Extract the folder and note the full path to `potrace.exe`

---

## Setup

1. Place all images you want to convert in the **same folder** as the Python script (`main.py`).
2. Update the `potrace_path` variable in `main.py` with the full path to your Potrace executable. Example:

```python
potrace_path = r"C:\Users\YourName\Downloads\potrace.exe"
```

---

## Running the Script

In the terminal / command prompt, run:

```bash
python main.py
```

or if your system uses `python3`:

```bash
python3 main.py
```

---

## Output

- Converted SVG files will appear in the folder: `svg_vector_output`
- Temporary PBM files are automatically created and deleted.
- Supported image formats: .png, .jpg, .jpeg

---

## Notes

- `os` and `subprocess` are built-in Python modules; no installation required.
- `cv2` (OpenCV) must be installed separately as shown above.
- Make sure the script, images, and Potrace executable are accessible in the system path you provide.

---
