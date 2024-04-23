## Understanding publisher and message broker.

1. How many data your publlsher program will send to the message broker in one
run? <br>
    Jawabannya 5. Ini dapat dilihat di main.rs. Pada main, publish event dipanggil sebanyak 5 kali. Satu pemanggilan publish event mengirimkan satu data. Maka dari itu terdapat 5 data yang dikirimkan pada satu run. 
2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? <br>
    url tersebut menandakannya melakukan protokol AMQP. amqp:// menandakan bahwa sedang membuat koneksi menggunakan protokol AMQP. guest:guest menandakan username:password saat autentikasi. localhost:5672 merupakan hostname dan port dari server AMQP. Maka url tersebut menandakan bahwa program dikonfigurasi untuk disambungkan ke server AMQP lokal.

![alt text](image.png)
tampilan sebelum di run
<br><br>

![alt text](image-5.png)

![alt text](image-6.png)

2 screenshot di atas merupakan hasil setelah di run di publisher dan juga subscriber. Dan berhasil dilakukan, terkirim data melalui message broker. Terlihat pada console.

![alt text](image-7.png)
spike pada grafik menunjukkan message rates. Message rates imenunjukkan jumlah message yang dikirim tiap detiknya.