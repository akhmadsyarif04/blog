---
layout: post
title: Edit Send Request API Json
categories: Laravel
tags:
  - laravel
  - php
published: true
---
## Edit Send Request API Json

### Pertama
Buat Resource
>> php artisan make:resource QuestionResource

### Kedua
pada controller yang bersangkutan tambahkan/edit pada show dan index seperti ini :  
```php
  public function index()
    {
        return QuestionResource::collection(Question::latest()->get()); // agar mengikuti aturan dari resource
    }
    
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
          'title' => $this->title, // kolom pada table database question
          'path' => $this->path,
          'body' => $this->body,
          'created_at' => $this->created_at,
          'user' => $this->user->name // ambil dari function user yang ada pada models questions yg telah direlasikan
        ];
        // kenapa name karena pada tabel questions telah direlasikan ke user jadi bisa didapatkan name user, ini untuk menghindari users tau id user tersebut ketka dikirim dengan API
    }
```

### Keempat
Pada models yang bersangkutan tambahkan :
```php
  public function getPathAttribute()
    {
      return asset("api/question/$this->slug");
    }
```

secara lengkap lihat pada project : [https://github.com/akhmadsyarif04/Real-Time-Single-Page-Forum-App-with-Pusher-Laravel-vuejs](https://github.com/akhmadsyarif04/Real-Time-Single-Page-Forum-App-with-Pusher-Laravel-vuejs)
