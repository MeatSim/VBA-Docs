---
title: Model3DFormat.IncrementRotationZ method (Word)
keywords: vbawd10.chm151584882
f1_keywords:
- vbawd10.chm151584882
ms.prod: word
api_name:
- Word.Model3DFormat.IncrementRotationZ
ms.date: 04/11/2019
ms.localizationpriority: medium
---


# Model3DFormat.IncrementRotationZ method (Word)

Changes the rotation of the specified shape around the z-axis by the specified number of degrees. 


## Syntax

_expression_.**IncrementRotationZ** (_Increment_)

_expression_ A variable that represents a **[Model3DFormat](Word.Model3DFormat.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Increment_|Required|**Single**|Specifies how much (in degrees) the rotation of the model around the z-axis is to be changed. Any value can be provided, although any value will be effectively normalized into the range 0..360 degrees.|

## Remarks

Use the **[RotationZ](Word.Model3DFormat.RotationZ.md)** property to set the absolute rotation of the shape around the z-axis.

To change the rotation of a model around the x-axis, use the **[IncrementRotationX](Word.Model3DFormat.IncrementRotationX.md)** method. To change the rotation around the y-axis, use the **[IncrementRotationY](Word.Model3DFormat.IncrementRotationY.md)** method.


## Example

This example tilts a 3D model on _myDocument_ by 10 degrees. Shape one must be a 3D model for this code to have any effect.


```vb
Set myDocument = ActivePresentation.Slides(1)

myDocument.Shapes(1).Model3D.IncrementRotationZ 10
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]