-> Meu primeiro escaneamento com o Nmap
O comando Nmap(Network Mapper) serve para mapeamento de redes. Para quem está começando no mundo Cyber, ele nos permite descobrir quais dispositivos estão online e encontrar brechas antes que cibercriminosos o façam.
Este passo a passo representa o mais básico da ferramenta, ideal para quem está dando os primeiros passos. Com o comando padrão, o que o nmap fornecerá de informações do alvo escaneado é:
quais são as  1.000 portas mais comuns(**) que estão abertas e escutando conexões, independentemente de estarem conectadas ativamente no momento no IP escaneado, e quais serviços podem estar rodando nessas portas.
---
- Como utilizar o comando "nmap"(Windows):
1. baixar a versão executável do Nmap no Windows
2. execute o instalador e prossiga
3. certifique-se de verificar se a instalação do Npcap está marcada(que é um complemento para o Nmap funcionar na rede)
4. abra o Prompt de Comando(CMD) ou o PowerShell e digite "nmap [seu endereço IP]"
5. caso não saiba seu IP, digite "ipconfig" e copie o Endereço IPv4 (depois execute o passo 4).

**Para escanear todas as portas seria necessário executar o comando "nmap -p- [IP]"
