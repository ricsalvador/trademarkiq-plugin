# TrademarkIQ Plugin

Plugin do [TrademarkIQ](https://trademarkiq.com.br): inteligência de marcas sobre a base completa do INPI, atualizada a cada Revista da Propriedade Industrial (RPI), disponível para assistentes de IA via MCP.

## Servidor MCP

- URL: `https://mcp.trademarkiq.com.br`
- Transporte: streamable HTTP
- Autenticação: OAuth (conta TrademarkIQ); o registro dinâmico de clientes é aceito
- 31 ferramentas, todas de leitura

## Instalação

Adicione o servidor ao seu cliente MCP:

```json
{
  "mcpServers": {
    "trademarkiq": {
      "type": "streamable-http",
      "url": "https://mcp.trademarkiq.com.br"
    }
  }
}
```

O mesmo conteúdo está em [`mcp.json`](mcp.json); o manifesto do plugin está em [`plugin.json`](plugin.json).

## O que dá para perguntar

- "O nome Aurora Café já está registrado no INPI para cafeteria?"
- "Quais classes de Nice preciso para abrir uma loja online de cosméticos naturais?"
- "Qual o risco de colidência da marca Vertice na classe 35?"

## Ferramentas

- Busca e registro: `buscar_marcas`, `detalhes_marca`, `obter_logo`, `classificar_atividade`, `classes_de_nice`
- Risco e viabilidade: `analisar_colidencia`, `diagnostico_viabilidade`
- Marcas fora do Brasil: `analise_internacional`, `mercado_por_pais`, `atualizacao_por_pais`, `origem_depositos_brasil`, `ranking_procuradores`, `relacoes_internacionais`
- Mercado e índice TIQ: `consultar_indice_tiq`, `valores_de_dimensao`, `ranking_tiq`, `relatorio_de_mercado`
- RPI: `rpi_edicoes`, `rpi_resumo`, `rpi_despachos`
- Processos judiciais e jurisprudência: `buscar_processos_pi`, `processo_pi`, `estatisticas_juris`, `jurisprudencia_pi`
- Carteira da conta conectada: `meu_portfolio`, `resumo_portfolio`, `eventos_portfolio`, `criticos_portfolio`, `vencimentos_portfolio`, `colidencias_ultima_rpi`, `contencioso_portfolio`

## Aviso

As análises são de risco, com base em dados públicos do INPI, e não constituem parecer jurídico nem garantia de registro ou de indeferimento.

## Links

- Site: https://trademarkiq.com.br
- Suporte: https://trademarkiq.com.br/contato
- Privacidade: https://trademarkiq.com.br/politica-de-privacidade
- Termos de uso: https://trademarkiq.com.br/termos-de-uso
