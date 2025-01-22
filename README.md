## Vision-Based Captioning for Images using Florence Model

### Project Overview
This project utilizes the **Florence-2-large** model by Microsoft to generate detailed captions for images. The model processes visual content and generates descriptive captions using natural language.

### Features
- **Image Processing**: Detects objects and scenes in images.
- **Caption Generation**: Generates detailed textual descriptions based on the image.
- **Multi-Image Support**: Handles different image inputs (e.g., screenshots, photos).

### Example Output
- **Volkswagen Beetle**:
  > "A vintage Volkswagen Beetle car parked on a cobblestone street in front of a yellow building. The car is turquoise with a white stripe, and the building has peeling paint."

- **Video Call Screenshot**:
  > "A screenshot of a video call interface showing six people in a grid layout. Options like 'Participants' and 'Share invite' are visible."

### Technologies Used
- **Florence-2-large Model** (Microsoft)
- **Transformers Library** (Hugging Face)
- **Torch** (GPU Acceleration)
- **PIL** (Image Processing)
- **Requests** (Image Downloading)

### How It Works
1. Load the pre-trained **Florence-2-large** model.
2. Process the image using `AutoProcessor` and `AutoModelForCausalLM`.
3. Generate captions based on predefined prompts (e.g., `<MORE_DETAILED_CAPTION>`).
4. Return a detailed caption describing the image content.

### Project Setup
- **Model**: `microsoft/Florence-2-large`
- **Dependencies**:
  - `transformers`
  - `torch`
  - `PIL`
  - `requests`
