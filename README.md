# Image Generation with Stable Diffusion and Gradio

This repository demonstrates how to generate images using the Stable Diffusion model and create a Gradio interface for user-friendly interaction.

## Prerequisites

- **GPU:** Ensure you have access to a GPU. If you're running this on Google Colab, select a GPU runtime (`Runtime > Change runtime type`).

## Configure GPU

1. Run the code snippet to check for a GPU. The code will fail if no GPU is found.

```python
# Check for a GPU
#todo fail if this fails
import os

if os.system('nvidia-smi'):
    raise Exception("No GPU found. Access a GPU through Runtime > Change runtime type and try again.")
