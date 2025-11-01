# Easy Invest

## 1. Informações Iniciais

**Nome do Projeto:** Easy Invest  
**Equipe:**  
- Marcus Vinicius Zelenato — RA: 22.223.084-9  
- Gustavo Teixeira Aquino — RA: 22.122.014-8  
- Mario Eugenio Silva — RA: 22.123.097-2  

**Data:** 22/08/2025  
**Correção:** 31/10/2025  

---

## 2. Modelo de Processo de Software

O modelo escolhido para o projeto foi o **incremental**, devido à sua flexibilidade e à natureza volátil do mercado financeiro.  
Com esse modelo, conseguimos lançar versões mínimas do produto de forma mais ágil, gerando valor ao usuário final desde as primeiras entregas.

Dessa forma, os investidores podem testar as versões iniciais e fornecer feedback em tempo real, evitando o desperdício de tempo com funcionalidades que não agregam valor.

Além disso, a plataforma pode nascer de maneira simples, otimizando o tempo de entrega inicial e evoluindo em complexidade com base nas interações e no retorno dos usuários.  
Isso torna o modelo incremental mais vantajoso que o modelo em cascata, no qual a descoberta de um erro conceitual apenas na fase final pode resultar em retrabalho caro e complexo.

---

## 3. Stakeholders

| **Papel** | **Interesse no sistema** |
|------------|----------------------------|
| **Pessoa com curiosidade sobre o mundo dos investimentos** | 1. Acompanhamento em tempo real das notícias e tendências do mercado financeiro, com alertas personalizados para os ativos de interesse.<br>2. Projetar a rentabilidade e simular o primeiro milhão, partindo do saldo inicial (R$ 0,00).<br>3. Participar de uma comunidade sobre investimentos, podendo ter acesso a chats com investidores.<br>4. Receber sugestão de carteira de investimento de acordo com a avaliação do tipo de perfil. |
| **Investidor** | Todas as funcionalidades do público anterior.<br>1. Simulação do primeiro milhão considerando o portfólio atual do investidor.<br>2. Consultoria virtual com especialistas: sessões de aconselhamento financeiro e suporte por chat ou vídeo com especialistas credenciados. |
| **Consultor** | 1. Acessar informações do perfil do investidor: visualizar dados, questionários e histórico de simulações.<br>2. Gerar sugestões de carteira de investimentos com base nos dados coletados.<br>3. Prestar consultoria com especialista: conduzir sessões de aconselhamento financeiro (chat, vídeo ou relatórios) diretamente pelo sistema. |

---

## 4. Perguntas de Entrevista

| **Stakeholder** | **Pergunta** |
|------------------|--------------|
| Ambos | Qual seu planejamento para chegar no primeiro milhão? |
| Ambos | Como você administraria seus aportes mensais para chegar no seu primeiro milhão? |
| Ambos | Como você escolheria sua carteira de investimentos? |
| Investidor | Quais as projeções para sua carteira de investimento? |
| Ambos | Como você aprende sobre o mercado financeiro? |
| Ambos | Com quem você conversa sobre o mercado financeiro? |
| Investidor | Qual sua visibilidade do seu portfólio de investimento? |
| Investidor | Quais os tipos de investimentos você tem atualmente? |
| Investidor | Você possui algum acompanhamento profissional? |
| Ambos | Como você acompanha as notícias do mundo financeiro? |

---

## 5. Requisitos Funcionais (RF)

### Simulação de Investimentos
- **RF01:** Oferecer a simulação do “primeiro milhão” de forma personalizada.

### Sugestões de Investimento
- **RF02:** Recomendação de carteira com base no perfil de risco do usuário.  
- **RF03:** Receber definição de perfil de investidor.  
- **RF04:** Alertas de risco e oportunidades do mercado.

### Portal de Conteúdo
- **RF05:** Disponibilizar notícias atualizadas do mercado financeiro.  
- **RF06:** Área de comunidade com fórum/chat para interação entre usuários.

### Capacitação dos Consultores
- **RF07:** Consultores especializados na área de economia.  
- **RF08:** Necessário certificação CEA.

### Consultoria Especializada
- **RF09:** Consultas com especialistas sobre o mercado financeiro.

### Análise de Usuários
- **RF11:** Questionário para avaliação do perfil de investimento do usuário.  
- **RF12:** Validação de CPF.

### Logar e Criar Conta
- **RF13:** Criar conta segura.  
- **RF14:** Logar como usuário.  
- **RF15:** Logar como consultor.

---

## 6. Requisitos Não Funcionais (RNF)

### Usabilidade
- **RNF01:** Interface responsiva e adaptada para mobile e desktop.  
- **RNF02:** Painel intuitivo, com gráficos e relatórios interativos.

### Segurança
- **RNF03:** Autenticação MFA.  
- **RNF04:** Acesso SSO.  
- **RNF05:** Criação de senha com 11 caracteres (caracteres especiais, números, letras minúsculas e maiúsculas).  
- **RNF06:** Criptografia ponta a ponta.

### Performance e Escalabilidade
- **RNF07:** O sistema deve suportar pelo menos 30.000 usuários simultâneos.  
- **RNF08:** Feedback de simulação em no máximo 3 segundos.

### Disponibilidade
- **RNF09:** Disponibilidade 24/7 e suporte via JIRA.  
- **RNF10:** Backups automáticos diários.

---

## 7. Restrições Técnicas

- O sistema deve ser desenvolvido para **web e mobile**.  
- Utilização de **APIs de mercado financeiro** para atualização de cotações e notícias.  
- Banco de dados **relacional (PostgreSQL/MySQL)** para dados transacionais e **NoSQL (MongoDB)** para notícias e histórico.

---

## 8. Regras de Negócio

- O usuário deve preencher seu **perfil de risco** (conservador, moderado ou arrojado) antes de receber recomendações.  
- Simulações devem considerar **inflação** e **taxas administrativas**.  
- Notícias exibidas devem ser sempre provenientes de **fontes confiáveis e verificadas**.  
- Consultorias virtuais só podem ser feitas com **especialistas credenciados**.  
- **Limite de uma conta por CPF/e-mail.**

- ## 9. Telas Do Prototipo
- Menu
<img width="735" height="494" alt="image" src="https://github.com/user-attachments/assets/aa723d25-b926-43d4-b2db-b7b08b05ad83" />

- Login/Cadastro
<img width="289" height="390" alt="image" src="https://github.com/user-attachments/assets/2f679602-96c0-49fe-a753-aca1beca8db7" />

-Menu
<img width="1326" height="595" alt="image" src="https://github.com/user-attachments/assets/665f5af2-7b47-4856-ab53-f341f5f24e5b" />

-Simulação do 1ºMilhão
<img width="1344" height="594" alt="image" src="https://github.com/user-attachments/assets/ca277561-a466-4e03-a3a8-d91e113faef2" />
<img width="1338" height="585" alt="image" src="https://github.com/user-attachments/assets/2482fd7f-cbba-424f-8792-5c7b92fc545b" />

-Analise de Perfil e Recomendação de Carteira
<img width="1333" height="591" alt="image" src="https://github.com/user-attachments/assets/e439f99d-b286-4a1c-9fc0-23b403ed5779" />
<img width="1159" height="589" alt="image" src="https://github.com/user-attachments/assets/ade727ec-17dd-4186-91e1-b8032afc82b1" />

-Painel de Noticias
<img width="1173" height="581" alt="image" src="https://github.com/user-attachments/assets/976a2047-c657-40c6-98c0-e1d71937cc79" />

- Comunidade de Conversas
<img width="1180" height="552" alt="image" src="https://github.com/user-attachments/assets/923dfb5f-39fb-45fe-bf38-28e43344c64c" />

- Agendamento de Consultoria
<img width="1332" height="592" alt="image" src="https://github.com/user-attachments/assets/bcb59cc0-f639-4aee-b2d5-3e934815a80a" />



