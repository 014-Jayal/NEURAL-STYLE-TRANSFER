# NEURAL-STYLE-TRANSFER

*COMPANY*: CODTECH IT SOLUTUIONS

*NAME*: JAYAL SHAH

*INTERN ID*: CODF94

*DOMAIN*: Artificial Intelligence Markup Language

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH



---

# 🎨 Neural Style Transfer

This repository presents a powerful implementation of **Neural Style Transfer** using deep learning techniques in Python. Neural Style Transfer (NST) is an exciting computer vision technique that combines the **content** of one image with the **style** of another to produce a new, stylized image. It enables users to recreate photographs in the style of famous painters like Van Gogh, Picasso, or Monet.

This project uses TensorFlow and Keras to extract and blend image features from a **content image** and a **style image**, generating an output that visually merges both. The notebook offers an accessible introduction to NST and serves as a hands-on example for those interested in AI-powered creativity.

---

## 🧠 How It Works

The NST algorithm is built on top of **convolutional neural networks (CNNs)**, specifically leveraging pretrained models like **VGG19**, which is well-suited for feature extraction tasks.

Here is a step-by-step explanation of the process:

1. **Load Images**:
   The user provides a **content image** (e.g., a landscape or portrait) and a **style image** (e.g., a Van Gogh painting). Both images are resized and preprocessed to match the input format expected by the neural network.

2. **Feature Extraction with VGG19**:
   A pretrained VGG19 model (without the classification head) is loaded. Specific layers are chosen to extract content and style representations:

   * Content layers capture the structural layout.
   * Style layers extract patterns, textures, and colors.

3. **Compute Style and Content Loss**:

   * **Content Loss** measures the difference in feature representations between the content image and the generated image.
   * **Style Loss** measures the difference in Gram matrices of the style image and the generated image.
   * **Total Loss** is a weighted sum of both losses.

4. **Optimization Loop**:
   Using gradient descent (or an optimizer like Adam), the generated image is iteratively updated to minimize the total loss. The image is treated as a trainable tensor.

5. **Image Postprocessing**:
   The output image is deprocessed and displayed to visually reflect the content of the original image styled in the artistic form of the chosen painting.

---

## 📦 Requirements

To run the notebook, install the following libraries:

```bash
pip install tensorflow matplotlib numpy pillow
```

You also need:

* A **content image** file.
* A **style image** file.

Make sure both are accessible in your working directory.

---

## 📌 Features

* Combines the visual structure of one image with the artistic flair of another.
* Uses VGG19, a well-established deep CNN for feature extraction.
* Highly customizable: tweak style/content weights, layer choices, and optimizer settings.
* Notebook format for interactive experimentation and visualization.

---

## 🎯 Use Cases

* Artistic rendering of photos.
* Creating AI-generated art.
* Understanding feature representations in CNNs.
* Demonstrating deep learning applications in creative fields.

---

## 🚀 Future Enhancements

* Add support for batch processing multiple images.
* Build a web interface for easier user input.
* Enable faster training using GPU acceleration or optimized libraries.
* Explore real-time NST using fast style transfer networks.

---

## 📤 Output:

![Image](https://github.com/user-attachments/assets/05ab2c16-ee1b-4ea5-8532-45eef18eb390)
![Image](https://github.com/user-attachments/assets/7e40467b-2903-490c-99e6-a84281a0fc94)
![Image](https://github.com/user-attachments/assets/ba797be8-6ac8-4301-9eb1-ccca1dc9d9f5)

---

This project is ideal for developers, artists, and machine learning enthusiasts who want to explore the intersection of art and artificial intelligence. Feel free to clone, modify, and experiment!
