# ComfyUI Image Workflows

This repository contains a curated collection of ComfyUI workflows for image generation, image editing, reference-guided transformation, and image upscaling. The workflows are provided as `.json` files and can be imported directly into a ComfyUI environment, allowing users to test, adapt, and extend the pipelines for their own creative or research purposes.

The repository is organised into three main folders:

- `workflows/`  
  Contains the ComfyUI workflow files in `.json` format. These files can be loaded directly into ComfyUI and used as starting points for image generation, editing, or upscaling tasks.

- `screenshots/`  
  Contains screenshots of each workflow as displayed in the ComfyUI interface. These images provide a quick visual reference for the structure, node layout, and logic of each workflow.

- `examples/`  
  Contains example outputs generated using the workflows. These examples demonstrate the intended use cases and visual capabilities of each pipeline.

## Workflows

### HiDream O1 Image ComfyUI Image Editing Workflow

The HiDream O1 Image workflow is designed for prompt-guided image editing while preserving the overall composition of the source image. It is particularly useful for modifying portraits, product images, interiors, and visual design concepts where the original layout should remain stable. The workflow enables users to test alternative looks, restyle visual material, or adjust specific image attributes without rebuilding the entire scene from scratch. It provides a practical pipeline for controlled image-to-image experimentation in ComfyUI.

<img width="384" height="211" alt="hidream-o1-image-comfyui-image-editing-precision-reference-edit-workflow-1423-example_03" src="https://github.com/user-attachments/assets/70947412-a7ee-476a-a8a8-57cf0b50cbda" />


### JoyAI Image Edit

The JoyAI Image Edit workflow supports instruction-based editing from a single reference image. Users can provide a source image and a concise text instruction to modify colours, objects, spatial relationships, or other visual attributes while retaining the integrity of the original composition. This workflow is suitable for prompt-guided photo editing, product visualisation, concept refinement, and rapid design iteration. It is especially useful when users need controlled edits without manual masking.

<img width="384" height="211" alt="joyAI-example_04" src="https://github.com/user-attachments/assets/63954189-8bbc-44cf-8683-a5f199bce650" />


### LongCat Image Text-to-Image Workflow

The LongCat Image workflow is a compact text-to-image generation pipeline for creating square images from written prompts. It is designed around a straightforward prompt-to-image process, making it suitable for quick visual exploration, concept generation, portraits, product-style imagery, and editorial visuals. The default configuration is oriented towards 1024 × 1024 image generation, with parameters that can be adjusted for further quality or sampling control. Its simplicity makes it accessible as a starting point for users who want a focused text-to-image workflow in ComfyUI.

<img width="384" height="384" alt="longcat-example_02 (2)" src="https://github.com/user-attachments/assets/85f3d4e0-81f9-4de5-9bb4-df946b24029b" />


### Flux 2 Klein 9B KV Image Edit Workflow

The Flux 2 Klein 9B KV Image Edit workflow is intended for precise, instruction-led image editing using one or more reference images. It supports targeted transformations such as background replacement, style transfer, outfit or material transfer, and detail refinement while aiming to preserve subject identity, pose, and composition. The workflow uses reference conditioning to maintain visual consistency and is suitable for users who need higher levels of control in iterative editing tasks. It is particularly relevant for design workflows where prompt accuracy, reference fidelity, and repeatable visual exploration are important.

<img width="2048" height="2048" alt="flux-2-klein-inpaint" src="https://github.com/user-attachments/assets/0f6c8287-bbc8-4e45-86a1-f42943bef2ec" />


### 2.3 Creator: Image Upscale & Analysis

The 2.3 Creator workflow combines image upscaling with automatic image analysis. It enhances image resolution while also generating a descriptive prompt from the input image, making it useful for both visual improvement and metadata generation. The workflow uses image analysis to identify scene content, object attributes, spatial relationships, and contextual details, which can support downstream prompting or documentation. It is suitable for digital art, photography, media production, and workflows where both improved image quality and descriptive understanding of an image are required.

<img width="830" height="795" alt="creator 2 3-enhance" src="https://github.com/user-attachments/assets/0fbddbf6-6e49-4d10-b0f1-5c9ada500806" />


## How to Use

1. Open ComfyUI.
2. Drag and drop a `.json` file from the `workflows/` folder into the ComfyUI canvas, or load it through the ComfyUI interface.
3. Check that all required models, custom nodes, and dependencies are installed in your local ComfyUI environment.
4. Add or replace the input images and prompts where required.
5. Queue the workflow and review the generated output.
6. Compare your results with the files in the `examples/` folder where relevant.

## Notes

Some workflows may require specific models, custom nodes, or hardware resources to run successfully. If a workflow does not run immediately, check the missing-node or missing-model messages in ComfyUI and install the required components before retrying.

The workflows in this repository are intended as practical starting points. Users are encouraged to adapt prompts, seeds, model settings, sampling parameters, and node structures according to their own creative, technical, or research needs.

## Repository Structure

```text
ComfyUI-img-workflows/
│
├── workflows/
│   ├── HiDream O1 Image ComfyUI Image Editing Workflow.json
│   ├── JoyAI Image Edit.json
│   ├── LongCat Image Text to Image Workflow.json
│   ├── Flux 2 Klein 9B KV Image Edit Workflow.json
│   └── 2.3 Creator Image Upscale and Analysis.json
│
├── screenshots/
│   └── Screenshots of each workflow in ComfyUI
│
└── examples/
    └── Example outputs generated using the workflows
