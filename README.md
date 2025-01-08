# Phishing com SEToolkit no Kali Linux

Este projeto demonstra a configuração e execução de um ataque de phishing utilizando a ferramenta **SEToolkit** no Kali Linux. O objetivo é criar um ambiente controlado para capturar credenciais de usuários como parte de um estudo de engenharia social.

---

## 🛠️ Ferramentas Utilizadas

- **Sistema Operacional:** Kali Linux
- **Ferramenta:** Social-Engineering Toolkit (SEToolkit)
- **Virtualização:** VirtualBox
  - Máquina virtual com Kali Linux para executar o ataque.
  - Máquina virtual com Windows 10 para simular o teste de credenciais.

> Todo o teste foi realizado em um ambiente virtualizado para maior segurança, isolando completamente o projeto do computador pessoal.

---

## 🖥️ Configurando o SEToolkit

1. Acesse o terminal como root:
> sudo su
2. insira a senha
> 
3. Inicie o SEToolkit:
> setoolkit
4. Escolha o tipo de ataque:
> Social-Engineering Attacks 
5. Selecione o vetor de ataque:
> Web Site Attack Vectors 
6. Escolha o método de ataque:
> Credential Harvester Attack Method 
7. Escolha a opção de clonar um site:
> Site Cloner 
8. Insira o IP da máquina para onde as credenciais serão enviadas
Caso o IP não seja exibido, utilize o comando:
> ifconfig
9. Forneça a URL do site que deseja clonar:
> ex: http://www.facebook.com

Após configurar, o SEToolkit criará um servidor local e capturará as credenciais inseridas no site clonado.
>Para o teste, utilizei uma VM com Windows 10. Com o navegador em modo anônimo, acessei a página falsa do Facebook usando o IP da VM Kali e inseri um login para simulação
![image](https://github.com/user-attachments/assets/f063ae4a-76fa-48d4-8380-76eebbb5add3)
