# Data Augmentation 

Data augmentation is the process of artificially generating new data from existing data, primarily to train new machine learning (ML) models.


## Non-Random Transforms

### ● Pad Transform
```
padded_imgs = [transforms.Pad(padding=padding, fill=125, padding_mode='reflect')(original_img) for padding in (5, 15, 20, 45)]
```

_Output_

![Sample Image](Non-Random_Transformstemp/output-figures/Pad.png)

### ● Resize Transform
```
resize_imgs = [transforms.Resize(size=size) (original_img) for size in (30, 50 , 100, original_img.size)]
```

_Output_

![Sample Image](Non-Random_Transformstemp/output-figures/Resize.png)

### ● CenterCrop Transform
```
centerCrop_imgs = [transforms.CenterCrop(size=size) (original_img) for size in (30, 50 , 100, original_img.size)]
```

_Output_

![Sample Image](Non-Random_Transformstemp/output-figures/CenterCrop.png)

### ● FiveCrop Transform
```
(top_left, top_right, bottom_left, bottom_right, center) = transforms.FiveCrop(size=(100, 100)) (original_img)
```

_Output_

![Sample Image](Non-Random_Transformstemp/output-figures/FiveCrop.png)


## Random Transforms

### ● ColorJitter Transform

_First Ouput_

![Sample Image](Random_Transforms/Outputs/ColorJitter-output.png)

_Second Output_

![Sample Image](Random_Transforms/Outputs/ColorJitter-second-output.png)


### ● RandomPerspective Transform

_First Ouput_

![Sample Image](Random_Transforms/Outputs/RandPrespective-1th-output.png)

_Second Output_

![Sample Image](Random_Transforms/Outputs/RandPrespective-2th-output.png)


### ● RandomRotation Transform

_First Ouput_

![Sample Image](Random_Transforms/Outputs/RandRotation-1th-output.png)

_Second Output_

![Sample Image](Random_Transforms/Outputs/RandRotation-2th-output.png)


### ● RandomCrop Transform

_First Ouput_

![Sample Image](Random_Transforms/Outputs/RandCrop-1th-output.png)

_Second Output_

![Sample Image](Random_Transforms/Outputs/RandCrop-2th-output.png)


### ● RandomVerticalFlip Transform

_First Ouput_

![Sample Image](Random_Transforms/Outputs/RandVerticalFlip-1th-output.png)

_Second Output_

![Sample Image](Random_Transforms/Outputs/RandVerticalFlip-2th-output.png)


## Auto Augmentation

### ● RandAugment Transform

_First Output_

![Sample Image](Auto_Augmentation/Outputs/RandAugment-1th-output.png)

_Second Output_

![Sample Image](Auto_Augmentation/Outputs/RandAugment-2th-output.png)


### ● AugMix Transform

_First Output_

![Sample Image](Auto_Augmentation/Outputs/AugMix-1th-output.png)

_Second Output_

![Sample Image](Auto_Augmentation/Outputs/AugMix-2th-output.png)
