# Consistent Character Video Generation

This repository demonstrates how to generate videos with a consistent character using fine-tuned diffusion models and ComfyUI. The process involves training a LoRA version of the Hunyuan model and leveraging ComfyUI for text-to-video and video-to-video generation.

## Features
- **LoRA Fine-Tuning**: Train a LoRA-adapted Hunyuan model for a specific character.
- **Text-to-Video**: Generate videos from text prompts.
- **Video-to-Video**: Convert an existing video while maintaining character consistency.

## Workflow

### 1. Training LoRA for Hunyuan
To ensure the model learns a specific character, follow these steps:

1. **Collect Images**: Gather a diverse set of images of the character in various poses and emotions.
2. **Prepare Prompts**: Write text prompts for each image. Keep the prompt minimal, using a single long word to avoid confusion during training.
3. **Train Using Diffusion-Pipe**: Utilize the repository [tdrussell/diffusion-pipe](https://github.com/tdrussell/diffusion-pipe) to fine-tune the model.

### 2. Video Generation with ComfyUI
Once training is complete, use ComfyUI to generate videos:

- **Text-to-Video**: Generate a video directly from a text prompt.
- **Video-to-Video**: Transform an existing video while maintaining the trained character's consistency.

The configurations required for these tasks are available in the `workflows/` folder.

## Dependencies
- [tdrussell/diffusion-pipe](https://github.com/tdrussell/diffusion-pipe) for training.
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) for video generation.

## Installation & Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/consistent-character-video.git
   cd consistent-character-video
   ```
2. Follow the instructions in `diffusion-pipe` to train the LoRA model.
3. Use the provided ComfyUI workflows for text-to-video and video-to-video generation.

## Example Results
(Include sample images or links to generated videos)

## Acknowledgements
- [tdrussell/diffusion-pipe](https://github.com/tdrussell/diffusion-pipe)
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI)

## License
Specify your preferred license here (e.g., MIT, Apache 2.0, etc.).

