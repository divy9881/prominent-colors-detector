# prominent-colors-detector
A engine which detects prominent colors from the image.

## Install Python Package
```
pip install image-pcd
```

## Usage

```python
from pcd import ImageProminentColor
from sklearn.cluster import KMeans

image_color = ImageProminentColor("<path to image file>")
prominent_colors = image_color.get_prominent_colors(KMeans, 3)
```
The above code-snippet gives you top 3 prominent colors in RGB form sorted in decreasing order of prominence from the image.

```python
image_color.get_image_plot("<Save image file path>")
image_color.get_color_plot("<Save image file path>")
```
The above code-snippet allows you to save the images of plots of the prominent color and image original colors in 3D-space with RGB components as axis.

## Samples (For top-3 Prominent Colors)
| Sample Image | Prominent Colors | Prominent Colors Plot | Image Colors Plot |
| ------------ | ---------------- | -------------------- | ---------------- |
| ![colorful](./images/colorful.jpg) | ![#215d1d](https://via.placeholder.com/15/215d1d/000000?text=+) `#215d1d` <br/> ![#97244a](https://via.placeholder.com/15/97244a/000000?text=+) `#97244a` <br/> ![#1d8197](https://via.placeholder.com/15/1d8197/000000?text=+) `#1d8197` | ![colorful_color](./images/colorful_color.png) | ![colorful_image](./images/colorful_image.png) |
| ![php](./images/php.png) | ![#7579b0](https://via.placeholder.com/15/7579b0/000000?text=+) `#7579b0` <br/> ![#fdfdfe](https://via.placeholder.com/15/fdfdfe/000000?text=+) `#fdfdfe` <br/> ![#010101](https://via.placeholder.com/15/010101/000000?text=+) `#010101` | ![php_color](./images/php_color.png) | ![php_image](./images/php_image.png) |
| ![colorful](./images/nodejs.png) | ![#fefefe](https://via.placeholder.com/15/fefefe/000000?text=+) `#fefefe` <br/> ![#323232](https://via.placeholder.com/15/323232/000000?text=+) `#323232` <br/> ![#67a15d](https://via.placeholder.com/15/67a15d/000000?text=+) `#67a15d`  | ![nodejs_color](./images/nodejs_color.png) | ![nodejs_image](./images/nodejs_image.png) |