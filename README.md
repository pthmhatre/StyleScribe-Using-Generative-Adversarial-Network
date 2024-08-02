# StyleScribe-Using-Generative-Adversarial-Network
<div align="justify">
StyleScribe is a sophisticated text-to-image generation project that leverages state-of-the-art techniques in Natural Language Processing (NLP) and Generative Adversarial Networks (GANs). The primary objective of this project is to generate high-quality images of fashion products based on textual descriptions. By bridging the semantic gap between text and visual content, StyleScribe offers an innovative solution for the fashion industry, enabling the creation of visual content from descriptive text inputs.
</div>

### Key Features
<div align='justify'>
  
**Text-to-Image Generator**: StyleScribe uses advanced GAN models to convert textual descriptions into realistic images of fashion products.
**Large Dataset**: The project utilizes a meticulously curated dataset of 60,000 unique fashion product images and their corresponding descriptions to train the model.<br>
**NLP Integration**: Extensive preprocessing of textual data ensures semantic coherence and relevance, enhancing the quality of generated images.<br>
**Custom GAN Architecture**: A tailored GAN model, comprising a generator and discriminator, is designed to produce high-fidelity fashion images.<br>
**Scalable Infrastructure**: The project is  hosted on Google Cloud RDP and uses Flask for the web interface and Firebase for real-time database management.<br>
</div>

### System Architecture
**Frontend:** <br>
● Developed using Flask, the frontend has intuitive web interface for users to input text descriptions and view generated images.<br>
**Backend:**  <br>
● The backend is powered by a Flask server, which handles incoming requests and communicates with the model server.<br>
**Model Server:**  <br>
● Hosted on Google Cloud RDP, the model server processes text inputs through the GAN model and generates images.<br>
**Database:**  <br>
● Firebase Firestore/Realtime Database stores metadata and text descriptions, ensuring real-time data synchronization.<br>
**Storage:**  <br>
● Google Cloud Storage or Firebase Storage is used to store the training dataset and generated images.<br>

# Proposed Algorithm
<div align='justify'>
The success of the project hinges on the development and implementation of an advanced
algorithm that seamlessly bridges textual descriptions of fashion concepts with visually stunning design outputs. The proposed algorithm, underpinned by deep learning techniques and
state-of-the-art technology, outlines the key steps and components that drive the transformative
power of the platform.</div>

1. Textual Input Interpretation: The algorithm processes user input, extracting relevant information using natural language processing (NLP). Whether it’s a simple phrase or a detailed description, the NLP techniques identify color, style, length, and design elements.
2. Neural Network for Text-to-Image Conversion:<br>
  ● Generator: This component creates an initial image representation based on the textual input. It translates extracted details (e.g., color, shape) into a visual concept.<br>
  ● Discriminator: Evaluates the quality and realism of generated images by comparing them to a real fashion image dataset. The feedback loop refines the generator’s output over time.
3. Training the AI Model: The neural network trains on a diverse fashion image dataset, enabling it to generate a wide range of design concepts.
4. Feedback Loop and Improvement: As users interact with the platform, the model learns from successes and mistakes, continuously improving its designs.
5. User Customization: Users can further customize designs, specifying color choices, patterns, and fabric textures.
6. Output Generation: The algorithm produces high-resolution images reflecting the user’s fashion concept.

# Use-Case Diagrams

| Actors  | Description|
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| User |Users act as creators by providing textual descriptions of their fashion concepts, customizing generated designs, and offering feedback. They drive the creative process, shaping the AI-generated fashaion designs to align with their vision.|
| Administrator |Administrator can make changes to the application by modifying or adding new models.An extension of the administrator’s role is that he can also Add new features if required.|
<p align="center">
  <img src="https://github.com/user-attachments/assets/9caf8d92-44da-4513-8054-e40511bbca6e" height="300px">
  &nbsp;&nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/5e1a48cf-5d32-4cd4-af48-2343d527c154" height="300px">
</p>

# Analysis Modeling
### ER Diagram
The ER Diagram outlines the backend process of an application, including input processing and activity flow. When the initial screen appears, functions are executed based on user actions. The input prompt plays a crucial role in this execution.
<p align="center">
  <img src="https://github.com/user-attachments/assets/0ba7563e-3d5c-444a-88d8-0acd6afa493e" height="300px" width="600px">
</p>

### Activity Diagram
The Activity Diagram outlines the stages in the application process. It begins with opening the application and focusing on the input field for manual text entry. Users can then interact with the displayed image, either closing the application or using additional features based on text prompts.
<p align="center">
  <img src="https://github.com/user-attachments/assets/cc7cd118-0434-442a-9b26-c660c12ca0d7" height="500px" width="600px">
</p>

# Functional Modeling
###  DFD:Level 0
In DFD the user queries for information. The Administrator has extra privileges
like changing the function and model. The system then creates the desired output and displays
it on screen.
<p align="center">
  <img src="https://github.com/user-attachments/assets/949b1a66-24a9-4cc2-81d4-7e5393312d90" height="300px" width="800px">
</p>

### DFD:Level 1
<div align="justify">
In DFD level 1 the user uses his smartphone or tablet to open the application andgive the text input using text field on UI.
The input then is used to first understand the meaning of the input text and extract the features. Once the features are extracted the image generation process starts and the image is generated pixel by pixel.</div>
<p align="center" >
    <img src="https://github.com/user-attachments/assets/fc0e437f-345e-4cc9-b820-9c2cd0b73543" height="300px" width="600px">
</p>

### DFD:Level 2
<div align="justify">
In DFD level 2 the user give the input to NLP algorithm and through that we get
the extracted features and those are used to refer to the image dataset and labled images which
lables are used to refere to the meaning and the features user expecting to include in output.
Image generator is used to create variations of the image user expecting as a output image by
Features Matching and Precise image selector Function
</div>
<p align="center" >
    <img src="https://github.com/user-attachments/assets/c8e6ecd6-421d-49f8-94eb-86c9a1561e32" height="300px" width="600px">
</p>

# Dataset
The project utilizes a meticulously curated dataset of 60,000 unique fashion product images and their corresponding descriptions to train the model.This images are lebelled with multiple attributes which provides its description in the form of metadata.

### Metadata
<p align="center" >
    <img src="https://github.com/user-attachments/assets/d8ec068d-b29c-4ba0-94f3-98726a6608af" height="300px" width="600px">
</p>
<p align="center" >
    <img src="https://github.com/user-attachments/assets/003e671f-6772-474f-8ba5-06fef10e20ba" height="300px" width="600px">
</p>

### Image data
<p align="center" >
    <img src="https://github.com/user-attachments/assets/89cc8b4d-e383-4833-a4a5-8bdb528f5bf2" height="300px" width="600px">
</p>
<p align="center" >
    <img src="https://github.com/user-attachments/assets/0444c4f7-76fe-4be3-a4b0-b2649d22d3f5" height="300px" width="600px">
</p>

# Results and UI Design 
<p align='center'>

<img src="https://github.com/user-attachments/assets/1caa50d1-58cf-4cc1-9252-147e8247d4fb">
<img src="https://github.com/user-attachments/assets/89703a8d-83e7-4728-90ec-9883d731efe6">
<img src="https://github.com/user-attachments/assets/faa687a4-5208-44ed-9adf-630fc62bb1bd">
<img src="https://github.com/user-attachments/assets/8785c08e-a34b-4ff0-8efa-5ce794bae653">
<img src="https://github.com/user-attachments/assets/75d8015d-55d7-4dda-8f29-6f22420ec4b1">
<img src="https://github.com/user-attachments/assets/9f4be771-d106-4834-89fb-3d70b528fa62">
<img src="https://github.com/user-attachments/assets/7a3d70ac-7001-446e-9a31-03977c57b8ed">

</p>
