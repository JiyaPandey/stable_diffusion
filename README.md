Here's your **README** file content. You can manually copy and paste it into a text file or a markdown file (`README.md`).  

---

# **Image Generation using Stable Diffusion & ComfyUI**  

## **Overview**  
This project explores AI-based image generation using **Stable Diffusion** integrated with **ComfyUI**. The goal is to leverage **Stable Diffusion’s text-to-image capabilities** within a node-based workflow for enhanced control over image synthesis. The project focuses on **custom prompts, negative prompts, model fine-tuning, and image enhancements** to generate high-quality AI artwork.  

## **Features**  
- **Text-to-Image Generation:** Create images based on text descriptions.  
- **Negative Prompting:** Exclude unwanted elements for refined outputs.  
- **ComfyUI Workflow:** A flexible, node-based interface for efficient model control.  
- **Seed Control:** Generate reproducible or randomized variations of images.  
- **Fine-Tuning Options:** Adjust parameters like **steps, CFG scale, and sampling methods** for optimal results.  
- **Checkpoint & VAE Support:** Load different models for diverse artistic styles.  

## **Installation**  

### **Prerequisites**  
Ensure you have the following installed:  
- **Python (3.8 or higher)**  
- **Git**  
- **Stable Diffusion Model (e.g., v1.5, v2.1, SDXL)**  
- **ComfyUI Framework**  
- **CUDA (if using GPU acceleration)**  

### **Steps**  

1. **Clone the ComfyUI Repository**  
   ```sh
   git clone https://github.com/comfyanonymous/ComfyUI.git
   cd ComfyUI
   ```  

2. **Install Dependencies**  
   ```sh
   pip install -r requirements.txt
   ```  

3. **Download and Place Stable Diffusion Model Checkpoints**  
   - Place `.ckpt` or `.safetensors` files in `ComfyUI/models/checkpoints/`  

4. **Run ComfyUI**  
   ```sh
   python main.py
   ```  
   - This starts a **local web interface** (default: `127.0.0.1:8188`).  

## **Usage**  
1. **Launch ComfyUI** and access the **workflow editor**.  
2. **Load a Stable Diffusion checkpoint**.  
3. **Configure CLIP text encoder nodes** to input prompts and negative prompts.  
4. **Adjust sampling settings** (steps, CFG scale, scheduler) for desired output quality.  
5. **Run the workflow** to generate and save images.  

## **Example Prompts**  

**Positive Prompt:**  
*A mystical sorcerer in a robe made of swirling galaxies*  

**Negative Prompt:**  
*no traditional wizard hats, medieval-style robes, or plain staffs, keeping the theme celestial and magical*  

**output :** 
![image](https://github.com/user-attachments/assets/a699ba2e-157e-495b-8ad8-839a22bf4635)




## **Troubleshooting**  
- **Black or Blank Images?**  
  - Increase sampling steps or use a different VAE model.  
- **Distorted Outputs?**  
  - Adjust CFG scale and refine prompts.  
- **Slow Processing?**  
  - Ensure GPU acceleration is enabled (check CUDA installation).  

## **Acknowledgments**  
- **Edunet AICTE & Edunet Foundation (IBM SkillsBuild)** for providing the learning platform.  
- **ComfyUI & Stable Diffusion open-source communities** for their extensive research and tools.  
