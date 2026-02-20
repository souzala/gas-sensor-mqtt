# Gas Sensor ESP32 + MQTT

Sistema embarcado para detecção de vazamento de gás com transmissão remota de dados via protocolo MQTT.

## 📌 Descrição

Este projeto implementa um sistema IoT baseado em ESP32 para monitoramento de gases inflamáveis em ambientes industriais ou domésticos.

O sistema realiza:
- Leitura contínua do sensor MQ-2
- Exibição local em LCD I2C
- Acionamento de alarme sonoro (buzzer)
- Agrupamento de leituras em fila circular
- Envio periódico de dados para broker MQTT
- Sincronização de horário via NTP

## 🏗 Arquitetura do Sistema

Sensor MQ-2 → ESP32 → Wi-Fi → Broker MQTT → Monitoramento remoto

## 🔧 Componentes Utilizados

- ESP32
- Sensor de gás MQ-2
- Display LCD 16x2 (I2C)
- Buzzer
- Broker: broker.hivemq.com
- Servidor NTP: pool.ntp.org

## 🌐 Comunicação

Protocolo utilizado: MQTT (Publish/Subscribe)

Tópico de publicação:
esp32/gasmonitor

## ⚙️ Funcionalidades

- Monitoramento em tempo real
- Alarme para valores acima do limite seguro
- Sincronização temporal via NTP
- Publicação de dados agrupados a cada 10 amostras
- Arquitetura IoT baseada em publish/subscribe

## 🚀 Aplicações

- Segurança industrial
- Monitoramento ambiental
- Laboratórios farmacêuticos
- Restaurantes e cozinhas industriais
- Sistemas de biodigestores

## ▶️ Simulação

Projeto desenvolvido e testado na plataforma Wokwi.
https://wokwi.com/projects/445455312530831361

https://www.youtube.com/watch?v=kNa4DrAVwxI
