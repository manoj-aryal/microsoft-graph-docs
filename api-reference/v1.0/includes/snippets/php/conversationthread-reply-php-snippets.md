---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new ReplyPostRequestBody();
$post = new Post();
$postBody = new ItemBody();
$postBody->setContentType(new BodyType('text'));

$postBody->setContent('content-value');


$post->setBody($postBody);

$requestBody->setPost($post);


$graphServiceClient->groupsById('group-id')->threadsById('conversationThread-id')->reply()->post($requestBody);


```