# 1. Informações Iniciais

**Nome do Projeto:** Easy Invest  
**Equipe:**  
- Marcus Vinicius Zelenato – RA: 22.223.084-9  
- Gustavo Teixeira Aquino – RA: 22.122.014-8
- Mario Eugenio Silva - RA: 22.123.097-2  

---

# 2. Modelo de Processo de Software

O modelo escolhido para o projeto foi o **incremental**, devido à sua flexibilidade e à natureza volátil do mercado financeiro. Com esse modelo, conseguimos lançar versões mínimas do produto de forma mais ágil, gerando valor ao usuário final desde as primeiras entregas. Dessa forma, os investidores podem testar as versões iniciais e fornecer feedback em tempo real, o que evita o desperdício de tempo com funcionalidades que não agregam valor.

Além disso, a plataforma pode nascer de maneira simples, otimizando o tempo de entrega inicial e evoluindo em complexidade com base nas interações e no retorno dos usuários. Isso torna o modelo incremental mais vantajoso que o modelo em cascata, no qual a descoberta de um erro conceitual apenas na fase final pode resultar em retrabalho caro e complexo.

---

# 3. Stakeholders

| **Papel** | **Interesse no sistema** |
|----------|---------------------------|
| Pessoa com curiosidade sobre o mundo dos investimentos | Este stakeholder representa o usuário iniciante, que possui interesse crescente em finanças e investimentos, mas ainda está em fase de aprendizado e exploração. Ele busca uma porta de entrada acessível e educativa para o universo financeiro, valorizando recursos que ensinem, simulem e informem de forma clara e prática. |
| Investidor | Este stakeholder já está ativo no mercado financeiro, possui investimentos em diferentes ativos e busca ferramentas de gestão, monitoramento e apoio estratégico para potencializar seus resultados e tomar decisões mais embasadas. Tem um nível de maturidade maior em comparação ao curioso, e exige funcionalidades avançadas que otimizem sua experiência. |

---

# 4. Perguntas de Entrevista

**Elabore 10 perguntas que seriam feitas aos stakeholders.**

| **Stakeholder** | **Pergunta** |
|------------------|--------------|
| Ambos stakeholders | Qual seu planejamento para chegar no primeiro milhão? |
| Ambos stakeholders | Como você administraria seus aportes mensais para chegar no seu primeiro milhão? |
| Ambos stakeholders | Como você escolheria sua carteira de investimentos? |
| Investidor | Quais as projeções para sua carteira de investimento? |
| Ambos stakeholders | Como você aprende sobre o mercado financeiro? |
| Ambos stakeholders | Com quem você conversa sobre o mercado financeiro? |
| Investidor | Qual sua visibilidade do seu portfólio de investimento? |
| Investidor | Quais os tipos de investimentos você tem atualmente? |
| Investidor | Você possui algum acompanhamento profissional? |
| Ambos stakeholders | Como você acompanha as notícias do mundo financeiro? |

---

# 5. Requisitos Funcionais (RF)

### Simulação de Investimentos
- **RF01:** Permitir ao usuário simular aportes mensais, taxa de rentabilidade e prazo para atingir metas.  
- **RF02:** Oferecer a simulação do “primeiro milhão” de forma personalizada.

### Gestão de Carteira
- **RF03:** Exibir visão consolidada de investimentos de diferentes corretoras.  
- **RF04:** Permitir comparação entre diferentes ativos e corretoras.

### Sugestões de Investimento
- **RF05:** Recomendação automática de carteira com base no perfil de risco do usuário.  
- **RF06:** Alertas de risco e oportunidades do mercado.

### Portal de Conteúdo
- **RF07:** Disponibilizar notícias atualizadas do mercado financeiro.  
- **RF08:** Área de comunidade com fórum/chat para interação entre usuários.

### Capacitação dos Consultores
- **RF09:** Consultores especializados na área de economia.  
- **RF10:** Necessário certificação CEA.

### Análise de Usuários
- **RF11:** Questionário para avaliação do perfil de investimento do usuário.  
- **RF12:** Validação de CPF.

---

# 6. Requisitos Não Funcionais (RNF)

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
- **RNF08:** Feedback de simulação de no máximo 3 segundos.

### Disponibilidade
- **RNF09:** Disponibilidade 24/7 e suporte via JIRA.  
- **RNF10:** Backups automáticos diários.

---

# 7. Restrições Técnicas

- O sistema deve ser desenvolvido para **web e mobile**.  
- Utilização de **APIs de mercado financeiro** para atualização de cotações e notícias.  
- **Banco de dados relacional** (ex.: PostgreSQL/MySQL) para dados transacionais e **NoSQL** (ex.: MongoDB) para notícias e histórico.

---

# 8. Regras de Negócio

- Usuário deve preencher seu perfil de risco (conservador, moderado, arrojado) antes de receber recomendações.  
- Simulações devem considerar **inflação e taxas administrativas**.  
- Notícias exibidas devem ser sempre provenientes de **fontes confiáveis e verificadas**.  
- Consultorias virtuais só podem ser feitas com **especialistas credenciados**.  
- Limite de **uma conta por CPF/e-mail**.

---
