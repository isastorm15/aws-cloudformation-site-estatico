# 🚀 AWS CloudFormation — Site Estático Automatizado

![AWS](https://img.shields.io/badge/AWS-CloudFormation-orange?logo=amazon-aws&logoColor=white)
![IaC](https://img.shields.io/badge/Infrastructure%20as%20Code-IaC-blue)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 🧭 Sobre o Projeto

Este projeto foi desenvolvido como parte de um **desafio da DIO**, com o objetivo de **automatizar a criação de uma infraestrutura AWS** para hospedar um **site estático** utilizando os serviços:

- 🪣 **Amazon S3** – armazenamento e hospedagem do site  
- 🌩️ **Amazon CloudFront** – CDN para distribuição global com HTTPS  
- ⚙️ **AWS CloudFormation** – automação completa da infraestrutura (IaC)

---

## 🧠 Objetivos de Aprendizagem

- Aplicar os conceitos aprendidos em um ambiente prático na AWS  
- Automatizar a infraestrutura com **CloudFormation**  
- Documentar o processo técnico de forma estruturada  
- Publicar o projeto no GitHub como portfólio técnico  

---

## 🏗️ Arquitetura da Solução

**Fluxo simplificado:**

Usuário 🌎 → CloudFront 🌩️ → S3 🪣 → Site Estático (HTML/CSS)

# 🚀 Passo a Passo da Implantação

## 🪄 1. Criar a infraestrutura na AWS
1. Acesse **AWS CloudFormation → Create stack**  
2. Escolha **With new resources (standard)**  
3. Faça upload do arquivo **`template_final.yaml`**  
4. Clique em **Next** e defina o nome da pilha (ex.: `site-estatico-stack`)  
5. **Next → Next → Create stack**  
6. Aguarde até o status **`CREATE_COMPLETE`**

---

## 🧱 2. Fazer upload dos arquivos do site
1. Vá para **Amazon S3 → Buckets**  
2. Clique no bucket criado automaticamente (ex.: `site-estatico-stack-sitebucket-xxxxx`)  
3. **Upload → Add files**  
4. Envie os arquivos:
   - `index.html`
   - `error.html`
5. Clique em **Upload**

---

## 🌐 3. Obter o link do site
1. Acesse **CloudFormation → Stacks → `site-estatico-stack`**  
2. Vá até a aba **Saídas (Outputs)**  
3. Copie o valor de **`SiteURL`** — algo como:
https://d1234abcdefg.cloudfront.net

yaml
Copiar código
4. Abra o link no navegador ✅

---

## 💻 Resultado Final
🎯 **Página publicada com sucesso!**  
🌟 Projeto finalizado utilizando **AWS CloudFormation**, **Amazon S3** e **Amazon CloudFront**.

---

## 🔒 Boas Práticas Adotadas
- ✅ Uso de **Object Ownership = BucketOwnerEnforced**  
- ✅ **Sem ACLs públicas** (compatível com o padrão atual da AWS)  
- ✅ Política de acesso mínima necessária: **`s3:GetObject`**  
- ✅ Deploy 100% automatizado via **Infrastructure as Code (IaC)**

---

## 🧩 Tecnologias Utilizadas
| Categoria                   | Serviço / Ferramenta   |
|----------------------------|------------------------|
| Infraestrutura como Código | AWS CloudFormation     |
| Armazenamento              | Amazon S3              |
| Distribuição de Conteúdo   | Amazon CloudFront      |
| Linguagem                  | YAML, HTML             |
| Hospedagem                 | AWS                    |

---

## 🧠 Aprendizados Principais
- Criação de **infraestrutura automatizada** com CloudFormation  
- Configuração **segura e moderna** de buckets S3  
- Entrega global via **CloudFront CDN**  
- Melhores práticas de **IaC (Infrastructure as Code)**  
- Documentação técnica e uso do **GitHub como portfólio**
