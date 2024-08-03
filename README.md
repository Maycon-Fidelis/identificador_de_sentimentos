# Detector de sentimentos

Este é um projeto capaaz de detectar qual o sentimento presente em um texto, sendo possível retornar felicidade, raiva e tristeza, caso a probabilidade de acerto for baixa ele retorna 'Emoção desconhecida'.

## Estrutura do Projeto

- `data/sentimentos.csv`: Arquivo que contem os dados usado para treinar o modelo, tendo frases com as emoções de felicidade, raiva e tristeza.
- `sentimentos.ipynb`:  Arquivo Jupyter Notebook que contém os dados, treino do modelo e a execução do modelo.

## Requisitos

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook


## Instruções para Execução

1. Clone este repositório:

    ```bash
    git clone https://github.com/Maycon-Fidelis/identificador_de_sentimentos.git
    cd identificador_de_sentimentos
    ```

2. Instale as dependências (se ainda não estiverem instaladas):

    ```bash
    pip install pandas numpy scikit-learn jupyterlab
    ```
    
3. Dentro da pasta `identificador_de_sentimentos`, digite o comando para abrir o Jupyter Notebook no navegador:
   ```
   jupyter notebook
   ```

4. No Jupyter, abra o arquivo `sentimentos.ipynb`.

## Uso

Execute os comandos pela ordem em que aparecem no notebook. Após treinar o modelo, você pode usar a função `detectar_emocao` para identificar a emoção de uma frase. Exemplo:

```python
print(detectar_emocao('Sinto sua falta')) # Retorna: tristeza
