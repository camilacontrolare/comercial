# 6. Proposta e precificação

## Princípios

1. **Preço por complexidade, não por "achismo".** Use sempre a mesma tabela para que dois vendedores cheguem ao mesmo valor.
2. **Escopo explícito.** O que está incluso, o que é cobrado à parte, limites (nº de lançamentos, notas, funcionários).
3. **Três opções (pacotes).** Facilita a decisão e ancora o valor — o cliente escolhe *qual* plano, não *se* contrata.
4. **Reajuste anual previsto em contrato** (índice definido, ex.: IPCA ou INPC).
5. **Evitar aviltamento de honorários** — o Código de Ética do contador veda honorários incompatíveis com o trabalho.

## Modelo de precificação `[AJUSTAR valores]`

Honorário mensal = **Base por regime** + **adicionais de complexidade**

A tabela de referência está em [modelos/tabela-precificacao.csv](../modelos/tabela-precificacao.csv). Estrutura:

| Componente | Variável |
|------------|----------|
| Base por regime | MEI, Simples – Serviços, Simples – Comércio, Lucro Presumido, Lucro Real |
| Faixa de faturamento | Multiplicador por faixa |
| Folha de pagamento | Valor por funcionário + valor por pró-labore |
| Volume de documentos | Adicional por faixa de notas/lançamentos |
| Atividade com obrigações extras | ICMS/ST, filiais, importação, etc. |
| Serviços avulsos | Abertura, alteração contratual, IRPF dos sócios, certidões, parcelamentos |

### Como calcular o custo (para validar a tabela)

Pelo menos uma vez por ano, confira se a tabela cobre o custo real:

```
Custo-hora do escritório = (custos fixos mensais + salários e encargos) ÷ horas produtivas da equipe no mês
Horas por cliente/mês     = estimativa da equipe (fiscal + contábil + DP + atendimento)
Preço mínimo              = horas por cliente × custo-hora × (1 + margem desejada)
```

Se o preço da tabela ficar abaixo do preço mínimo para um perfil de cliente, a tabela precisa ser revista.

## Pacotes sugeridos `[AJUSTAR]`

| | **Essencial** | **Gestão** (recomendado) | **Estratégico** |
|---|---|---|---|
| Contabilidade e obrigações fiscais | ✅ | ✅ | ✅ |
| Folha de pagamento e eSocial | ✅ | ✅ | ✅ |
| Atendimento | E-mail/WhatsApp em até 24h | WhatsApp em até 4h | Contador dedicado |
| Relatório gerencial mensal (DRE simplificada) | — | ✅ | ✅ |
| Reunião de resultados | — | Trimestral | Mensal |
| Planejamento tributário anual | — | ✅ | ✅ |
| IRPF dos sócios | Cobrado à parte | 1 sócio incluso | Todos os sócios |
| BPO financeiro (contas a pagar/receber) | — | — | ✅ |
| **Honorário mensal** | R$ [X] | R$ [X × 1,4] | R$ [X × 2,2] |

## Estrutura da proposta

Modelo completo em [modelos/proposta-comercial.md](../modelos/proposta-comercial.md):

1. Capa personalizada (nome e logo do cliente)
2. **O que entendemos da sua empresa** (resumo do diagnóstico, com as palavras do cliente)
3. Objetivos que vamos atingir juntos
4. Escopo dos serviços e pacotes
5. Investimento e condições
6. Como funciona a transição (onboarding em 30 dias)
7. Por que nós (diferenciais + depoimentos)
8. Próximos passos e validade da proposta (ex.: 10 dias)

## Apresentação da proposta (20 min)

1. Recapitule as dores ("Você me disse que...") — 3 min
2. Mostre como cada dor é resolvida — 7 min
3. Apresente os pacotes, começando pelo **recomendado** — 5 min
4. Pergunte: **"Qual desses faz mais sentido para vocês?"** — e fique em silêncio — 5 min

## Política de descontos `[AJUSTAR]`

| Situação | Desconto máximo | Aprovação |
|----------|-----------------|-----------|
| Pagamento anual antecipado | 10% | Comercial |
| Indicação de cliente atual | 1º mês com 50% | Comercial |
| Cliente estratégico / grande conta | Até 15% | Sócio(a) |
| Qualquer outra | — | Sócio(a), com justificativa |

Prefira **ajustar o escopo** a dar desconto: "Para chegar nesse valor, podemos tirar X do pacote."
