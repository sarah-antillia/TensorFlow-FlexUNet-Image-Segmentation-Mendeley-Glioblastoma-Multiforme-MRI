<h2>TensorFlow-FlexUNet-Image-Segmentation-Mendeley-Glioblastoma-Multiforme-MRI (2026/04/23)</h2>
Sarah T. Arai<br>
Software Laboratory antillia.com<br><br>
This is the first experiment of Image Segmentation for <b>Mendeley-Glioblastoma-Multiforme-MRI</b> based on 
our <a href="./src/TensorFlowFlexUNet.py">TensorFlowFlexUNet</a>
 (<b>TensorFlow Flexible UNet Image Segmentation Model for Multiclass</b>), and a 512x512 pixels PNG
 <a href="https://drive.google.com/file/d/1Z-K5dIRw0TZ7TW1NAEKpL6qflLuMkqzz/view?usp=sharing">
Mendeley-Glioblastoma-Multiforme-ImageMask-Dataset.zip</a> with colorized masks 
(<a href="https://creativecommons.org/licenses/by/4.0/">
CC BY 4.0</a>), which was derived by us from <br><br>
<a href="https://data.mendeley.com/datasets/mxsb7snyvx/2">
Glioblastoma Multiforme Brain MRI Dataset for Tumor Detection and Classification
</a> on the mendeley.com
<br><br>
<hr>
<b>Actual Image Segmentation for Glioblastoma-Multiforme Images of 512x512 pixels</b><br>
As shown below, the inferred masks predicted by our segmentation model trained by the dataset appear similar to the 
ground truth masks, but they lack precision in certain areas.
<br><br>
<b>class_color_map = {NCR (Necrotic Tumor Core):red, ED (Edema):green, ET (Enhancing Tumor):blue}</b>
<br><br>
<table>
<tr>
<th>Input: image</th>
<th>Mask (ground_truth)</th>
<th>Prediction: inferred_mask</th>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/images/10080_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/masks/10080_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test_output/10080_.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/images/10180_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/masks/10180_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test_output/10180_.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/images/10523_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/masks/10523_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test_output/10523_.png" width="320" height="auto"></td>
</tr>
</table>
<hr>
<br>
<h3>1. Dataset Citation</h3>
The image dataset used here was taken from <br><br>
<a href="https://data.mendeley.com/datasets/mxsb7snyvx/2">
Glioblastoma Multiforme Brain MRI Dataset for Tumor Detection and Classification
</a> on the mendeley.com
<br><br>
The following explanation was taken from the above mendeley web site.
<br><br>
<b>Description</b><br>
The dataset consists of MRI brain scans of healthy subjects and patients diagnosed with Glioblastoma, collected from JK CT Scan & Research Centre, Jammu – 180003, India, during the period 2 March 2023 to 10 March 2024.
<br><br>
The data collection process was carried out under the supervision and clinical guidance of Dr. Sahil Gupta, Consultant Radiologist and Director at JK CT Scan & Research Centre. Dr. Gupta facilitated access to the MRI scans, ensured clinical correctness of diagnoses, and verified that all scans were acquired following standard radiological protocols.
<br><br>
All MRI data were fully anonymized prior to being handed over for research use. No personally identifiable information (PII) such as patient names, registration numbers, or demographic identifiers was included in the dataset. The data were provided strictly for academic and non-commercial research purposes, in compliance with ethical standards and patient confidentiality norms.
<br>
<br>
<b>Citation</b><br>
Singh, Kuljeet; Malhotra, Deepti; Gupta, Sahil  (2026), <br>
“Glioblastoma Multiforme Brain MRI Dataset for Tumor Detection and Classification”, <br>
Mendeley Data, V2, doi: 10.17632/mxsb7snyvx.2
<br><br>
<b>License</b><br>
<a href="https://creativecommons.org/licenses/by/4.0/">
CC BY 4.0</a>
<br>
<br>
<h3>2 Mendeley-Glioblastoma-Multiforme ImageMask Dataset</h3>
<h3>2.1 Download Mendeley-Glioblastoma-Multiforme Dataset</h3>
 If you would like to train this Mendeley-Glioblastoma-Multiforme Segmentation model by yourself,
 please download the dataset from the google drive our downscaled 
 <a href="https://drive.google.com/file/d/1Z-K5dIRw0TZ7TW1NAEKpL6qflLuMkqzz/view?usp=sharing">
Mendeley-Glioblastoma-Multiforme-ImageMask-Dataset.zip</a> .zip</a> 
(<a href="https://creativecommons.org/licenses/by/4.0/">CC BY 4.0</a>)) 
, expand the downloaded ImageMaskDataset and put it under <b>./dataset</b> folder to be:
<br>
<pre>
./dataset
└─Mendeley-Glioblastoma-Multiforme
    ├─test
    │   ├─images
    │   └─masks
    ├─train
    │   ├─images
    │   └─masks
    └─valid
        ├─images
        └─masks
</pre>
<br>
<b>Mendeley-Glioblastoma-Multiforme Statistics</b><br>
<img src ="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/Mendeley-Glioblastoma-Multiforme_Statistics.png" width="512" height="auto"><br>
<br><br>
As shown above, the number of images of train and valid datasets is large enough to use for the
 training set of our segmentation model.
<br><br>
<h4>2.2 Derivation of 512x512 pixels ImageMask Dataset</h4>
The folder structure of <b>Glioblastoma Multiforme Brain MRI Dataset for Tumor</b> is the following, which
contains 936 JPG images files, but no corresponding annotation files.<br>
<pre>
./Glioblastoma Multiforme Brain MRI Dataset for Tumor
└─Glioblastoma
     ├─00D5A20C.jpg
     ├─00D5A824.jpg  
...
     └─00499695.jpg
</pre>
<b>Original Glioblastoma Sample Images</b><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/original_glioblastoma.png" 
width="1024" height="auto"><br><br>
<b>Step 1</b><br>
We generated a 512x512 pixels PNG master <b>Glioblastoma Multiforme image and annotation (mask)</b> dataset by applying a
segmentation (inference) method of a pretrained Glioma TensorFlowFlexUNet model 
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-UTSW-Glioma-T2W-Subset">
TensorFlow-FlexUNet-Image-Segmentation-UTSW-Glioma-T2W-Subset
</a> to the Glioblastoma images, without human annotation experts.<br><br>
We also used the following class color mapping table for Glioma three classes.<br><br>
<table border="1" style="border-collapse: collapse;">
<tr><th>Index</th><th>Category</th><th>Color </th><th>RGB triplet</th></tr>
<tr>
<td>1</td><td>NCR(Necrotic Tumor Core)</td><td>red</td><td>(255,0,0)</td>
</tr>
<tr>
<td>2</td><td>ED (Peritumoral Edema)</td><td>green</td><td>(0,255,0)</td>
</tr>
<tr>
<td>3</td><td>ET (Enhancing Tumor)</td><td>blue</td><td>(0,0,255)</td>
</tr>
</table>
<br><br>
<b>Step 2</b><br>
We generated an augmented PNG ImageMask Dataset from the master dataset by using 
<a href="https://github.com/sarah-antillia/Image-Deformation-Tool">Image Deformation Tool</a> and 
<a href="https://github.com/sarah-antillia/Image-Distortion-Tool">Image Distortion tool</a>.<br><br>

<h3>2.3 Train Sample Images and Masks</h3>
<b>Train sample images</b><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/train_images_sample.png" width="1024" height="auto">
<br>
<b>Train sample masks</b><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/train_masks_sample.png" width="1024" height="auto">
<br>
<h3>3 Train TensorFlowFlexUNet Model</h3>
 We trained Mendeley-Glioblastoma-Multiforme TensorFlowFlexUNet Model by using the 
<a href="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/train_eval_infer.config"> <b>train_eval_infer.config</b></a> file. <br>
Please move to ./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme and run the following bat file.<br>
<pre>
>1.train.bat
</pre>
, which simply runs the following command.<br>
<pre>
>python ../../../src/TensorFlowFlexUNetTrainer.py ./train_eval_infer.config
</pre>
<hr>
<b>Model parameters</b><br>
Defined a small <b>base_filters = 16 </b> and large <b>base_kernels = (11,11)</b> for the first Conv Layer of Encoder Block of 
<a href="./src/TensorFlowFlexUNet.py">TensorFlowFlexUNet.py</a> 
and a large num_layers (including a bridge between Encoder and Decoder Blocks).
<pre>
[model]
;You may specify your own UNet class derived from our TensorFlowFlexModel
model         = "TensorFlowFlexUNet"
image_width    = 512
image_height   = 512
image_channels = 3
input_normalize = True
normalization  = False
num_classes    = 4
base_filters   = 16
base_kernels   = (11,11)
num_layers     = 8
dropout_rate   = 0.05
dilation       = (1,1)
</pre>
<b>Learning rate</b><br>
Defined a small learning rate.  
<pre>
[model]
learning_rate  = 0.00007
</pre>
<b>Loss and metrics functions</b><br>
Specified "categorical_crossentropy" and <a href="./src/dice_coef_multiclass.py">"dice_coef_multiclass"</a>.<br>
<pre>
[model]
loss           = "categorical_crossentropy"
metrics        = ["dice_coef_multiclass"]
</pre>
<b>Dataset class</b><br>
Specifed <a href="./src/ImageCategorizedMaskDataset.py">ImageCategorizedMaskDataset</a> class.<br>
<pre>
[dataset]
class_name    = "ImageCategorizedMaskDataset"
</pre>
<br>
<b>Learning rate reducer callback</b><br>
Enabled learing_rate_reducer callback, and a small reducer_patience.
<pre> 
[train]
learning_rate_reducer = True
reducer_factor     = 0.5
reducer_patience   = 5
</pre>
<b>Early stopping callback</b><br>
Enabled early stopping callback with patience parameter.
<pre>
[train]
patience      = 10
</pre>
<b>RGB Color map</b><br>
Specifed rgb color map dict for Mendeley-Glioblastoma-Multiforme 1+3 classes.<br>
<pre>
[mask]
mask_datatyoe    = "categorized"
mask_file_format = ".png"
;Mendeley-Glioblastoma-Multiforme rgb color map dict for 1+3 classes.
rgb_map = {(0,0,0):0, (255,0,0):1, (0,255,0):2, (0,0,255):3,}
</pre>
<b>Epoch change inference callback</b><br>
Enabled <a href="./src/EpochChangeInferencer.py">epoch_change_infer callback</a></b>.<br>
<pre>
[train]
epoch_change_infer       = True
epoch_change_infer_dir   =  "./epoch_change_infer"
num_infer_images         = 6
</pre>
By using this callback, on every epoch_change, the inference procedure can be called
 for 6 images in <b>mini_test</b> folder. This will help you confirm how the predicted mask changes 
 at each epoch during your training process.<br> 
<br> 
As shown below, early in the model training, the predicted masks from our UNet segmentation model showed 
discouraging results. However, as training progressed through the epochs, the predictions gradually improved. 
<br><br> 
<b>Epoch_change_inference output at starting (epoch 1,2,3)</b><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/epoch_change_infer_at_start.png" width="1024" height="auto"><br>
<br>
<b>Epoch_change_inference output at middlepoint (epoch 28,29,30)</b><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/epoch_change_infer_at_middlepoint.png" width="1024" height="auto"><br>
<br>
<b>Epoch_change_inference output at ending (epoch 58,59,60)</b><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/epoch_change_infer_at_end.png" width="1024" height="auto"><br>
<br>
In this experiment, the training process was terminated at epoch 60.<br><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/train_console_output_at_epoch60.png" width="1024" height="auto"><br>
<br>
<a href="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/eval/train_metrics.csv">train_metrics.csv</a><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/eval/train_metrics.png" width="520" height="auto"><br>
<br>
<a href="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/eval/train_losses.csv">train_losses.csv</a><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/eval/train_losses.png" width="520" height="auto">
<br>
<h3>
4 Evaluation
</h3>
Please move to <b>./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme</b> folder, 
and run the following bat file to evaluate TensorFlowUNet model for Mendeley-Glioblastoma-Multiforme.<br>
<pre>
>./2.evaluate.bat
</pre>
This bat file simply runs the following command.
<pre>
>python ../../../src/TensorFlowFlexUNetEvaluator.py ./train_eval_infer_aug.config
</pre>
Evaluation console output:<br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/evaluate_console_output_at_epoch60.png" width="1024" height="auto">
<br><br>Image-Segmentation-Mendeley-Glioblastoma-Multiforme
<a href="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/evaluation.csv">evaluation.csv</a><br>
The loss (categorical_crossentropy) to this <b>Mendeley-Glioblastoma-Multiforme/test</b> was not so low, 
and dice_coef_multiclass not high as shown below.
<br>
<pre>
categorical_crossentropy,0.0488
dice_coef_multiclass,0.9752
</pre>
<br>
<h3>
5 Inference
</h3>
Please move to a <b>./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme</b> folder, and run the following bat file to infer segmentation regions for images by the Trained-TensorFlowUNet model for Mendeley-Glioblastoma-Multiforme.<br>
<pre>
>./3.infer.bat
</pre>
This simply runs the following command.
<pre>
>python ../../../src/TensorFlowFlexUNetInferencer.py ./train_eval_infer_aug.config
</pre>
<hr>
<b>mini_test_images</b><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/mini_test_images.png" width="1024" height="auto"><br>
<b>mini_test_mask(ground_truth)</b><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/mini_test_masks.png" width="1024" height="auto"><br>
<hr>
<b>Inferred test masks</b><br>
<img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/asset/mini_test_output.png" width="1024" height="auto"><br>
<br>
<hr>
<b>Enlarged images and masks of Mendeley-Glioblastoma-Multiforme Images of 512x512 pixels</b><br>
As shown below, the inferred masks predicted by our segmentation model trained by the dataset appear similar to the ,
ground truth masks, but they lack precision in certain areas.
<br><br>
<b>class_color_map = {NCR (Necrotic Tumor Core):red, ED (Edema):green, ET (Enhancing Tumor):blue}</b>
<br><br>
<table>
<tr>
<th>Input:Image</th>
<th>Mask (ground_truth)</th>
<th>Prediction:Inferred-mask</th>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/images/10018_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/masks/10018_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test_output/10018_.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/images/10036_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/masks/10036_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test_output/10036_.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/images/10158_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/masks/10158_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test_output/10158_.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/images/10313_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/masks/10313_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test_output/10313_.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/images/10345_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/masks/10345_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test_output/10345_.png" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/images/10674_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test/masks/10674_.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Mendeley-Glioblastoma-Multiforme/mini_test_output/10674_.png" width="320" height="auto"></td>
</tr>
</table>
<hr>
<br>
<h3>
References
</h3>
<b>1. The Brain Tumor Segmentation (BraTS) Challenge 2023: Glioma Segmentation in Sub-Saharan Africa Patient 
Population (BraTS-Africa)</b><br>
Maruf Adewole, Jeffrey D. Rudie, Anu Gbadamosi, Oluyemisi Toyobo, Confidence Raymond, Dong Zhang,<br>
Olubukola Omidiji, Rachel Akinola, Mohammad Abba Suwaid, Adaobi Emegoakor, Nancy Ojo, Kenneth Aguh, <br>
Chinasa Kalaiwo, Gabriel Babatunde, Afolabi Ogunleye, Yewande Gbadamosi, Kator Iorpagher, Evan Calabrese,<br>
Mariam Aboian, Marius Linguraru, Jake Albrecht, Benedikt Wiestler, Florian Kofler, Anastasia Janas,<br>
Dominic LaBella, Anahita Fathi Kzerooni, Hongwei Bran Li, Juan Eugenio Iglesias, Keyvan Farahani, <br>
James Eddy, Timothy Bergquist, Verena Chung, Russell Takeshi Shinohara, Walter Wiggins, Zachary Reitman,<br>
Chunhao Wang, Xinyang Liu, Zhifan Jiang, Ariana Familiar, Koen Van Leemput, Christina Bukas, Maire Piraud,<br>
Gian-Marco Conte, Elaine Johansson, Zeke Meier, Bjoern H Menze, Ujjwal Baid, Spyridon Bakas, Farouk Dako,<br>
Abiodun Fatade, Udunna C Anazodo<br>
<a href="https://arxiv.org/pdf/2305.19369">https://arxiv.org/pdf/2305.19369</a>
<br><br>
<b>2. Advancing Precision: A Comprehensive Review of MRI Segmentation Datasets from BraTS Challenges (2012–2025)</b><br>
Beatrice Bonato, Loris Nanni and Alessandra Bertoldo<br>
<a href="https://www.mdpi.com/1424-8220/25/6/1838">https://www.mdpi.com/1424-8220/25/6/1838</a>
<br><br>
<b>3. Multi-class glioma segmentation on real-world data with missing MRI sequences: comparison of three deep learning algorithms
</b><br>
Hugh G. Pemberton, Jiaming Wu, Ivar Kommers, Domenique M. J. Müller, Yipeng Hu, Olivia Goodkin, <br>
Sjoerd B. Vos, Sotirios Bisdas, Pierre A. Robe, Hilko Ardon, Lorenzo Bello, Marco Rossi, <br>
Tommaso Sciortino, Marco Conti Nibali, Mitchel S. Berger, Shawn L. Hervey-Jumper, Wim Bouwknegt,<br>
Wimar A. Van den Brink, Julia Furtner, Seunggu J. Han, Albert J. S. Idema, Barbara Kiesel,<br>
Georg Widhalm, Alfred Kloet, Michiel Wagemakers, Aeilko H. Zwinderman, Sandro M. Krieg, <br>
Emmanuel Mandonnet, Ferran Prados, Philip de Witt Hamer, Frederik Barkhof & Roelant S. Eijgelaar<br>
<a href="https://www.nature.com/articles/s41598-023-44794-0">
https://www.nature.com/articles/s41598-023-44794-0
</a>
<br><br>
<b>4. Training 3D U-Net for Brain Tumor Segmentation Challenge – Medical Imaging</b><br>
Jaykumaran<br>
<a href="https://learnopencv.com/3d-u-net-brats/">https://learnopencv.com/3d-u-net-brats/</a>
<br><br>
<b>5. TensorFlow-FlexUNet-Image-Segmentation-UTSW-Glioma-T2W-Subset</b><br>
Toshiyuki Arai<br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-UTSW-Glioma-T2W-Subset">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-UTSW-Glioma-T2W-Subset
</a>
<br><br>
<b>6. TensorFlow-FlexUNet-Image-Segmentation-Multiclass-BraTS2023-Subset</b><br>
Toshiyuki Arai<br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Multiclass-BraTS2023-Subset">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Multiclass-BraTS2023-Subset
</a>
<br><br>
<b>7. TensorFlow-FlexUNet-Image-Segmentation-Multiclass-BraTS2020</b><br>
Toshiyuki Arai<br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Multiclass-BraTS2020">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Multiclass-BraTS2020
</a>
<br><br>
<b>8. TensorFlow-FlexUNet-Image-Segmentation-Brain-Tumor-BraTS2019-HGG-LGG-MRI</b><br>
Toshiyuki Arai<br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Brain-Tumor-BraTS2019-HGG-LGG-MRI">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Brain-Tumor-BraTS2019-HGG-LGG-MRI
</a>
<br><br>
<b>9. TensorFlow-FlexUNet-Image-Segmentation-Model</b><br>
Toshiyuki Arai <br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Model">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Model
</a>
<br>
<br>
