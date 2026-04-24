# 💻 Criando uma Máquina Virtual no Azure

## 📌 O que é uma Máquina Virtual (VM)?
Uma **Máquina Virtual (VM)** no Azure é um servidor virtual que roda na nuvem, permitindo executar sistemas operacionais e aplicações.

👉 Faz parte do modelo **IaaS (Infrastructure as a Service)**

---

## ⚙️ Passo a passo para criar uma VM

### 🔹 1. Acessar o portal
- Entre no portal do Azure: https://portal.azure.com

---

### 🔹 2. Criar o recurso
- Clique em **"Máquinas Virtuais"**
- Clique em **"Criar" > "Máquina Virtual"**

---

### 🔹 3. Configurações básicas

Preencha os principais campos:

- **Assinatura** → ex: Azure for Students  
- **Grupo de Recursos** → criar novo ou usar existente  
- **Nome da VM** → ex: `vm-estudos-az900`  
- **Região** → ex: Brazil South  
- **Imagem** → ex: Ubuntu Server ou Windows Server  
- **Tamanho (SKU)** → define CPU e memória  

---

### 🔹 4. Configurar acesso

- **Usuário administrador**
- **Senha ou chave SSH** (recomendado para Linux)

---

### 🔹 5. Configurar portas de entrada (inbound)

- Liberar portas conforme necessidade:
  - **22** → SSH (Linux)
  - **3389** → RDP (Windows)

---

### 🔹 6. Configurar disco

- Escolher tipo:
  - HDD (mais barato)
  - SSD (melhor desempenho)

---

### 🔹 7. Revisar e criar

- Clique em **"Revisar + Criar"**
- Depois em **"Criar"**

👉 A VM será provisionada em alguns minutos

---

## 🔌 Como acessar a VM

### Linux:
- Via SSH:
```bash
ssh usuario@ip-publico
