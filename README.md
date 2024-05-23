# Data Augmentation 

Data augmentation is the process of artificially generating new data from existing data, primarily to train new machine learning (ML) models.


## Non-Random Transforms

### < Pad Transform
```
padded_imgs = [transforms.Pad(padding=padding, fill=125, padding_mode='reflect')(original_img) for padding in (5, 15, 20, 45)]
```

_Output_

![Sample Image](Non-Random_Transformstemp/output-figures/Pad.png)

### -Resize Transform
```
resize_imgs = [transforms.Resize(size=size) (original_img) for size in (30, 50 , 100, original_img.size)]
```

_Output_

![Sample Image](Non-Random_Transformstemp/output-figures/Resize.png)

### -CenterCrop Transform
```
centerCrop_imgs = [transforms.CenterCrop(size=size) (original_img) for size in (30, 50 , 100, original_img.size)]
```

_Output_

![Sample Image](Non-Random_Transformstemp/output-figures/CenterCrop.png)

### -FiveCrop Transform
```
(top_left, top_right, bottom_left, bottom_right, center) = transforms.FiveCrop(size=(100, 100)) (original_img)
```

_Output_

![Sample Image](Non-Random_Transformstemp/output-figures/FiveCrop.png)

