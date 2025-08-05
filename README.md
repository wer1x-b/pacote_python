# Pacote Python: meu_pacote

Este projeto demonstra como organizar funções em um pacote Python simples.

## Estrutura de Pastas

```
pacote_python/
├── meu_pacote/
│   ├── __init__.py
│   ├── codigo_principal.py
│   └── funcoes.py
```

## Arquivos

- **funcoes.py**: Contém funções utilitárias, como `n_par`.
- **codigo_principal.py**: Script principal que utiliza as funções do pacote.
- **__init__.py**: Torna a pasta `meu_pacote` um pacote Python.

## Como Executar

1. Abra o terminal e navegue até a pasta `pacote_python`:

   ```shell
   cd c:\Users\wer1x\Downloads\pacote_python
   ```

2. Execute o script principal como módulo do pacote:

   ```shell
   python -m meu_pacote.codigo_principal
   ```

   Isso irá imprimir `True` no terminal.

## Observações

- O import das funções no `codigo_principal.py` deve ser feito assim:

  ```python
  from funcoes import n_par
  ```

  Se quiser usar import relativo, altere para:

  ```python
  from .funcoes import n_par
  ```

  e execute como módulo do pacote.

- Certifique-se de que existe um arquivo `__init__.py` na pasta do pacote.

## Requisitos

- Python 3.13 ou superior (de acordo com seu ambiente)
- Recomenda-se usar um ambiente virtual (`venv`)

---

**Dúvidas?**  
Abra uma issue no repositório ou consulte a documentação do Python sobre pacotes e módulos.