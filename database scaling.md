# Database Scaling

Ada dua teknik scaling
Vertical & Horizontal

## Vertical Scaling
    Yang paling gampang di scale (Upg Hardware)
    (-) Hardware ada limit juga
    (-) Harga hardware 
    Kurang worth cuman paling untuk sementara

## Horizontal Scaling
    Beli hardware juga tapi yang sama murah
    ex: tambah server bukan upgrade hardware
    (-) Bingung ambil dan nambah (select/insert) data di server
        ->solusi teknik routing/sharding data
            ->Logicnya yang sederhana biar ga bingung
                Insert Data
                (Sharding Algorithm) hashing terhadap primary key (ex email->interger->modulo sebanyak node/server)
                Searching
                Melakukan di semua shard(potongan) partisi
                    (-)Paging? Deep Paging Problem
                    Belum ada solving
                    Merubah menjadi rentang waktu / crieteria
                    (-)Server Mati Salah Satu DB
                        Teknik Replication-> data 2x lipat, didataruh di server berbeda

            ## Jangan Lakukan Manual serahkan ke Database yang sudah bagus (mongoDb, kasandra)

## Caching paling rekomendasi
    Lebih baik dilakukan di Database
    System -> chace/memory -> Database


Sumber : https://www.youtube.com/watch?v=wH5LZ6ALxpw