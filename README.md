# Image-Text-Image

The Image-Text-Image Architecture is a powerful paradigm for manipulating and generating visual content based on textual descriptions. It creates a cyclical relationship: first, analyzing an input image to generate a textual description (Image to Text); then, allowing this text to be modified (Text Manipulation/Modification); and finally, using the modified text to generate a new image (Text to Image).
The project involved setting up an environment with key Python libraries like EasyOCR, PyTorch, transformers, and diffusers, requiring sufficient disk space and preferably a GPU. A crucial step was extracting text from images using EasyOCR's optical character recognition capabilities.

To generate textual descriptions from images, I implemented three pretrained image captioning models: Salesforce's BLIP, the ViT-GPT2 model, and Microsoft's GIT model trained on the COCO dataset. Each model offers different strengths in generating natural language descriptions.The project also includes a Visual Question Answering component using the BLIP VQA model for interactive image analysis through natural language queries.
To handle large-scale data, I integrated the COCO dataset with a custom COCODataset class and DataLoader for efficient processing.Completing the cycle, I explored two text-to-image generation approaches: Google's Imagen and Stability AI's Stable Diffusion model, both allowing for new image generation from textual input.

The project culminates in an end-to-end pipeline chaining these components: from initial image text extraction and captioning to generating new images based on modified text. The modular design allows for model experimentation, and I've included examples demonstrating the pipeline's effectiveness on various images.
My work on this project has reinforced my understanding that these AI tools augment creators with new capabilities, expanding the horizons of visual content generation. Understanding the underlying technology and practical building steps was key to successfully undertaking this project and harnessing its full potential.

Colab: https://colab.research.google.com/drive/1hut1bw0HYohpkfKerbCQsgrjmnY9cHqi?usp=sharing
