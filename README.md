# AI Photo Editing With Inpainting

# Project drscription
- App Functionality: The app enables users to either select a subject from an image and change its background or keep the background and change the subject. 
- Image Upload and Selection: Users start by uploading an image and selecting the main object by clicking on it. The app then uses the Segment Anything Model (SAM) to create a precise mask around the selected object, selecting the most accurate mask generated.
- Mask Refinement: Users are shown the initial mask result and can either accept it or refine it further by clicking additional points on the image. This step ensures high accuracy in masking the desired object.
- Background Substitution: Once the mask is finalized, users can provide a text description (and possibly a negative prompt) to specify a new background for the selected object. An infill model generates this new background, and the final image is displayed. Alternatively, users can choose to invert the mask to substitute the subject while keeping the background intact.
- Versatile Uses: The app can be utilized for various tasks such as swapping backgrounds, swapping subjects, removing objects, and more, providing users with a wide range of creative possibilities.

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
## Testing

Explain the steps needed to run any automated tests

### Break Down Tests

Explain what each test does and why

```
Examples here
```

## Project Instructions

This section should contain all the student deliverables for this project.

## Built With

* [Item1](www.item1.com) - Description of item
* [Item2](www.item2.com) - Description of item
* [Item3](www.item3.com) - Description of item

Include all items used to build project.

## License

[License](LICENSE.txt)
