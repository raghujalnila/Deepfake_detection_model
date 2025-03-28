# DeepFake Face Detection Using InceptionV3
 
![sample_image](https://github.com/user-attachments/assets/9b9422a4-a29c-4998-b7d9-9b5dff6a03bd)
## Project Overview
In an era of rapidly advancing AI-generated imagery, distinguishing between real and fake faces has become increasingly critical. I developed this project using InceptionV3 to detect deepfake and AI-generated faces with remarkable precision.
By creating a sophisticated deep learning model, I aimed to address the growing challenges of digital identity verification and misinformation spread through synthetic imagery. The model meticulously analyzes visual characteristics, uncovering subtle artifacts that reveal an image's synthetic origin.
My solution provides a powerful mechanism to verify the authenticity of facial images in an increasingly complex digital landscape, offering a crucial tool for researchers and cybersecurity professionals.

## Project Structure

- **Deepfake_Detection_Model/**
  - 📄 `app.py`
  - 📄 `binary_classification_inception_model.pth`
  - 📄 `inceptionnet_model.ipynb`
  - 📄 `README.md`
  - 📄 `requirements.txt`
  - **static/**
    - 🖼️ `background.jpg`
  - **templates/**
    - 📝 `index.html`

## Quick Start Guide
### 1. Clone the Repository
git clone https://github.com/yourusername/fake-face-detector.git
cd fake-face-detector

### 2. Create a Virtual Environment (Recommended)
#### On Windows
python -m venv venv
venv\Scripts\activate
#### On macOS/Linux
python3 -m venv venv
source venv/bin/activate

### 3. Install Dependencies
pip install -r requirements.txt

### 4. Download Pre-trained Model (If not included)
Ensure model.pth is in the project root directory
If missing, you may need to train the model using the model.ipynb notebook

### 5. Run the Application
python app.py

### 6. Access the Web Interface
Open a web browser and navigate to:
'http://localhost:5000'

### 7. Using the Fake Face Detector
Click on "Upload Image"
Select an image file
Click "Detect"
View the results (Real or Fake face detection)

## User Interface :
![Screenshot 2025-03-28 141818](https://github.com/user-attachments/assets/e7c0c685-0b67-447f-bf98-55ac9fbe7f6f)

## Performance Metrics & Model Journey
   ### Accuracy Highlights
   
   **Final Accuracy**: 98.33%
   
   **Model Evolution**: Initially used ResNet-18 but switched to InceptionV3 after recognizing its superior feature extraction capabilities.  
                        This transition improved model performance and accuracy.
  ### Training Insights
  **Initial Challenge**: Significant overfitting in early iterations
  
   **Solution**: Comprehensive dataset refinement and diverse image augmentation
      
  **Breakthrough**: Achieved robust generalization through strategic data integration
 ![inception loss model](https://github.com/user-attachments/assets/bcc79576-8049-497c-81c3-44f39688c862)
 
### Detection Capabilities
  **Strong Performance**: Excellent at detecting synthetic images from:
                         - "This Person Doesn't Exist"
                          - DALL·E generated faces
                          - Various StyleGAN outputs
                          
### Current Limitations
                          
  **Challenge**: Limited detection of ChatGPT-generated images due to dataset constraints
    
  **Future Goal**: Expand training data to improve detection of emerging AI image generation techniques

  ## License
  This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.










