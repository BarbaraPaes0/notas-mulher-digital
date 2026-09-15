# Lab Prático: Introdução às Redes Hierárquicas (Cisco Packet Tracer)

Neste laboratório prático, montei e configurei uma topologia de rede corporativa utilizando o modelo hierárquico de 3 camadas da Cisco: **Acesso, Distribuição e Núcleo (Core)**. Durante a atividade, realizei as conexões entre os dispositivos, configurei o endereçamento IP, utilizei a CLI do Cisco IOS e realizei testes de conectividade.

## Objetivo
Compreender na prática a função das três camadas da arquitetura de redes Cisco, praticar comandos básicos de CLI e verificar a comunicação entre os dispositivos por meio de testes de conectividade e análise de pacotes.

## Contexto
Atividade prática realizada durante a capacitação no programa **Mulher Digital**, com orientação e suporte da instrutora do curso.

## Passos Realizados

1. **Organização da topologia**
   * **Núcleo (Core):** 1 Roteador Cisco 4331.
   * **Distribuição:** 1 Switch Cisco 3650-24PS, com instalação do módulo de fonte AC Power Supply.
   * **Acesso:** 2 Switches Cisco 2960-24TT (`SW-Acesso-Lab` e `SW-Acesso-Sec`).
   * **Dispositivos finais:** 4 PCs, organizados nos setores `PC-Lab01`, `PC-Lab02`, `PC-Sec01` e `PC-Sec02`.

2. **Cabeamento e conexão das portas**
   * Conexão dos dispositivos utilizando cabos diretos (*Straight-Through*).
   * Conexão dos PCs aos respectivos switches de acesso.
   * Conexão dos switches de acesso ao switch de distribuição pelas interfaces `GigabitEthernet1/0/1` e `1/0/2`.
   * Conexão do switch de distribuição ao roteador Core, utilizando `GigabitEthernet1/0/24` e `GigabitEthernet0/0/0`.

3. **Configuração do endereçamento IP**
   * Configuração manual de endereço IP, máscara de rede e Gateway Padrão nos quatro PCs, utilizando **Desktop > IP Configuration**.

4. **Configuração do roteador via CLI**
   A interface `GigabitEthernet0/0/0` do Roteador Cisco 4331 foi configurada utilizando comandos do Cisco IOS:

   ```bash
   Router> enable
   Router# configure terminal
   Router(config)# interface gigabitEthernet 0/0/0
   Router(config-if)# ip address 192.168.1.1 255.255.255.0
   Router(config-if)# no shutdown
   Router(config-if)# exit
   ```

5. **Testes e validação**
   * Realização de testes de comunicação utilizando o comando `ping`, como `ping 192.168.1.20` e `ping 192.168.1.1`.
   * Utilização do modo **Simulation** do Packet Tracer para acompanhar o percurso dos pacotes.
   * Aplicação do filtro **ICMP** para visualizar a passagem da PDU pelas camadas de **Acesso → Distribuição → Núcleo**.

## Resultado e Aprendizados
A topologia foi configurada e os testes realizados apresentaram comunicação entre os dispositivos utilizados na atividade e o Gateway principal.

**Principais aprendizados:**
* Compreensão prática das funções das camadas de Acesso, Distribuição e Core.
* Interpretação de tabelas de endereçamento e mapeamento de portas.
* Prática com comandos básicos do Cisco IOS por meio da CLI.
* Realização de testes de conectividade com `ping`.
* Observação e análise de pacotes ICMP utilizando o modo Simulation do Cisco Packet Tracer.
