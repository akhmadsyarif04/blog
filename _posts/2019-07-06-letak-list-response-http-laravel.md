---
layout: post
title: Letak List Response HTTP Pada Laravel
categories: Laravel
tags:
  - laravel
  - php
published: true
---
## Letak List response http pada laravel

lihat daftar respone pada file vendor/symfony/http-foundation/Response.php  

```php
public function destroy(Question $question)
    {
        $question->delete();
        // return response('Deleted', 201);
        // lihat daftar respone pada file vendor/symfony/http-foundation/Response.php
        return response(null, Response::HTTP_NO_CONTENT);

    }
```
