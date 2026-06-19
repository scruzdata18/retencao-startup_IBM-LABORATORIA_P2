# Análise de Retenção de Coorte: Uma Startup Não Atingiu PMF

## 📊 A Pergunta

**Triplicar o investimento em aquisição de usuários é uma boa estratégia quando uma startup enfrenta churn alto?**

A resposta é: **não, não é**.

---

## 🎯 Por Que Isso Importa

Muitas startups lidam com a pressão de crescer: "Vamos trazer mais usuários, mais rápido." Mas se os usuários existentes saem em massa, adicionar mais combustível ao fogo é desperdício.

Este projeto demonstra como análise de coorte revela a verdade por trás dos números de superfície — e como esses insights devem informar decisões estratégicas.

---

## 📈 O Que Fizemos

Analisamos a base de **330 assinantes** de uma startup de serviços de assinatura, rastreando:

- **Retenção mensal e trimestral** de cada coorte (grupos de usuários que entraram no mesmo período)
- **Churn mensal e trimestral** (taxa de cancelamento)
- **Trajetória de vida** de cada coorte ao longo de 8 trimestres (2019–2020)

**Metodologia:** Análise de coorte clássica com formatação condicional de cores (verde = bom, amarelo = atenção, vermelho = problema).

**Ferramentas:** Google Sheets com QUERY, PROCV, LINS, COLS e mapa de calor.

---

## 🔴 Os Achados Principais

| Métrica | Valor | Interpretação |
|---------|-------|----------------|
| **Retenção T1 2019** | 97,87% | Entrada forte |
| **Retenção T4 2020** | 51,35% | Queda de **46 pontos** em 12 meses |
| **Estabilização** | T2 2020 em diante | Retenção "estanca" em ~51%, sem recuperação |
| **Churn médio geral** | 36,36% | Mais de 1/3 dos assinantes cancela |

**O gráfico-chave:** A série temporal de retenção vs. churn mostra degradação consistente — não é um blip isolado, é um padrão sistemático de perda de confiança no produto.

---

## 💡 Conclusão Executiva

### A startup **NÃO atingiu PMF** (Product-Market Fit)

Quando retenção cai 46 pontos percentuais em 12 meses e estabiliza em ~51%, isso sinaliza:

1. **Produto não resolve o problema adequadamente** para a maioria dos usuários
2. **Valor percebido < custo da assinatura** — usuários acham mais fácil sair do que ficar
3. **Expandir aquisição agora é um desperdício** — você estará trazendo mais pessoas para uma experiência que as faz sair

### ✅ Recomendação Estratégica:

| ❌ Não Faça | ✅ Faça Primeiro |
|------------|-----------------|
| Triplicar investimento em aquisição | Investigar por que users saem (entrevistas, análise de perfil de churn) |
| Escalar marketing agressivo | Melhorar o produto até retenção > 70% |
| Expandir para novos mercados | Monitorar retenção como KPI central |
| | Só depois que PMF estiver sólido, escalar aquisição |

---

## 📊 Visualizações Principais

### Retenção Mensal
![Retenção Mensal](https://github.com/sthefcruz18/retencao-startup_IBM-LABORATORIA_P2/blob/3ee82f31056bc53f49d86c1858bc088da2827725/1.retencao_mes.png)

### Retenção Trimestral
![Retenção Trimestral](https://github.com/sthefcruz18/retencao-startup_IBM-LABORATORIA_P2/blob/3ee82f31056bc53f49d86c1858bc088da2827725/2.retencao_trimestral.png)

### Churn Mensal
![Churn Mensal](https://github.com/sthefcruz18/retencao-startup_IBM-LABORATORIA_P2/blob/3ee82f31056bc53f49d86c1858bc088da2827725/3.churn_mensal.png)

### Churn Trimestral
![Churn Trimestral](https://github.com/sthefcruz18/retencao-startup_IBM-LABORATORIA_P2/blob/3ee82f31056bc53f49d86c1858bc088da2827725/4.churn_trimestral.png)

### Retenção vs. Rotatividade (Série Temporal)
![PMF](https://github.com/sthefcruz18/retencao-startup_IBM-LABORATORIA_P2/blob/3ee82f31056bc53f49d86c1858bc088da2827725/5.grafico_PMF.png)

---

## 🌍 Bridge to Education: Aplicando Análise de Retenção a Dados Educacionais

Este projeto demonstra análise de coorte e retenção em contexto comercial. A mesma metodologia pode ser aplicada a dados educacionais para responder perguntas críticas em políticas públicas:

- **Quais alunos persistem em cursos técnicos integrados ao ensino médio?**
- **Que fatores predizem conclusão vs. evasão?**
- **Como a oferta de EPT varia por região e impacta trajetórias de alunos?**

Essas questões são centrais para o design de políticas de educação profissional baseadas em evidências. Os métodos usados aqui — **análise de coorte, taxas de retenção, segmentação de grupos** — são diretamente transferíveis a dados públicos educacionais (Censo Escolar, SAEB, microdados de secretarias estaduais).

Assim como identificar "churn alto = não escale", na educação identificar "evasão alta = produto/oferta inadequados = antes de expandir, reformule".

---

## 📁 Como Reproduzir

1. **Clone este repositório**
   ```bash
   git clone https://github.com/scruzdata18/retencao-startup_IBM-LABORATORIA_P2.git
   ```

2. **Abra o arquivo de análise**
   - [Relatório no Google Sheets](https://docs.google.com/spreadsheets/d/1y_iBEGvKWOPkftDI58K9R7JkfAqJfYX04fuWH_akWRI/edit?usp=sharing)

3. **Etapas de análise:**
   - Importar e revisar dados
   - Organizar em coortes por data de entrada
   - Calcular retenção/churn mensal e trimestral
   - Aplicar formatação condicional (mapa de calor)
   - Identificar padrões de degradação

---

## 🎓 Competências Desenvolvidas

✅ Organizar dados em planilhas (formatação, filtros, ordenação)  
✅ Manipular dados com tabelas dinâmicas e conexão de fontes (PROCV, QUERY)  
✅ Entender Product-Market Fit e suas repercussões  
✅ Realizar análise de coorte com mapas de calor  
✅ Tomar decisões comerciais baseadas em dados  

---

## 📊 Dataset

- **Fonte:** [Andrew Chen - Cohort Analysis Spreadsheet](https://andrewchen.com/the-easiest-spreadsheet-for-churn-mrr-and-cohort-analysis-guest-post/)
- **Tipo:** Dados fictícios públicos
- **Período:** jan/2019 – dez/2020
- **Assinantes:** 330 usuários

---

## 🎬 Apresentação

📹 [Vídeo de Apresentação dos Resultados](https://www.loom.com/share/aed2a60b097c417cb03b572d457c8529)

---

## 📧 Contato

**Sthefany Cruz**  
Data Analyst | Ciência de Dados aplicada a Educação e Políticas Públicas  
📧 [sthefcruz18@gmail.com](mailto:sthefcruz18@gmail.com)  
🔗 [GitHub](https://github.com/scruzdata18) | [LinkedIn](https://www.linkedin.com/in/sthefcruz18/)

---

## 📚 Referências

- Análise de coorte: [Understanding Cohort Analysis - Intercom](https://www.intercom.com/blog/cohort-analysis/)
- Product-Market Fit: Sean Ellis, "Find Product/Market Fit"
- Métricas SaaS: [SaaS Metrics 101 - Forecastly](https://www.forentrepreneurs.com/saas-metrics-2/)
- Formação: Laboratoria + IBM — Certificação em Análise de Dados
