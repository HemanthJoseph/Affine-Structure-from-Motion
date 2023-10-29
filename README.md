# Affine Structure from Motion
Structure from Motion (SfM) is a Computer Vision and Photogrammetry technique that aims to reconstruct the 3D structure of a scene from a collection of 2D images or video frames captured from different viewpoints. It involves estimating the 3D positions of points or features in the scene, as well as the camera parameters (position and orientation) for each image. The ultimate goal of SfM is to create a 3D model of the scene that represents the spatial arrangement of objects and their relationship to each other.

![SfM](/Images/SfM1.png)

## Affine Vs Projective SfM
Affine Structure from Motion and Projective Structure from Motion are two different approaches to solving the problem of reconstructing 3D scenes from 2D images or video sequences. They differ in the assumptions they make about the underlying geometry of the scene and the camera models they use. Here's a brief explanation of the key differences between the two:

1. Geometry Assumptions:
    * **Affine Structure from Motion**: Affine Structure from Motion assumes that the 3D scene and camera motion can be described using affine transformations. Affine transformations are a more general class of transformations that include translations, rotations, and non-uniform scaling. This means that the method assumes the 3D scene is undergoing an affine transformation over time, which is more restrictive than purely projective transformations.
    * **Projective Structure from Motion**: Projective Structure from Motion, on the other hand, assumes a more general projective geometry. Projective transformations include affine transformations as a special case but also encompass perspective transformations and other more complex mappings. Therefore, Projective Structure from Motion is more flexible in terms of the types of scene and camera motion it can handle.

2. Camera Models:
    * **Affine Structure from Motion**: Affine Structure from Motion typically uses an affine camera model to represent the camera's projection of 3D points onto the 2D image plane. This model includes parameters for translation, rotation, and non-uniform scaling.
    * **Projective Structure from Motion**: Projective Structure from Motion typically uses a more general projective camera model that includes parameters for translation, rotation, focal length, and the perspective projection. This model can handle a wider range of camera configurations, including those with significant perspective effects.

3. Applicability:
    * **Affine Structure from Motion**: Affine Structure from Motion is well-suited for scenarios where the scene and camera motion can be reasonably approximated as affine transformations. It might be appropriate for certain types of planar scenes or scenes with significant planar surfaces.
    * **Projective Structure from Motion**: Projective Structure from Motion is more versatile and can be applied to a wider range of scenarios, including scenes with significant perspective effects and non-planar structures.

## Applications
* 3D modeling of objects, environments, and cultural heritage sites.
* Robotics and navigation, where SfM can help robots understand their surroundings.
* Augmented reality and virtual reality, for realistic integration of virtual objects into the real world.
* Geographic information systems (GIS) and cartography.
* Motion tracking and surveillance.

## Usage

* Clone the repo to your local machine
```
git clone https://github.com/HemanthJoseph/Affine-Structure-from-Motion.git
```
* Download the file ```Affine_SfM.ipynb``` and open it on your local Google Colab

* Run each cell as per the instruction

## Dependencies

1. Numpy
2. Scipy
3. Matplotlib

Since you will be running it on Google Colab, it will take care of the dependencies.

## Results

### Image structure
 
| Input Images             |  3D Point Cloud Reconstruction |
:------------------------------:|:-------------------------:
![Input Image](/Images/SfM2.png)  |  ![output Image](/Images/output.png)

### Camera Motion 
![output Image Cam Motion](/Images/output2.png)