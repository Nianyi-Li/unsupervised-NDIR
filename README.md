# Unsupervised Non-Rigid Image Distortion Removal via Grid Deformation

### [**Paper**](https://openaccess.thecvf.com/content/ICCV2021/papers/Li_Unsupervised_Non-Rigid_Image_Distortion_Removal_via_Grid_Deformation_ICCV_2021_paper.pdf) | [**Video**](https://youtu.be/aeJkb5u0Cb8)

Nianyi Li<sup>3,1</sup>, Simron Thapa<sup>1</sup>, Cameron Whyte<sup>2</sup>, Albert Reed<sup>2</sup>, Suren Jayasuriya<sup>2</sup>, Jinwei Ye<sup>1</sup>

<sup>1</sup>Louisiana State University,         <sup>2</sup>Arizona State University,         <sup>3</sup>Clemson University

Accepted as poster in ICCV 2021


<!-- ![teaser](https://user-images.githubusercontent.com/22784070/129606461-13390c92-9e59-4f0f-8fad-e2111e7ada24.png){:height="20%" width="20%"} -->
<!--- This isn't commented out 
<img src="https://user-images.githubusercontent.com/22784070/129606461-13390c92-9e59-4f0f-8fad-e2111e7ada24.png" width="70%" height="70%"> --->



### Problem Definition
Many computer vision problems face difficulties when imaging through turbulent refractive media (e.g., air and water) due to the refraction and scattering of light. These effects cause geometric distortion that requires either handcrafted physical priors or supervised learning methods to remove. 

![problems](https://user-images.githubusercontent.com/22784070/137431727-b960e88a-f158-4abd-bebe-070c65731dc4.gif)

### Network Architecture
In this paper, we present a novel unsupervised network to recover the latent distortion-free image. The key idea is to model non-rigid distortions as deformable grids. Our network consists of a grid deformer that estimates the distortion field and an image generator that outputs the distortion-free image. 

![network](https://user-images.githubusercontent.com/22784070/137433546-753f48d2-c8eb-4778-9c5a-0e957b50327d.png)

By leveraging the positional encoding operator, we can simplify the network structure while maintaining fine spatial details in the recovered images. 


### Results

Our method doesn't need to be trained on labeled data and has good transferability across various turbulent image datasets with different types of distortions. Extensive experiments on both simulated and real-captured turbulent images demonstrate that our method can remove both air and water distortions without much customization.


![Air result_new](https://user-images.githubusercontent.com/22784070/137434314-75897f73-0a1c-4a0c-92f3-08cdf44093ac.gif)

![Water result_new](https://user-images.githubusercontent.com/22784070/137434589-4c65647a-3e96-4ca9-aea6-7dffb46e0fd5.gif)

## Citation

```
@InProceedings{Li_2021_ICCV,
    author    = {Li, Nianyi and Thapa, Simron and Whyte, Cameron and Reed, Albert W. and Jayasuriya, Suren and Ye, Jinwei},
    title     = {Unsupervised Non-Rigid Image Distortion Removal via Grid Deformation},
    booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
    month     = {October},
    year      = {2021},
    pages     = {2522-2532}
}
```


