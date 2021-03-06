---
title: Overview of prebuilt AI models -  AI Builder | Microsoft Docs
description: Describes the prebuilt AI models that are available in AI Builder.
author: alanabrito
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 10/04/2019
ms.author: alanab
ms.reviewer: v-dehaas
---

# Language detection model

The prebuilt language detection model identifies the predominant language of a text document. The model analyses the text and returns the detected language and a numeric score between 0 and 1. Scores close to 1 indicate higher certainty in the result. The detected language is returned as the "script" of the language. For instance, for the phrase "I have a dog" it will return “en” instead of “en-US”. The response for languages that can't be detected is **unknown**.

## Use in Microsoft Flow

If you want to use this prebuilt model in Microsoft Flow, you can find more information in [Use language detection model in Microsoft Flow](flow-language-detection.md).  

## Supported language and data format

- Documents cannot exceed 5,120 characters.
- The language detection model can detect a wide range of languages, variants, dialects, and some regional or cultural languages. The exact list of languages for this feature isn't currently available

## Model output

If text is detected, the language detection model will output the following information:

- **Results**: A list of languages detected in the input text.
- **Language**: Script version of the language code (ex.: “en”, “fr”, “zh_chs”, “ru”)
- **Score**: Numeric value from 0 to 1 where values close to 1 indicate 100% certainty that the identified language is true 
