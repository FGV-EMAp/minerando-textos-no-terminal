# Minerando Textos no Terminal
Usando  sed e outras ferramentas do terminal para minerar textos.

## Descrição do exercício.
Seu objetivo é resolver todas as tarefas usando apenas recursos do terminal, Bash no Linux e Gitbash no Windows. 

Coloque cada solução em um script shell separado, usando o seguinte padrão para nomear os arquivos: `ex_1.sh`.

Cada um destes scipts, quando executado, deve escrever a resposta em um arquivo chamado `resposta_ex_1`, `resposta_ex_2`, e assim por diante. 

### Exercícios
Na pasta Dados está a obra completa de Machado de Assis na forma de vários arquivos de texto, distribuídos em vários sub-diretórios.

1. Quantas palavras tem a obra completa?
2. Liste os títulos das obras, em ordem alfabética.
3. Liste os contos (seus títulos), em ordem cronológica de publicação. o resultado deve ser algo como:

```
Contos Fluminenses, 1870
Historias da Meia-Noite, 1873
...
```
4. Escolha uma obra, e liste as palavras distintas que aparecem nela, em ordem alfabética, seguidas do número de ocorrências de cada uma. O resultado deve ser algo como:

```
6 romance,
6 rompeu
6 rosto.
...
```
dica: Para facilitar comece colocando cada palavra em uma linha separada:
```bash
$ echo "gato sapato" | sed 's/ /\n/g'
```
