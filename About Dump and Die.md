# Die Dump & Dump by Andi Syafrianda
Laravel memberi kita pilihan metode untuk Debugging yaitu dd() dan dump()

## Method dd() dan dump()
contoh dd()
```
    $posts = Post::where('status','published')->get();
    dd($posts); // Here dd() will dump the resultset and stop the execution.

```

Pada Laravel 5.5, kita dapat memakai dd() dan dump() secara langsung dalam satu instance. Metode debugnya membuat lebih mudah.

```
    $posts = Post::all();
    $posts->dump()
      ->sortBy('created_at')
      ->dump()
      ->take(10)
      ->pluck('post_title')
      ->dd() // here dd will dump the resulst and stops the execuation. 
      ->take(1);
```

## Perbedaan antara dd() dan dump()
Kedua fungsi digunakan untuk debuging. Tetapi mempunyai satu perbedaan. yaitu :
dump() outputnya adalah suatu hasil dan melanjutkan proses,
dd() outputnya adalah suatu hasil tapi memberhentikan proses dengan segera.
dd seperti melakukan proses dump() dan die()
