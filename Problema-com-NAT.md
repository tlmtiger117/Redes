# 15/03/26
# Problema com NAT em VM

- 1° Verifique o adaptador da vm (se tem NAT habilitado)
   - Dica: Utilize apenas um adaptador e configure o arquivo de rede da sua VM com um pra NAT e rede Interna(outro).
   - Comecei a fazer isso, e resolve a maioria das dores de cabeça relacionados a NAT.
     

- 2°Configure o arquivo de rede do seu host. No meu caso é esse aqui:
  
   - (KALI-LINUX)-Comando: sudo nano /etc/network/interfaces
   - Configure a sua ineterface(eth0,enp0s3...) com DHCP automático, Comando:
     
      - 1° auto eth0
      - 2° iface eth0 inet dhcp
      

- 3° Reativar a rede:
   - comandos: sudo ifdown eth0 && sudo ifup eth0 (Desativa e reativa a rede, pra adcionar a configuração)
      - Sempre olhe sua interface, ela pode ser diferente.
     

- 4° Testar a conexão:
   - Pingar o seu ip NAT
   - Pingar o seu roteador NAT
   - Pingar algum host externo(google.com, 8.8.8.8...)
     

- Fiz isso é resolveu o meu problema. Espero que isso possa ajudar alguém.






