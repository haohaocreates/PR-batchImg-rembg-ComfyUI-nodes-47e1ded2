# [Rembg](https://github.com/danielgatis/rembg) of Plural Images for [ComfyUI](https://github.com/comfyanonymous/ComfyUI) custom-nodes
</br>
</br>

<img src = 'https://github.com/Mamaaaamooooo/batchImg-rembg-ComfyUI-nodes/assets/135937372/d3e05963-b047-4900-aa58-10f1e1b0980c' width="400" height="400"></img>
<img src = 'https://github.com/Mamaaaamooooo/batchImg-rembg-ComfyUI-nodes/assets/135937372/bef5f8b4-3976-4c59-848f-7e77df6bd5a3' width="400" height="400"></img>


## Installation 

1. Clone to your `custom_nodes` folder in ComfyUI:

```
git clone https://github.com/Mamaaaamooooo/batchImg-rembg-ComfyUI-nodes.git
```

2. Install `rembg[gpu]` (recommended) or `rembg`, depending on GPU support, to your ComfyUI virtual environment. E.g.:

```
pip install rembg[gpu]
pip install tqdm
```


### [batchImg-rembg](https://github.com/Mamaaaamooooo/batchImg-rembg-ComfyUI-nodes) workflows will often make use of these helpful node packs:
---
</br>

- > [ComfyUI-AnimateDiff-Evolved](https://github.com/Kosinkadink/ComfyUI-AnimateDiff-Evolved) for img2vid.
- > [ComfyUI-VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite) for loading videos, combining images into videos.
- > [comfyui_controlnet_aux](https://github.com/Fannovel16/comfy_controlnet_preprocessors) for preprocessing original images to depth, lineart, openpose images. 
</br>
    
## Workflow 
> for example,
<img src= 'https://github.com/Mamaaaamooooo/batchImg-rembg-ComfyUI-nodes/assets/135937372/a516f83b-f149-45be-9dba-31c35c719f3b'>

</br>
</br>
</br>
<img src = 'https://github.com/Mamaaaamooooo/batchImg-rembg-ComfyUI-nodes/assets/135937372/17966afa-0b8a-4774-95d0-2c57b3846694'>


### Optional Models(Choose according to your work, downloaded automatically)
---

All models are downloaded and saved in the user home folder in the `.u2net` directory.

The available models are:

- u2net(default) ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases.
- u2netp ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
- u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human segmentation.
- u2net_cloth_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths Parsing from human portrait. Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
- silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
- isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
- isnet-anime ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy segmentation for anime character.
- sam(not recommended, it's not easy to use) ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.


## Acknowledgements

Thanks to [rembg-comfyui-node](https://github.com/Jcd1230/rembg-comfyui-node) for insight.</br>
Thanks to [rembg-comfyui-node-better](https://github.com/Loewen-Hob/rembg-comfyui-node-better/tree/main) for modifying repo.