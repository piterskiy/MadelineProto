---
title: messages.readFeaturedStickers
description: messages.readFeaturedStickers parameters, return type and example
---
## Method: messages.readFeaturedStickers  
[Back to methods index](index.md)


### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|id|Array of [long](../types/long.md) | Yes|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **NO**


### Example:


```
$MadelineProto = new \danog\MadelineProto\API();
$MadelineProto->session = 'mySession.madeline';
if (isset($number)) { // Login as a user
    $MadelineProto->phone_login($number);
    $code = readline('Enter the code you received: '); // Or do this in two separate steps in an HTTP API
    $MadelineProto->complete_phone_login($code);
}

$Bool = $MadelineProto->messages->readFeaturedStickers(['id' => [long], ]);
```

Or, if you're using the [PWRTelegram HTTP API](https://pwrtelegram.xyz):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.readFeaturedStickers`

Parameters:

id - Json encoded  array of long




Or, if you're into Lua:

```
Bool = messages.readFeaturedStickers({id={long}, })
```

