# Base de Conhecimento

## Dados Utilizados

Descreva se usou os arquivos da pasta `data`, por exemplo:

| Arquivo | Formato | Utilização no Agente |
|---------|---------|---------------------|
| `historico_atendimento.csv` | CSV | Contextualizar interações anteriores, e resumir a última interação se houver relação com a nova interação |
| `perfil_consumidor.json` | JSON | Analisar e contribuir com melhoria no desenvolvimento financeiro do usuário |
| `transacoes.csv` | CSV | Analisar padrão de gastos do cliente |

> [!TIP]
> **Quer um dataset mais robusto?** Você pode utilizar datasets públicos do [Hugging Face](https://huggingface.co/datasets) relacionados a finanças, desde que sejam adequados ao contexto do desafio.

---

## Adaptações nos Dados

> Você modificou ou expandiu os dados mockados? Descreva aqui.

- O nome do arquivo '/data/perfil_investidor.json' mudaram para '/data/perfil_consumidor', e os seus dados também foram alterados para serem utilizados no desenvolvimento do agente com a função de alertar sobre consumos excessivos.
- Os dados do arquivo '/data/historico_atendimento' foram alterados para acompanhar o treinamento do agente com a função de alertar e auxiliar no desenvolvimento financeiro saúdavel do usuário.
- Arquivo '/data/produtos_financeiros' foi excluído, não necessário para o agente que será desenvolvido.

---

## Estratégia de Integração

### Como os dados são carregados?
> Descreva como seu agente acessa a base de conhecimento.

Os JSON/CSV são carregados no início da sessão e incluídos no contexto do prompt

### Como os dados são usados no prompt?
> Os dados vão no system prompt? São consultados dinamicamente?

[Sua descrição aqui]

---

## Exemplo de Contexto Montado

> Mostre um exemplo de como os dados são formatados para o agente.

```
Dados do Cliente:
- Nome: João Silva
- Perfil: Moderado
- Saldo disponível: R$ 5.000

Últimas transações:
- 01/11: Supermercado - R$ 450
- 03/11: Streaming - R$ 55
...
```
