#  Branch

Branch yang artinya ranting adalah fungsi dari Git yang memudahkan kita untuk membuat berbagai cabang/versi dari aplikasi kita. Beberapa Perintah yang berkaitan


  - Git Branch
  - Git Merge
  - Git Checkout
  - Git Tag
 
### Git Branch

```sh
git branch –help              //untuk penjelasan lengkap branch
git branch -D <nama_branch>   //untuk menghapus branch
```

### Git Merge
Berfungsi untuk menyatukan branch. 

###### //Menyatukan secara fast-forward
```sh
git merge <nama_branch>             
```

###### //Menyatukan juga dengan metode commit,yang berarti mudah merawat atau maintence (no fast-forward)
```sh
git merge –no-ff <nama_branch>    
```

![alt text][logo]



### Git Checkout
Berfungsi untuk melakukan aktifasi, membuat, menghilangkan perubahan pada sebuah file atau direktori.
```sh
git checkout -b <nama_branch> //membuat & mengaktifkan branch
git checkout -b <nama_branch_new> <nama_branch_old> //menduplikasi branch lama
git checkout <nama_branch> //mengaktifkan branch
```

### Git Tag
Berfungsi untuk menandai repo dan kebanyakan pengguna menggunakan untuk menandai untuk versi aplikasi.

```sh
git tag -a <version> //pastinya untuk menandai versi 
git tag –list // untuk melihat semua list tag pada repo
git tag -d <version> //menghilangkan tanda versi repo
```

# Kelebihan memakai Branch:

  - Lebih mudah menelusuri kembali aplikasi yang sudah jadi untuk diperbaiki 
  - Tidak menyebabkan masalah untuk versi pada branch lain

### Sumber

* https://belajarwebdesign.com/web-programming/menggunakan-git-branch-dengan-optimal/
* https://git-scm.com/book/id/v1/Branching-Pada-Git-Apakah-Branch-Itu
### Blog Bule
* https://blog.jonathanoliver.com/my-new-best-friend-git-merge-no-ff/
### Artikel Berhubungan lainnya :
* http://nvie.com/posts/a-successful-git-branching-model/
* http://paul.stadig.name/2010/12/thou-shalt-not-lie-git-rebase-ammend.html

[logo]: https://i.stack.imgur.com/FMD5h.png "Beda no fast forward"