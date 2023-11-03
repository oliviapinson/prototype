# CNN for Skin Cancer Detection Prototype

Convolutional Neural Networks (CNNs) are used for image classification. They utilize convolutional layers to detect patterns and spatial relationships to identify important features within images. This would be the preferred method for our project which aims to classify an image as a type of skin cancer. We found a dataset on Kaggle to test this concept.

**Dataset**

*  *Image* file:
      * Consists of 10,015 dermatoscopic images
  
* *Metadata* file:
    * **Diagnostic Categories/Labels (7 different classes of skin cancer):**
      * Melanocytic nevi (nv)
      * Melanoma (mel)
      * Benign keratosis-like lesions (bkl)
      * Basal cell carcinoma (bcc)
      * Actinic keratoses (akiec)
      * Vascular lesions (vasc)
      * Dermatofibroma (df)

  * **Diagnostic Method:**
      * histopathology (histo)
      * follow-up examination (follow_up)
      * expert consensus (consensus)
      * confirmation by in-vivo confocal microscopy (confocal)

**Columns in Metadata file**


  *   **image_id:** to connect with image file name
  *   **dx:** nv, mel, bkl, bcc, akiec, vasc, df
  *   **dx_type:** histo, follow_up, consensus, confocal
  *   **age:** 0-85
  *   **sex:** male, female
  *   **localization:** area on body

    

**Model**: 
In -> [[Conv2D->relu]*2 -> MaxPool2D -> Dropout]*2 -> Flatten -> Dense -> Dropout -> Out

**Test Dataset (Unseen Data) Accuracy**: 75%


[See .ipynb file for outputs]
