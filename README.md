# Module 09 Reflection

## Understanding publisher and message broker

1. Banyak data yang dikirim dalam satu kali run. Banyak data yang dikirim dalam sekali run program publisher ini adalah 
sebanyak 5 data message, yang setiap messagenya mengandung user id dan username.
2. Arti dari url amqp://guest://guest:guest@localhost:5672. Penggunaan url yang sama berarti protokol, akun yang
digunakan, dan server RabbitMQ dari subscriber dan publisher sama.

## Running RabbitMQ as message broker

![RabbitMQ dashboard screenshot](/assets/images/rabbitmq_dashboard.png)

## Sending and processing event

![console screenshot](/assets/images/message_consoles.png)
Ketika cargo run dijalankan publisher mengirim 5 message ke subscriber

## Monitoring chart based on publisher

![RabbitMQ message rates screenshot](/assets/images/rabbitmq_spikes.png)
Ketika publisher di run maka publisher akan mengirim sebuah message ke subscriber, sehingga pengiriman message
terdeteksi dalam grafik messages rates yang ada di RabbitMQ