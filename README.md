# 🖼 Advanced Image WorkDesk  

An *all-in-one AI-powered image editing tool* built with *Streamlit, **Stable Diffusion, and **OpenCV*.  
This app combines classic computer vision techniques with modern generative AI, enabling users to edit, enhance, and generate stunning images effortlessly.  

---

## 🚀 Features  

- *Image Input Options*  
  - Upload from your device  
  - Capture with your camera  
  - Load from a URL  
  - Generate new images with *Stable Diffusion XL (Text-to-Image)*  

- *Editing Tools*  
  - Crop  
  - Background removal (via rembg)  
  - Mirror / Flip  
  - Convert to grayscale or black & white  
  - Rotate  
  - Adjust brightness, contrast, saturation, sharpness  
  - Compare original vs. processed images  
  - Download processed image  

- *AI-Powered Enhancements*  
  - Colorize black & white images  
  - Stable Diffusion XL Image-to-Image  
  - Stable Diffusion XL Inpainting (mask-based editing)  
  - Randomize effects  

---

## 🛠 Tech Stack  

- *Frontend & App*: Streamlit  
- *Image Editing*: Pillow, OpenCV, rembg  
- *Generative AI*: Diffusers (Stable Diffusion XL)  
- *Model Integration*: Hugging Face Inference API  
- *Deployment*: LocalTunnel / Streamlit  

---

## 📦 Installation  

Clone the repository and install dependencies:  

```bash
git clone https://github.com/ayushmohta7/Advanced-Image-WorkDesk.git
cd Advanced-Image-WorkDesk

# Install Python dependencies
pip install -r requirements.txt

# (Optional) Install LocalTunnel for sharing
npm install -g localtunnel
