# desafio-azure-recursos

# ☁️ Azure Resource Provisioning Guide

Este repositório contém o passo a passo para a criação e configuração de recursos no Microsoft Azure utilizando o portal web. Ideal para iniciantes, times de desenvolvimento ou documentação de projetos.

## 📋 Pré-requisitos

- Conta ativa no [Microsoft Azure](https://portal.azure.com/)
- Permissão para criar recursos no seu grupo de recursos
- Conhecimentos básicos de cloud (opcional, mas recomendado)

---

## 🚀 Etapas para Criar Recursos no Azure

### 1. Acessar o Portal Azure
Acesse o [Portal do Azure](https://portal.azure.com/) e entre com sua conta Microsoft.

---

### 2. Criar um Grupo de Recursos (Resource Group)

1. Vá até **"Grupos de recursos"** no menu lateral
2. Clique em **"Criar"**
3. Preencha:
   - **Assinatura**: selecione a assinatura desejada
   - **Nome do grupo**: ex: `rg-projeto-demo`
   - **Região**: ex: `Brazil South`
4. Clique em **"Revisar + criar"** e depois em **"Criar"**

---

### 3. Criar um Recurso (Ex: App Service)

1. No menu lateral, clique em **"Criar um recurso"**
2. Selecione **"App Service"**
3. Preencha as informações:
   - **Nome**: `meu-app-service`
   - **Publicar**: Código / Docker / Contêiner
   - **Runtime stack**: Node.js / .NET / Java etc.
   - **Região**: `Brazil South`
   - **Grupo de recursos**: `rg-projeto-demo`
4. Clique em **"Revisar + criar"** e depois em **"Criar"**

---

### 4. Criar um Banco de Dados (Ex: Azure SQL Database)

1. Clique em **"Criar um recurso"** > **"Banco de Dados"** > **"SQL Database"**
2. Preencha:
   - **Nome**: `db-projeto`
   - **Servidor**: criar novo ou usar existente
   - **Grupo de recursos**: `rg-projeto-demo`
   - **Camada de preços**: definir conforme uso (Free, Basic, Standard, Premium)
3. Clique em **"Revisar + criar"** e depois em **"Criar"**

---

### 5. (Opcional) Criar um Armazenamento (Storage Account)

1. Vá em **"Criar um recurso"** > **"Armazenamento"** > **"Conta de armazenamento"**
2. Preencha os campos:
   - **Nome**: `storageprojetodemo`
   - **Região**: `Brazil South`
   - **Tipo de Redundância**: LRS
3. Clique em **"Revisar + criar"** e depois em **"Criar"**

---

## 🧾 Observações

- Use nomes padronizados para facilitar organização (ex: `app-`, `db-`, `rg-`, `storage-`)
- Cuidado com os custos: escolha camadas gratuitas ou de baixo custo em ambientes de desenvolvimento
- Utilize **Tags** nos recursos para facilitar o controle e governança

---

## 📦 Recursos Criados

| Recurso           | Nome               | Região        | Grupo de Recursos |
|-------------------|--------------------|----------------|--------------------|
| App Service       | `meu-app-service`  | Brazil South   | `rg-projeto-demo`  |
| SQL Database      | `db-projeto`       | Brazil South   | `rg-projeto-demo`  |
| Storage Account   | `storageprojetodemo`| Brazil South  | `rg-projeto-demo`  |

---

## 🛠️ Ferramentas recomendadas

- Azure CLI: https://learn.microsoft.com/pt-br/cli/azure/
- Azure Bicep: https://learn.microsoft.com/pt-br/azure/azure-resource-manager/bicep/overview
- ARM Templates: https://learn.microsoft.com/pt-br/azure/azure-resource-manager/templates/overview

---

## ✉️ Contribuições

Sinta-se à vontade para abrir issues ou pull requests com melhorias e atualizações.

---
