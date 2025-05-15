# Testes de Detecção de Pontos com Gemini

Este notebook explora o uso da API do Gemini (Google Generative AI) para realizar a detecção de anomalias em séries temporais sintéticas.

## Objetivo

- Gerar uma série temporal fictícia com ruído e um pico propositado.
- Enviar essa série para o modelo Gemini, solicitando que detecte:
  - **Gaps (ausência de valores)** prolongados.
  - **Mudanças abruptas (picos)**.
- Visualizar os pontos identificados como anômalos.
- Classificar cada ponto da série em categorias como:
  - Ausência de vendas;
  - Pico;
  - Normal.

## Tecnologias e Bibliotecas

- Python 3
- [NumPy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [Matplotlib](https://matplotlib.org/)
- [Google Generative AI (Gemini)](https://ai.google.dev/)

## Como Executar

1. Configure sua chave da API Gemini no notebook:

```python
genai.configure(api_key="SUA_CHAVE")
```

2. Execute o notebook célula por célula para:

   * Criar a série temporal
   * Fazer chamadas ao modelo Gemini
   * Visualizar os resultados

## Exemplo de Saída

* Série com ruído e pico visualizada.
* Índices de anomalias identificados automaticamente.
* Classificação textual dos dias (ex: "pico", "ausência de vendas", etc.).

## ⚠️ Observações

* É necessário possuir uma chave de API válida do Google Generative AI para utilizar o modelo Gemini.
* O modelo pode retornar variações nos resultados conforme atualizações da API ou alterações no prompt.

## Autor

Felipe Lapa do Nascimento
