# AI Photo Editing With Inpainting

# Project drscription
- App Functionality: enables users to either select a subject from an image and change its background or keep the background and change the subject. 
- Image Upload and Selection: upload an image and select the main object by clicking on it. Apply Segment Anything Model (SAM) to create a precise mask around the selected object, selecting the most accurate mask generated.
- Mask Refinement: Users are shown the initial mask result and can either accept it or refine it further by clicking additional points on the image. 
- Background Substitution:when mask is finalized, users can provide a text description (and possibly a negative prompt) to specify a new background for the selected object. An infill model generates this new background, and the final image is displayed. Alternatively, users can choose to invert the mask to substitute the subject while keeping the background intact.
- Application: for various tasks like swapping backgrounds, swapping subjects, removing objects.

### Installation
1. Clone the project to your local machine
```
git clone https://github.com/hoangduchuy93/AI-photo-editing-with-inpainting.git
```
2. Create the env
```
python -m venv inpainting_project
source inpainting_project/bin/activate
```
3. Install below libraries to run the project
```
!pip install diffusers
!pip install gradio
!pip install accelerate
!pip install torch
!pip install transformers
```
4. Run the notebook
```
jupyter notebook
```

5. Follow the flow in notebook and open the public URL to try the app

### Result demo
Below is some results
1. The orginal Mona Lisa photo
- Prompt: the very royal queen with the crown on her head
- Negative prompt: artifacts, low quality, distortion
- Target: the subject of the photo (not the background)
![image](https://github.com/user-attachments/assets/71c13592-cfcd-4ccf-876b-9b90424d7f6c)

2. The original Mona Lisa photo
- Prompt: the girl in red gown in cartoon style
- Negative prompt: artifacts, low quality, distortion
- Target: the subject of the photo (not the background)
![image](https://github.com/user-attachments/assets/447679d7-7a46-414e-b681-9ecd7ef12b83)

3. The original a car photo
- Prompt: the car on the beach
- Negative prompt: artifacts, low quality, distortion
- Target: the background (not the subject of the photo)
![image](https://github.com/user-attachments/assets/818b11d9-6cae-4b02-a43a-1f9ffb71bf0a)


