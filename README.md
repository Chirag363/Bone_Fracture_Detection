
# 🦴 Radiographic Fracture Detection: Evaluating Severity through X-ray Analysis

**Bone_Fracture_Detection** is a Python-based AI system that assists in detecting and annotating bone fractures in radiographic (X-ray) images. Designed with modularity and usability in mind, it helps streamline medical diagnostics by providing accurate predictions and generating automated PDF reports—all accessible via a clean web interface.

---

## 🚀 Key Features

- 🔍 **AI-powered Fracture Detection** using deep learning models
- 🖼️ **Visual Annotation** of fracture regions on uploaded X-ray images
- 📄 **PDF Report Generation** with severity classification
- ☁️ **Cloudinary Integration** for optimized image storage
- 🐳 **Docker Support** for easy deployment across systems
- 🧪 **Self-contained Test Scripts** for Cloudinary and PDF generation validation

---

## 📁 Folder Structure

```bash
Bone_Fracture_Detection/
│
├── annotated_images/          # Stores AI-annotated X-ray images
├── app/                       # Core logic and application layer
├── uploads/                   # Folder for user-uploaded X-ray images
├── mnt/data/                  # (If mounted) Stores datasets/model files
├── test_cloudinary_integration.py  # Cloudinary storage test script
├── test_pdf_generation.py     # PDF output test script
├── temp_report.pdf            # Example generated PDF report
├── requirements.txt           # Python dependencies
├── Dockerfile                 # Docker configuration for deployment
└── run.py                     # Main execution script
```

---

## ⚙️ Getting Started

### ✅ Prerequisites

- Python ≥ 3.8
- `pip` for package management
- (Optional) Docker for containerized setup

### 🧪 Installation (Local)

1. Clone the repository:
   ```bash
   git clone https://github.com/Gatt101/Bone_Fracture_Detection.git
   cd Bone_Fracture_Detection
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the app locally:
   ```bash
   python run.py
   ```

### 🐳 Installation (Docker)

1. Build and run:
   ```bash
   docker build -t bone_fracture_detection .
   docker run -p 5000:5000 bone_fracture_detection
   ```

---

## 🧠 How It Works

1. Upload an X-ray image via the frontend or place it inside the `uploads/` directory.
2. The backend AI model processes the image to detect fracture regions.
3. Annotated images are saved in the `annotated_images/` folder.
4. A PDF report is generated detailing severity and predictions.

---

## 🧪 Testing Utilities

- ✅ `test_cloudinary_integration.py`: Verifies image upload and delivery via Cloudinary.
- ✅ `test_pdf_generation.py`: Tests automatic PDF generation for diagnostic reports.

---

## 👥 Team Contributions

- **Gaurav Patil**: Project lead, model integration, PDF generation, deployment.
- **Chirag Patil**: Frontend development, UI enhancements, deployment coordination.
- **Prathamesh Patil & Tanvi Prabhudesai**: Documentation, research assistance.

---

## 📜 License

⚠️ *This project currently does not have an open license. Please contact [@Gatt101](https://github.com/Gatt101) for permission to use or adapt the code.*

---

## 🙏 Acknowledgements

- YOLOv8 for fracture detection reference [📄 arXiv]
- Medical LLM dataset: [`Mohammed-Altaf/medical-instruction-120k`](https://huggingface.co/datasets/Mohammed-Altaf/medical-instruction-120k)
- Comparative study: [AI vs Radiologists – jbsr.be](https://www.jbsr.be/)
- Flask, Cloudinary, and PyMuPDF for backend logic and media generation

---

## 🔗 Live Demo

🖥️ Try the application here:  
**[Live App](https://orthopedic-agent.vercel.app/)**  
📂 Explore the source code:  
**[GitHub Repo](https://github.com/Gatt101/Bone_Fracture_Detection)**

---

> _"Radiographic AI is not just about predictions—it’s about empowering radiologists with faster insights and better patient outcomes."_
