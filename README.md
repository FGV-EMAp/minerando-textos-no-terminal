# Minerando Textos no Terminal
Usando  sed e outras ferramentas do terminal para minerar textos.

## Descrição do exercício.
Seu objetivo é resolver todas as tarefas usando apenas recursos do terminal, Bash no Linux e GitBash no Windows. 

Coloque cada solução em um **script shell separado**, usando o seguinte padrão para nomear os arquivos: `ex_1.sh`.

Cada um destes scipts, quando executado, deve escrever a resposta em um arquivo chamado `resposta_ex_1`, `resposta_ex_2`, e assim por diante. 

### Exercícios
Na pasta *Dados* está a obra completa de Machado de Assis na forma de vários arquivos de texto, distribuídos em vários sub-diretórios.

1. Quantas palavras tem a obra completa?
2. Liste os títulos das obras, em ordem alfabética.
3. Liste os contos (seus títulos), em ordem cronológica de publicação. o resultado deve ser algo como:

```
Contos Fluminenses, 1870
Historias da Meia-Noite, 1873
...
```
4. Utilizando o conto `macn001.txt` , e liste as palavras distintas que aparecem nela, em ordem alfabética, seguidas do número de ocorrências de cada uma. O resultado deve ser algo como:

```
6 romance,
6 rompeu
6 rosto.
...
```
Dica 1: Para facilitar comece colocando cada palavra em uma linha separada:
```bash
$ echo "gato sapato" | sed 's/ /\n/g'
```
No código acima, a expressão regular `s/ /\n/g` substitui todos os espaços por quebras de linha.

Dica 2: use o comando `sort` e o `uniq`.

5. faça o mesmo que o exercício anterior, mas agora para todas as obras.
6. Usando o resultado do exercício anterior, liste as palavras que aparecem mais de 1000 vezes. 

Dica:  considere o seguinte componente para o seu pipeline: `grep -E "^ *[[:digit:]]{4}"`; [Dicas de grep](https://github.com/fccoelho/introcomp/blob/main/conte%C3%BAdo/Introdu%C3%A7%C3%A3o%20%C3%A0%20programa%C3%A7%C3%A3o/GREP.md).
   
## Entrega
Coloque os scrits com as suas soluções e os arquivos de resposta no diretório `Solução` deste repositório. ao final, não esqueça de fazer um commit e um push.
