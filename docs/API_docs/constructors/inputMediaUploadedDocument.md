---
title: inputMediaUploadedDocument
description: inputMediaUploadedDocument attributes, type and example
---
## Constructor: inputMediaUploadedDocument  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|nosound\_video|[Bool](../types/Bool.md) | Optional|
|file|[InputFile](../types/InputFile.md) | Yes|
|thumb|[InputFile](../types/InputFile.md) | Optional|
|mime\_type|[string](../types/string.md) | Yes|
|attributes|Array of [DocumentAttribute](../types/DocumentAttribute.md) | Yes|
|stickers|Array of [InputDocument](../types/InputDocument.md) | Optional|
|ttl\_seconds|[int](../types/int.md) | Optional|



### Type: [InputMedia](../types/InputMedia.md)


### Example:

```
$inputMediaUploadedDocument = ['_' => 'inputMediaUploadedDocument', 'nosound_video' => Bool, 'file' => InputFile, 'thumb' => InputFile, 'mime_type' => 'string', 'attributes' => [DocumentAttribute], 'stickers' => [InputDocument], 'ttl_seconds' => int];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "inputMediaUploadedDocument", "nosound_video": Bool, "file": InputFile, "thumb": InputFile, "mime_type": "string", "attributes": [DocumentAttribute], "stickers": [InputDocument], "ttl_seconds": int}
```


Or, if you're into Lua:  


```
inputMediaUploadedDocument={_='inputMediaUploadedDocument', nosound_video=Bool, file=InputFile, thumb=InputFile, mime_type='string', attributes={DocumentAttribute}, stickers={InputDocument}, ttl_seconds=int}

```


