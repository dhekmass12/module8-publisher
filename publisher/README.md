<ol>
    <li>5 (line 25-39)</li>
    <li>**amqp://guest:guest@localhost:5672** adalah alamat dari RabbitMQ server. guest:guest adalah credentialnya. guest pertama adalah usernamenya dan guest kedua merupakan passwordnya. localhost:5672 berarti menggunakan localhost dengan port 5672.</li>
</ol>

![](img.png "")
Publisher mengirimkan 5 events ke subscribernya
<br/>

![](img2.png "")
spike terjadi saat pesan/event dikirim.

![](img3.png "")
queuenya menjadi lebih panjang karena subscribernya hanya 1 saja.

![](img4.png "")
queuenya menjadi lebih panjang karena subscribernya ada banyak sehingga jika 1 subscriber tidak ready, maka akan dilimpahkan ke subscriber lainnya.