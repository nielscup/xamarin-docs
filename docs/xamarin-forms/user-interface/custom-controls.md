---
title: "Create a custom control with Xamarin.Forms"
description: "Buid a custom control using Xamarin.Forms, without a custom renderer."
ms.prod: xamarin
ms.assetid: 1689718E-5508-40E9-96A5-04D0C00BEF81
ms.technology: xamarin-forms
author: mshwf
ms.author: crdun
ms.date: 05/23/2019
---
# Create a custom control with Xamarin.Forms

The process of building UI elements requires, at some point, some customizations to give the unique feel and look to the application and to extend the functionality of existing controls. Whether the customization is just overriding the default TextColor of the Entry or creating a brand new control with new look and behavior, building custom controls can provide the simple solution to achieve that, without the need of custom renderers.

The process for creating custom controls is as follows:

1. Create a subclass of the view you want to extend or modify.
2. Alter the functionality of the subclass by overriding the default value of the base class’s bindable properties and/or create new bindable properties that will interact with user actions.
3. Process inputs through the `propertyChanged` delegate of the newly added bindable properties.

## Create a custom Toggle bar

