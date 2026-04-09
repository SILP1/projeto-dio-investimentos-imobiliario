# ⚙️ Prompts Reutilizáveis: Templates para Futuras Consultas

## Como Usar Esta Biblioteca

Cada prompt abaixo é um **template** pronto para usar:
1. Copie o prompt exato
2. Substitua os [COLCHETES] pelos valores reais
3. Cole em seu buscador (NotebookLM, ChatGPT, Claude, etc)
4. Ajuste conforme necessário

**Dica Pro**: Estes prompts foram testados e otimizados. Use-os como está 
para melhores resultados.

---

## 📋 CATEGORIA 1: ANÁLISE DE FIIs ESPECÍFICOS

### Prompt 1.1: Análise Completa de um FII

**Situação**: Você encontrou um FII interessante e quer analisá-lo a fundo.

**Prompt**:
```
Faça uma análise completa do FII [TICKER DO FII]. 
Estruture sua resposta assim:

1. RESUMO: O que é, qual segmento, principais características
2. FUNDAMENTOS ATUAIS:
   - DY (últimos 12 meses)
   - P/VPA
   - Taxa de ocupação
   - Histórico de dividendos (crescendo ou caindo?)
3. COMPARAÇÃO COM PARES: 
   - Compare com 2-3 FIIs similares do mesmo segmento
   - Qual é mais atrativo?
4. AVALIAÇÃO: Compra agora ou espera?
5. RISCOS: Quais são os principais riscos específicos deste FII?
6. PRÓXIMAS CATALISTAS: O que monitorar nos próximos 3-6 meses?
```

**Exemplo de preenchimento**:
```
Faça uma análise completa do FII LOGR3...
```

---

### Prompt 1.2: Comparação Entre Dois FIIs

**Situação**: Você está entre dois FIIs e não sabe qual escolher.

**Prompt**:
```
Compare os FIIs [TICKER 1] e [TICKER 2]. 

Crie uma tabela com:
- DY histórico (12m)
- P/VPA
- Taxa de ocupação
- Rentabilidade 12 meses
- Taxa de administração
- Histórico de dividendos (últimos 3 anos se possível)

Depois, para cada critério, indique qual é melhor: [1 ou 2]

Conclusão: Qual você compraria e por quê?
```

---

### Prompt 1.3: Avaliação de Risco de um FII

**Situação**: FII apresenta DY muito alto e você quer entender se é risco.

**Prompt**:
```
Avalie o risco do FII [TICKER]. 

Checklist de risco:
1. DY está acima da média do segmento? Por quê?
2. Histórico de dividendos: aumentou, manteve ou caiu?
3. Taxa de ocupação: está acima de 90%?
4. Há notícias recentes negativas?
5. Saúde financeira: patrimônio está crescendo?
6. Qual é o maior risco específico deste FII?

Conclusão: É seguro investir ou há sinais de alerta?
```

---

## 📈 CATEGORIA 2: ACOMPANHAMENTO MENSAL/TRIMESTRAL

### Prompt 2.1: Revisão Trimestral da Carteira

**Situação**: Você precisa revisar sua carteira a cada trimestre.

**Prompt**:
```
Ajude-me a revisar minha carteira de FIIs para [MÊS/ANO].

Minha carteira:
- [TICKER 1]: [Quantidade] cotas
- [TICKER 2]: [Quantidade] cotas
- [TICKER 3]: [Quantidade] cotas
[continuar...]

Para cada FII, analise:
1. Divulgou resultado trimestral? Como foi?
2. Dividendo aumentou ou diminuiu? Por quê?
3. Há mudanças nos fundamentos?
4. Ainda faz sentido manter ou considerar vender?

Responda também:
- Minha carteira ainda está bem diversificada?
- Preciso rebalancear (ajustar pesos)?
- Há oportunidades para comprar mais de algum FII?
```

---

### Prompt 2.2: Monitoramento Mensal Rápido

**Situação**: Você quer acompanhar rapidinho sem entrar em muitos detalhes.

**Prompt**:
```
Resumo mensal do FII [TICKER] para [MÊS/ANO]:

1. Qual foi a performance do FII neste mês?
2. Alguma notícia importante?
3. Dividendo está em dia?
4. Algum sinal de alerta que eu deva ficar atento?

Responda em máximo 5 pontos, bem objetivo.
```

---

## 🎯 CATEGORIA 3: DECISÃO DE COMPRA/VENDA

### Prompt 3.1: Devo Comprar Este FII?

**Situação**: Você encontrou um FII e quer decidir se compra agora.

**Prompt**:
```
Devo comprar o FII [TICKER] agora?

Contexto:
- Minha carteira tem [DESCREVER: ex: 40% logística, 30% varejo]
- Meu patrimônio em FIIs é R$ [VALOR]
- Sou um investidor [PERFIL: conservador/moderado/agressivo]
- Meu objetivo é [OBJETIVO: renda/crescimento/ambos]
- Tenho R$ [VALOR] disponível para investimento

Considerações:
- Este FII seria qual % da minha carteira?
- Qual segmento ele representa?
- Preciso desse segmento para diversificação?
- O preço está atrativo agora (comparar DY com histórico)?

Recomendação: Comprar, esperar, ou é melhor outra opção?
```

---

### Prompt 3.2: Devo Vender Este FII?

**Situação**: Seu FII caiu de preço e você está em dúvida.

**Prompt**:
```
Devo vender minha posição no FII [TICKER]?

Situação:
- Comprei a R$ [PREÇO]
- Agora está R$ [PREÇO]
- Ganho/perda: [CALCULAR]
- Motivo da queda: [DESCREVER o que você sabe]

Análise:
1. Por que caiu? (Mercado todo ou problema específico deste FII?)
2. Os fundamentos mudaram? (Taxa ocupação, dividendos?)
3. Isso é queda cíclica ou deterioração real?
4. Se esperar 12 meses, qual é minha expectativa?
5. Se vender agora, para que investir esse dinheiro?

Recomendação: Vender, manter, ou até comprar mais?
```

---

## 🔍 CATEGORIA 4: ANÁLISE FUNDAMENTALISTA

### Prompt 4.1: Leitura de Resultado Trimestral

**Situação**: FII divulgou resultado e você quer entender.

**Prompt**:
```
Ajude-me a entender o resultado trimestral do FII [TICKER] de [TRIMESTRE/ANO].

Destaque:
1. RECEITA: 
   - Total de receita
   - Comparar com trimestre anterior (cresceu/caiu?)
   - Há novos imóveis?

2. DIVIDENDO:
   - Valor distribuído neste trimestre
   - Comparar com trimestre anterior
   - FFO / Dividendo (é sustentável?)

3. OCUPAÇÃO:
   - Taxa de ocupação (acima de 90%?)
   - Mudanças recentes

4. PATRIMÔNIO:
   - Patrimônio total
   - Cresceu ou diminuiu?

5. IMPLICAÇÕES:
   - O que isso significa para o futuro?
   - Devo manter, aumentar ou vender?

```

---

### Prompt 4.2: Análise de Segmento

**Situação**: Você quer entender como está o segmento inteiro, não só um FII.

**Prompt**:
```
Analise o cenário atual do segmento de FIIs de [SEGMENTO].

Contexto econômico:
- Selic em [NÍVEL]
- Inflação em [NÍVEL]
- Economia: [Crescimento/estagnação/recessão]

Para o segmento [SEGMENTO]:
1. Como está performando? (Rentabilidade média)
2. Quais são os principais desafios?
3. Quais são as oportunidades?
4. Qual é minha expectativa para os próximos 12 meses?
5. Qual é o timing (melhor hora para comprar/vender)?

FIIs principais do segmento: [LISTAR alguns]
```

---

## 💡 CATEGORIA 5: ESTRATÉGIA E PLANEJAMENTO

### Prompt 5.1: Montar Carteira do Zero

**Situação**: Você está começando e quer montar uma carteira.

**Prompt**:
```
Ajude-me a montar uma carteira de FIIs do zero.

Meu perfil:
- Idade: [IDADE]
- Capital inicial: R$ [VALOR]
- Objetivo: [RENDA/CRESCIMENTO/AMBOS]
- Perfil de risco: [CONSERVADOR/MODERADO/AGRESSIVO]
- Horizonte de investimento: [1-2 anos / 5 anos / 10+ anos]
- Conhecimento: [INICIANTE/INTERMEDIÁRIO/AVANÇADO]

Quero que você:
1. Recomende alocação por segmento (em %)
2. Sugira 2-3 FIIs em cada segmento
3. Indique quanto investir em cada FII
4. Explique o racional da alocação
5. Como acompanhar/rebalancear anualmente
```

---

### Prompt 5.2: Estratégia de Longo Prazo (Viver de Dividendos)

**Situação**: Seu objetivo é eventualmente viver de dividendos de FIIs.

**Prompt**:
```
Quero construir uma carteira de FIIs que me pague dividendos 
suficientes para [OBJETIVO: complementar renda/viver disso tudo].

Minha realidade:
- Tenho hoje R$ [PATRIMÔNIO] em FIIs
- Quero receber R$ [VALOR] mensais
- Tenho [TEMPO] anos até aposentar
- Posso aportar R$ [VALOR] por mês

Plano:
1. Qual é meu alvo de patrimônio? (para atingir R$ [VALOR]/mês com DY de 6%)
2. Quanto tempo levará?
3. Qual deve ser minha estratégia: apenas FIIs ou combinar com outras aplicações?
4. Qual segmento priorizar para maior estabilidade de dividendos?
5. Ao atingir o alvo, como rebalancear para evitar perder patrimônio?
```

---

## ⚠️ CATEGORIA 6: TROUBLESHOOTING E PROBLEMAS

### Prompt 6.1: FII com Problema

**Situação**: Seu FII está apresentando sinais estranhos.

**Prompt**:
```
Tenho preocupação com o FII [TICKER] porque:

Sinais estranhos:
- [DESCREVER: ex: dividendo caiu 20%, preço muito baixo]
- [DESCREVER]
- [DESCREVER]

Quero entender:
1. Isso é normal ou problema real?
2. Por que isso está acontecendo?
3. Quais são as implicações futuras?
4. Devo vender ou esperar?
5. Qual é seu diagnóstico?
```

---

### Prompt 6.2: Contexto de Mercado Desfavorável

**Situação**: Mercado caiu, juros subiram e você está assustado.

**Prompt**:
```
O mercado está [SITUAÇÃO: em queda/volatilidade alta] e juros subiram 
para [NÍVEL]. Qual é o impacto para minha carteira de FIIs?

Minha carteira:
- [SEGMENTO 1]: [%]
- [SEGMENTO 2]: [%]
- [SEGMENTO 3]: [%]

Análise:
1. Qual é o impacto esperado em cada segmento?
2. Deve esperar se recuperar ou vender agora?
3. É oportunidade para comprar mais?
4. Qual deve ser minha estratégia?
5. Histórico: já passou por isso? O que aconteceu?
```

---

## 📊 CATEGORIA 7: COMPARAÇÃO E BENCHMARKING

### Prompt 7.1: Minha Carteira vs Mercado

**Situação**: Você quer saber como sua carteira está comparada à média.

**Prompt**:
```
Comparar minha carteira de FIIs com a média do mercado.

Minha carteira:
- [LISTAR FIIs com quantidade de cotas]

Análise:
1. DY média da minha carteira vs DY média do IFIX
2. Exposição por segmento: estou bem diversificado?
3. Tamanho dos FIIs: estou em fundos pequenos/médios/grandes?
4. Concentração: estou muito concentrado?
5. Performance: como estou rendendo vs a média?

Conclusão: Minha carteira é bom construída ou precisa de ajustes?
```

---

### Prompt 7.2: Análise de Performance Histórica

**Situação**: Você quer entender como seu FII performou no passado.

**Prompt**:
```
Análise histórica do FII [TICKER]:

Períodos:
1. Últimos 12 meses
2. Últimos 2 anos
3. Últimos 5 anos (se disponível)

Para cada período, quero:
- Rentabilidade total
- Rentabilidade por dividendos
- Rentabilidade por valorização
- Volatilidade
- Como comparou com a média do segmento?

Padrões: Há algo padrão em sua performance?
```

---

## 🎓 CATEGORIA 8: APRENDIZADO E DESENVOLVIMENTO

### Prompt 8.1: Revisar Conceitos

**Situação**: Você quer consolidar um conceito que não entendeu bem.

**Prompt**:
```
Explique-me [CONCEITO: ex: P/VPA, FFO, Cap Rate] de forma simples.

Estrutura:
1. Definição em 1 frase
2. Fórmula (se houver)
3. Como interpretar: o que significa um valor alto vs baixo?
4. Exemplo prático com números
5. Por que isso importa para investidor?
6. Comparar com conceito similar: [CONCEITO B]
7. 1-2 erros comuns ao interpretar
```

---

### Prompt 8.2: Aprender Sobre Segmento

**Situação**: Você quer entender profundamente um segmento.

**Prompt**:
```
Faça um mini-curso sobre FIIs de [SEGMENTO].

Módulo 1: FUNDAÇÃO
- O que caracteriza este segmento?
- Dinâmica de receita
- Riscos específicos

Módulo 2: ANÁLISE
- Principais métricas para avaliar
- Valores de referência (DY bom/ruim, P/VPA, etc)
- Como comparar dois FIIs deste segmento

Módulo 3: OPORTUNIDADES
- Qual é o melhor momento para investir?
- Expectativas para 5 anos
- Qual é meu alvo de alocação?

Módulo 4: PRÁTICA
- 3 FIIs principais deste segmento
- Qual você compraria agora? Por quê?
```

---

## 🚀 CATEGORIA 9: CASOS DE USO ESPECIAIS

### Prompt 9.1: FIIs para Aposentadoria

**Situação**: Você quer usar FIIs como parte do plano de aposentadoria.

**Prompt**:
```
Quero usar FIIs para complementar minha aposentadoria.

Situação:
- Tempo até aposentar: [TEMPO]
- Patrimônio atual em FIIs: R$ [VALOR]
- Capacidade de aporte mensal: R$ [VALOR]
- Renda mensal desejada em aposentadoria: R$ [VALOR]

Plano:
1. Qual é meu alvo de patrimônio? (para gerar renda passiva)
2. Taxa de retorno realista: DY + valorização
3. Qual deve ser meu mix de FIIs para segurança?
4. Quanto precisaré aportar por mês?
5. Como estruturar para minimizar riscos?

Roadmap: Ano por ano, qual deve ser minha estratégia?
```

---

### Prompt 9.2: FIIs como Hedging

**Situação**: Você quer usar FIIs para proteger patrimônio contra inflação.

**Prompt**:
```
Quero usar FIIs como proteção contra inflação.

Meu portfólio:
- [Descrever: rendimento fixo, ações, dólar, imóvel etc]

Análise:
1. Qual é meu risco de inflação atual?
2. FIIs são boa proteção contra inflação? Por quê?
3. Quanto alocar em FIIs para proteção adequada?
4. Qual tipo de FII (segmento) é melhor para hedging?
5. Comparar com outras proteções (ouro, dólar, imóvel direto)

Recomendação: Qual é meu alvo de alocação em FIIs?
```

---

## 📝 CATEGORIA 10: DOCUMENTAÇÃO E REGISTRO

### Prompt 10.1: Resumo da Carteira para Meus Registros

**Situação**: Você quer documentar sua carteira para referência futura.

**Prompt**:
```
Crie um resumo documentado da minha carteira de FIIs em [DATA].

Informações:
- [LISTAR TODOS OS FIIs COM: Ticker, Quantidade, Preço de compra, Data, DY atual]

Resumo Consolidado:
1. Total investido: R$ [VALOR]
2. Valor atual: R$ [VALOR]
3. Gain/Loss: R$ [VALOR] ([%])
4. Dividendos recebidos até agora: R$ [VALOR]
5. DY médio da carteira: [%]
6. Distribuição por segmento: [%]

Projeção:
- Dividendos esperados no próximo ano: R$ [VALOR]
- Patrimônio esperado em 5 anos (com aportes): R$ [VALOR]

Meta:
- Objetivo de patrimônio: R$ [VALOR]
- Prazo: [ANO]
- Ano de revisão próxima: [DATA]
```

---

## 💎 Prompt Bonus: O Melhor Prompt

Se você só tiver tempo para 1 pergunta, use este:

```
Você é um consultor especializado em FIIs. 
Analise os FIIs [TICKER 1], [TICKER 2] e [TICKER 3].

Para cada um, estruture assim:
1. Resumo: Segmento, tamanho, gestor
2. Atratividade atual: DY vs histórico, P/VPA
3. Risco: Principais vulnerabilidades
4. Score: 0-10, sendo:
   - 0-3 = Evitar
   - 4-6 = Manter (se tem)
   - 7-8 = Comprar
   - 9-10 = Compra urgente

Tabela final comparativa dos 3.

Recomendação: Qual comprar agora com R$ [VALOR]?
```

---

## 📌 Dicas para Melhorar Seus Prompts

1. **Seja específico**: Sempre inclua datas, valores, nomes
2. **Contextualize**: Explique seu perfil e objetivo
3. **Estruture**: Peça resposta em formato específico (tabela, lista, etc)
4. **Itere**: Se resposta não satisfez, refine a pergunta
5. **Guarde**: Prompts que funcionaram bem, reutilize

---

## Index Rápido por Situação

| Situação | Prompt | Página |
|----------|--------|--------|
| Tenho um FII e quero analisar | 1.1 | Categoria 1 |
| Estou entre 2 FIIs | 1.2 | Categoria 1 |
| FII com DY muito alto | 1.3 | Categoria 1 |
| Revisar carteira | 2.1 | Categoria 2 |
| Acompanhamento rápido | 2.2 | Categoria 2 |
| Devo comprar? | 3.1 | Categoria 3 |
| Devo vender? | 3.2 | Categoria 3 |
| Entender resultado | 4.1 | Categoria 4 |
| Como está o segmento? | 4.2 | Categoria 4 |
| Montar carteira do zero | 5.1 | Categoria 5 |
| Planejar aposentadoria | 5.2 | Categoria 5 |
| FII com problema | 6.1 | Categoria 6 |
| Mercado em crise | 6.2 | Categoria 6 |
| Comparar com mercado | 7.1 | Categoria 7 |
| Análise histórica | 7.2 | Categoria 7 |
| Entender conceito | 8.1 | Categoria 8 |
| Aprender segmento | 8.2 | Categoria 8 |

---

**Última atualização**: Abril de 2026

**Estes prompts foram testados em múltiplas iterações e refinados 
para máxima efetividade. Use como templates, adapte conforme necessário.**

