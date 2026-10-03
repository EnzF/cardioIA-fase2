# CardioIA — Parte 1

## Arquivos

- `carregador_base.py`: abre os CSVs e o arquivo de relatos.
- `extrator_sintomas.py`: normaliza o texto e detecta conceitos/atributos.
- `analisador_clinico.py`: consulta as associações da knowledge base.
- `main.py`: executa o pipeline e mostra o resultado.

## Como executar

Os arquivos devem estar dentro de `CardioAI/src/`, ao lado das pastas já existentes
`data/` e `knowledge_base/`.

No terminal, a partir da raiz `CardioAI`:

```bash
python src/main.py
```

Também funciona com o terminal aberto dentro de `src`:

```bash
python main.py
```

## Observação

A pontuação exibida serve apenas para ordenar e explicar quantas evidências
cadastradas foram encontradas. Ela não é probabilidade nem diagnóstico médico.
