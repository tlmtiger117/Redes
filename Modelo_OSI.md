# 06/03/26
# Modelo Osi

- O que é: É um framework(ferramenta conceitual nesse caso) utilizado para entender as camadas que um pacote faz até chegar no
          seu destino final:

- Tabela OSI:
  
- 1️° Física (Physical)
   - Transmite bits pelo meio físico (cabos, sinais elétricos/ópticos).
   - Ex: cabos, conectores, sinais.

- 2️° Enlace/amarração de Dados (Data Link)
   - Faz a comunicação entre dispositivos na mesma rede.
   - Controle de erro e uso de endereços MAC.

- 3°  Rede (Network)
   - Define roteamento e endereços IP para enviar dados entre redes diferentes.

- 4️° Transporte (Transport)
   - Garante entrega correta dos dados.
   - Pode ser confiável (TCP) ou mais rápido sem confirmação (UDP).

- 5️° Sessão/conexão estabelecida (Session)
   - Cria, mantém e encerra sessões de comunicação entre dispositivos.

- 6️° Apresentação/criptografia (Presentation)
   - Formata, criptografa e comprime os dados para que o sistema receptor entenda.

- 7️° Aplicação/processamento (Application)
   - Camada mais próxima do usuário.
   - Onde atuam protocolos como HTTP, FTP, SMTP.

- Após esse fluxo, o porcesso inverso acontece para o user receber as informações da conexão/Probe.

- [Dica para memorizar] (de baixo para cima):

   1°- Física(cabos,sinais) → 2°- Enlace(Ethernet/LAN) → 3° Rede(IP SRC e DST) → 4°Transporte(TCP/UDP) → 5° Sessão(SYN-ACK) →
   6° Apresentação(criptografia) → 7° Aplicação(processamento) -> processo inverso para o user receber os dados.


  
