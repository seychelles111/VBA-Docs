---
title: Crop.PictureOffsetX property (Office)
ms.prod: office
api_name:
- Office.Crop.PictureOffsetX
ms.assetid: 71ba4f1d-d94e-262e-e719-32d06bf258ef
ms.date: 01/04/2019
ms.localizationpriority: medium
---


# Crop.PictureOffsetX property (Office)

Gets or sets the _x_-axis offset of the image that is to be cropped. Read/write.


## Syntax

_expression_.**PictureOffsetX**

_expression_ An expression that returns a **[Crop](Office.Crop.md)** object.


## Return value

Single


## Remarks

**OffsetX** and **OffsetY** are relative to the center of the shape and image.


## Example

The following example inserts a 200 x 200 image into a PowerPoint presentation approximately in the center of the slide. It then resizes the image inside the frame to 100 x 100. The image frame stays at 200 x 200. The code then adds a square (the default shape) just above and to the right of the image, essentially cropping the lower-left corner of the image.


```vb
Sub CropImage() 
 ActivePresentation.Slides(1).Shapes.AddPicture "c:\myImage.png", msoFalse, msoTrue, 250,150, 200, 200 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.PictureHeight = 100 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.PictureWidth = 100 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.PictureOffsetX = 0 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.PictureOffsetY = 0 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.ShapeHeight = 100 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.ShapeWidth = 100 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.ShapeLeft = 330 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.ShapeTop = 170 
End Sub 

```


## See also

- [Crop object members](overview/library-reference/crop-members-office.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]