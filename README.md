# 🏋️ FitManager - Sistema de Gestão para Academias

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)

O **FitManager** é uma solução completa de gestão multiacademia, desenvolvida para simplificar a administração de unidades de fitness, controle de alunos, prescrição de treinos e acompanhamento financeiro. Inspirado no modelo SCA, o sistema oferece isolamento total de dados e alta escalabilidade.

---

## 📖 Documentação e Planejamento

Para detalhes completos sobre requisitos, casos de uso, regras de negócio e cronograma, acesse:
👉 [**Documentação do Projeto no Notion**](https://www.notion.so/Projeto-FitManager-2e0301f1f4de80ad9865e6feed24ddd8?source=copy_link)

---

## 🚀 Funcionalidades Principais

### 🛡️ Gestão e Segurança
* **Multiacademia:** Suporte a múltiplas unidades com isolamento total (Multi-tenant).
* **Controle de Acesso (RBAC):** Perfis para Administradores e Professores com permissões distintas.
* **Autenticação:** Segurança via JWT (JSON Web Tokens) e criptografia de senhas com `bcrypt`.

### 👥 Gestão de Alunos e Planos
* **Financeiro:** Controle de mensalidades, histórico de pagamentos e alertas de inadimplência.
* **Frequência:** Controle de entrada (preparado para integração com QR Code).
* **Prontuário:** Cadastro de restrições de saúde, objetivos e evolução.

### 📋 Treinos e Avaliações
* **Fichas Digitais:** Prescrição detalhada (séries, repetições, carga e descanso).
* **Avaliação Física:** Cálculo automático de indicadores como IMC e registro de medidas.
* **Biblioteca de Exercícios:** Catálogo organizado por grupos musculares com suporte a mídia.

---

## 🛠️ Tecnologias Utilizadas

| Camada | Tecnologia | Descrição |
| :--- | :--- | :--- |
| **Frontend** | React.js | Interface dinâmica e SPA (Single Page Application). |
| **Estilização** | Tailwind CSS | Design moderno, responsivo e utilitário. |
| **Backend** | Node.js | API REST escalável utilizando Express. |
| **Banco de Dados** | PostgreSQL | Banco de dados relacional robusto. |
| **ORM** | Prisma / Sequelize | Abstração e segurança na manipulação de dados. |
| **Estado** | Context API | Gerenciamento de estado global da aplicação. |

---

## 📐 Estrutura do Banco de Dados (DER)

O modelo relacional foi projetado para garantir a integridade entre as unidades:
* **Academias:** Entidade pai que isola os dados.
* **Usuários:** Colaboradores vinculados a cada unidade.
* **Alunos:** Registros de clientes e seus respectivos planos.
* **Treinos & Exercícios:** Estrutura N:N para montagem de fichas personalizadas.
* **Pagamentos:** Fluxo de caixa e controle de acesso financeiro.

---

## 🎨 Experiência do Usuário (UX)

O sistema segue quatro pilares fundamentais:
1.  **Dashboard Visual:** Informações críticas (faturamento e alunos ativos) logo no primeiro acesso.
2.  **Agilidade:** Fluxos curtos para tarefas diárias (como dar presença ou criar treino).
3.  **Feedback:** Mensagens de sistema claras e padronizadas.
4.  **Dark Mode Aesthetic:** Identidade visual moderna em tons de **Verde e Preto**.

---

## 🏁 Como Rodar o Projeto

### Pré-requisitos
* Node.js (v18 ou superior)
* PostgreSQL rodando localmente ou via Docker

### Configuração

1. **Clone o repositório:**
```bash
git clone [https://github.com/DouglasFariasRodigues/FitManager.git](https://github.com/DouglasFariasRodigues/FitManager.git)
Configuração do Backend:

Bash

cd fitmanager/backend
npm install
# Crie um arquivo .env seguindo o .env.example
npm run migrate
npm run dev
Configuração do Frontend:

Bash

cd fitmanager/frontend
npm install
npm start
🔮 Futuras Implementações (Roadmap)
[ ] App Mobile do Aluno: Visualização de fichas de treino no celular.

[ ] Integração de Pagamentos: Gateway para pagamento automático (Cartão/Pix).

[ ] Check-in por QR Code: Automação de acesso via app.

[ ] Relatórios de BI: Gráficos avançados de retenção e crescimento.

Desenvolvido com foco em performance e gestão esportiva. 🚀

Caso precise de suporte ou queira contribuir com o projeto, sinta-se à vontade para abrir uma Issue ou enviar um Pull Request.


---

### O que incluí para ficar "profissional":
* **Badges de Tecnologia:** Selos coloridos que facilitam a identificação da stack.
* **Tabela Técnica:** Organização das ferramentas de forma limpa.
* **Callouts de Destaque:** Uso de ícones e negritos para guiar o olhar.
* **Instruções de Instalação:** Código formatado em blocos para fácil cópia.
* **Roadmap:** Lista de "To-do" com checkboxes para mostrar que o projeto tem visão de futuro.

**Deseja que eu crie também um arquivo `.env.example` para acompanhar este README e facilitar a configuração para outros desenvolvedores?**