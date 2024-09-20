# Image Description and Comparison Tool

This project provides a versatile tool for generating descriptions of images and comparing them using advanced AI models. It utilizes the BLIP (Bootstrapping Language-Image Pre-training), BLIP-2, and CLIP (Contrastive Language-Image Pre-training) models to create detailed captions for given images and compare visual content.

## Features

- Simple image description generation using BLIP
- Enhanced image description generation using BLIP-2
- Image comparison using CLIP
- Support for various image formats (JPEG, PNG, etc.)
- Flexible image description and comparison functionality

## Installation

1. Clone this repository:

   ```
   git clone https://github.com/yourusername/image-description-generator.git
   cd image-description-generator
   ```

2. Install the required dependencies:
   ```
   pip install transformers Pillow sentence-transformers torch
   ```

## Usage

1. Place your image(s) in the `images` directory.

2. To generate a description for a single image:

   ```
   python models/describe.py
   ```

3. To compare two images:

   ```
   python models/compare.py
   ```

4. The scripts will process the image(s) and output the results.

## Customization

- To use different images, modify the `image_path` variables in the `main()` functions of `models/describe.py` and `models/compare.py`.
- To switch between simple and enhanced description generation, change the function call in `describe.py` from `describe_image_enhanced()` to `describe_image_simple()` or vice versa.

## Models

- `describe_image_simple()`: Uses the BLIP base model for faster but simpler descriptions.
- `describe_image_enhanced()`: Uses the BLIP-2 model for more detailed and context-aware descriptions.
- `compare_images()`: Uses CLIP to compare the visual similarity between two images.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).
