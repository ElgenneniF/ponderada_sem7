# ponderada_sem7

Video: 


Durante a demonstração, configurei o ESP32 para monitorar a intensidade do sinal Wi-Fi (em dBm), enviando os dados para a plataforma Ubidots via MQTT e exibindo-os no monitor serial. Comecei na sala, onde permaneci por cerca de 10 segundos. Nesse momento, a conexão estava estável, com o ESP32 transmitindo os dados em tempo real para a nuvem.

Saí da sala e segui em direção à catraca principal. Durante o trajeto, os valores de dBm começaram a oscilar, mas a conexão MQTT permaneceu ativa, e os dados continuavam a ser registrados e enviados para o Ubidots. Após passar pela catraca, entrei no elevador para ir ao segundo andar. Assim que o elevador começou a se mover, a conexão Wi-Fi foi completamente perdida devido à interferência e ao ambiente fechado. Sem conexão Wi-Fi, o protocolo MQTT foi interrompido, e o ESP32 parou de medir, já que dependia da conectividade para funcionar. Durante todo o tempo no elevador, nenhum dado foi registrado ou transmitido.

Ao sair do elevador no segundo andar, o ESP32 reconectou-se automaticamente à rede Wi-Fi, e a conexão MQTT foi restabelecida. Assim que isso aconteceu, o dispositivo retomou as medições e os envios de dados. Caminhei em direção ao laboratório, onde o sinal estabilizou novamente, com os valores de dBm retornando a níveis normais e a transmissão de dados fluindo sem interrupções.

De lá, segui para o mezanino 2, próximo à sala R09. Durante o trajeto, o sinal apresentou algumas oscilações, mas a conexão foi mantida na maior parte do tempo, permitindo que os dados fossem registrados continuamente. Em um pequeno ponto de sombra da rede, a conexão caiu por alguns segundos, interrompendo temporariamente o envio de dados, mas foi rapidamente restabelecida.

Ao decidir retornar ao térreo, utilizei novamente o elevador. Assim como na subida, não havia sinal Wi-Fi dentro do elevador, e a conexão foi perdida novamente. O ESP32 parou de medir e transmitir até que eu saísse do elevador no térreo, onde o dispositivo reconectou à rede e voltou a funcionar normalmente. Passei novamente pela catraca principal e segui para a lanchonete, onde a conexão foi perdida, até chegar la.

Depois de sair da lanchonete, deixei o campus e comecei a atravessar a rua. Durante a travessia, a intensidade do sinal Wi-Fi diminuiu rapidamente, e a conexão MQTT foi perdida por completo. Com isso, o ESP32 parou de registrar os dados, já que dependia do envio em tempo real. Enquanto isso acontecia, acabei tropeçando e caindo na rua.
