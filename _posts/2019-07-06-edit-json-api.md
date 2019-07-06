---
published: false
---
## A New Post

### Pertama
Buat Resource
>> php artisan make:resource QuestionResource

### Kedua
pada controller yang bersangkutan tambahkan pada show seperti ini :  
```php
  public function show(Question $question)
    {
        return new QuestionResource($question);
    }
```
