# Subscriber App

## Reflection
> What is `amqp`?

`amqp` adalah singkatan dari **Advanced Message Queuing Protocol**. Ini merupakan sebuah protokol untuk mengirim dan menerima suatu *message* dari berbagai servis ke servis-servis lain. *Message* yang dimaksud disini merupakan data yang dikirimkan melalui internet sebagai suatu *stream of bytes*. `amqp` juga merupakan protokol pada lapisan aplikasi, seperti layaknya `HTTP` dan `HTTPS`. Dalam penggunaan `amqp`, *message* yang diterima bisa dikirimkan dari satu poin ke poin yang lain, atau bisa juga seperti model *publisher* dan *subcsriber* yang akan dilakukan pada tutorial ini. 

> What does "guest:guest@localhost:5672" means? What is the first "guest", the second "guest", and what is "localhost:5672" for?

Pada uri "guest:guest@localhost:5672", `guest` yang pertama menandakan username dari akun yang akan digunakan untuk dihubungkan dengan sesi `amqp`. `guest` yang kedua menandakan password dari username yang digunakan. `localhost` menandakan bahwa sesi `amqp` yang akan disambungkan adalah sesi `amqp` yang berada pada mesin lokal saya. `5672` disini menandakan port dimana sesi `amqp` ini berjalan pada `localhost`. Secara keseluruhan, uri "guest:guest@localhost:5672" menandakan bahwa *subscriber* akan menyambungkan dirinya dengan sesi `amqp` yang berjalan di `localhost:5672` dan menggunakan username dan password `guest`.
