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

### Ketiga
Pada Resource tambahkan seperti ini :  
```php
  public function toArray($request)
    {
        return [
          'title' => $this->title,
          'path' => $this->path,
          'body' => $this->body,
          'created_at' => $this->created_at,
          'user' => $this->user->name
        ];
        // kenapa name karena pada tabel questions telah direlasikan ke user jadi bisa didapatkan name user, ini untuk menghindari users tau id user tersebut ketka dikirim dengan API
    }
```

### Keempat

