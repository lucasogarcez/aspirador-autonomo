# Ideias Iniciais — Robô Aspirador Autônomo

## 🎯 Objetivo do projeto
Criar um robô aspirador que:
- Mapeie o ambiente com sensores.
- Aspire de forma inteligente (evitando áreas já cobertas).
- Retorne à base de carregamento sozinho.
- Funcione offline depois que o mapa estiver salvo.

## 🧠 Arquitetura geral
- ESP32 como controlador embarcado principal.
- PC com ROS para fase de mapeamento inicial (SLAM).
- Exportação do mapa em forma de matriz para o ESP32 usar depois.
- Comunicação ESP32 ↔ PC via Wi-Fi (MQTT ou HTTP).

## 🔌 Recarga automática
- Base com terminais de recarga conectados a uma fonte de 12,6V.
- Robô detecta sinal IR da base.
- Ao se aproximar, alinha e encosta nos terminais para iniciar recarga.

## 🤔 Coisas que quero testar ou decidir depois:
- Testar se o VL53L0X é preciso o suficiente para mapeamento em movimento.
- Ver se vale usar dois ESP32 (um pro controle, outro pro mapeamento simplificado).
- Se a odometria dos motores vai ser confiável ou se vai precisar de giroscópio.
- Pensar em um botão para "modo manual" (ativar/desativar limpeza).
- Adicionar sensores de queda (beirada de escada).

## 🛠️ Futuras melhorias (depois do MVP):
- Modo “seguir trajeto programado por app”.
- Câmera para reconhecimento de obstáculos maiores (tipo cadeira).
- Implementar detecção de ambientes diferentes (cômodos) por cor do piso ou tempo de deslocamento.
