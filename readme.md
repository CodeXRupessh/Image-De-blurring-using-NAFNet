## NAFNet: Nonlinear Activation Free Network for Image Restoration
 
### Installation

```python
python 3.9.5
pytorch 1.11.0
cuda 11.3
```

```
git clone
cd 
pip install -r requirements.txt
python setup.py develop --no_cuda_ext

```

* Single Image Inference Demo:
    * Image Denoise:
    ```
    python basicsr/demo.py -opt options/test/SIDD/NAFNet-width64.yml --input_path ./demo/noisy.png --output_path ./demo/denoise_img.png
  ```
    * Image Deblur:
    ```
    python basicsr/demo.py -opt options/test/REDS/NAFNet-width64.yml --input_path ./demo/blurry.jpg --output_path ./demo/deblur_img.png
    ```
    * ```--input_path```: the path of the degraded image
    * ```--output_path```: the path to save the predicted image
