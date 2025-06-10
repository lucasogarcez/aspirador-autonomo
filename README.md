# 🤖 Robô Aspirador Autônomo com Mapeamento e Retorno à Base

Projeto pessoal de um robô aspirador de pó com mapeamento de ambiente (SLAM) e retorno automático à base de recarga. A proposta é utilizar um ESP32 (e eventualmente um Arduino Uno) em conjunto com um PC rodando ROS para processar os dados de sensores.

## 🔧 Estrutura

- `firmware/`: código-fonte embarcado para ESP32 e Arduino.
- `pc-side/`: scripts e configurações ROS usados no PC para SLAM e mapeamento.
- `hardware/`: lista de componentes, esquemas e ligações dos módulos.
- `docs/`: anotações, ideias e registro de progresso durante o desenvolvimento.

## ✅ Objetivo final
- Robô capaz de:
  - Mapear o ambiente.
  - Aspirar seguindo trajetórias planejadas.
  - Retornar à base de carregamento de forma autônoma.

## 🚧 Status atual
- [x] Planejamento da arquitetura
- [ ] Integração de sensores com ESP32
- [ ] Comunicação ESP32 ↔ ROS
- [ ] Mapeamento SLAM com GMapping
- [ ] Navegação offline com mapa salvo
- [ ] Implementação da base de recarga
- [ ] Projeto final pronto

## 🧠 Autor
Desenvolvido por Lucas Oliveira Garcez. Projeto documentado aos poucos, conforme o tempo permitir 😅
