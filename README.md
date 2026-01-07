# 🐉 Guia de Instalação Kali Linux

![Kali Banner](https://www.kali.org/images/kali-logo.svg)

Este repositório fornece um guia simplificado para a instalação do **Kali Linux**.

---

## 📋 Sumário
- [Pré-requisitos](#-pré-requisitos)
- [Downloads](#-downloads)
- [Criando Mídia de Instalação](#-criando-mídia-de-instalação)
- [Passo a Passo da Instalação](#-passo-a-passo-da-instalação)
- [Primeiros Passos (Pós-Instalação)](#-primeiros-passos-pós-instalação)

---

## 📌 Pré-requisitos

Requisitos mínimos:

* **Espaço em Disco:** Mínimo de 20GB (Recomendado: 50GB+).
* **Memória RAM:** Mínimo de 2GB (Recomendado: 8GB para melhor desempenho).
* **Arquitetura:** Processador de 64 bits.
* **Pendrive:** Mínimo de 8GB de capacidade.

---

## 📥 Downloads

Para garantir a segurança, baixe sempre as imagens das fontes oficiais:

1.  **ISO do Kali Linux:** [Página de Downloads Oficial](https://www.kali.org/get-kali/)
2.  **Rufus (Para Windows):** [Site Oficial](https://rufus.ie/) - Utilizado para criar o pendrive bootável.
3.  **BalenaEtcher (Multiplataforma):** [Site Oficial](https://www.balena.io/etcher/) - Alternativa ao Rufus.

---

## 💾 Criando Mídia de Instalação

1. Conecte o pendrive ao seu computador.
2. Abra o **Rufus**.
3. Em **Dispositivo**, selecione o seu pendrive.
4. Em **Seleção de Boot**, clique em `SELECIONAR` e escolha o arquivo `.iso` baixado.
5. Clique em `INICIAR`. 
    Se solicitado, escolha o modo "Gravar em modo Imagem ISO".*
6. Aguarde a conclusão e seu pendrive estará pronto.

---

## 🖥️ Passo a Passo da Instalação

1.  **Boot:** Insira o pendrive no PC, reinicie e acesse o menu de boot (geralmente `F12`, `F11`, `F10` ou `ESC`).
2.  **Menu Inicial:** Selecione a opção `Graphical Install`.
3.  **Localização:** Selecione `Portuguese (Brazil)` e o layout do teclado como `Português Brasileiro (ABNT2)`.
4.  **Rede:** * **Nome da máquina:** Escolha um nome (ex: `kali`).
    * **Nome de domínio:** Pode ser deixado em branco.
5.  **Usuários e Senhas:** Crie o seu nome de usuário e defina uma senha segura.
6.  **Particionamento:**
    * Para iniciantes: Escolha `Assistido - usar o disco inteiro`.
    * *Atenção: Isso apagará todos os dados do disco selecionado.*
7.  **Seleção de Software:** Mantenha as opções padrão (Desktop Environment XFCE e ferramentas recomendadas).
8.  **Carregador de Inicialização (GRUB):** Quando perguntado se deseja instalar o GRUB na unidade principal, selecione `Sim`.

---

## 🛠️ Primeiros Passos (Pós-Instalação)

Após o primeiro login, abra o terminal e execute os comandos abaixo para garantir que o sistema esteja atualizado:


# Atualizar a lista de pacotes
sudo apt update

# Atualizar o sistema completo
sudo apt full-upgrade -y

# Reiniciar para aplicar mudanças de Kernel, se houver
reboot

## Comandos adicionais úteis:

ip a: Verificar endereço IP.

sudo apt install nome-do-pacote: Instalar novas ferramentas.
