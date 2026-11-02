# Protocolo de anotação: feijão em estágio inicial, versão v3

Base: as 8 imagens com `para_anotar = 1` em `imagens/drybean-estagio-inicial/selecao.csv`.
Ferramenta: `ferramentas/anotar_feijao.py` (sem argumentos). As imagens originais não são alteradas.

Medidas de referência (~1,5 cm/pixel): cada parcela tem 3 linhas de plantio espaçadas
~20 px (~30 cm), com ~60 a 70 px (~1 m) de comprimento; plantas com ~6 a 8 px.

## 1. Região (ciano, tecla r)
- Um retângulo de ~400 x 300 px (8 a 12 parcelas), marcado com dois cliques em cantos opostos.
- Área com parcelas bem visíveis e algumas falhas; evitar bordas da imagem e manchas muito escuras.
- Se possível, bordas do retângulo sobre as ruas, sem cortar parcelas.
- Só o que está dentro da região é anotado e avaliado.

## 2. Linhas (amarelo, tecla l)
- Cada uma das 3 linhas de cada parcela dentro da região: um segmento do centro da primeira
  planta ao centro da última, seguindo o eixo da linha.
- A linha nunca é dividida, mesmo com falhas.
- Linha inteiramente sem plantas: anotar na posição esperada (alinhada às vizinhas, ~20 px),
  com o comprimento das outras duas linhas da parcela.
- Se faltam plantas na ponta, a linha vai até a altura das pontas das vizinhas.
- Parcela cortada pela borda da região: anotar só a parte dentro dela.

## 3. Falhas (vermelho, tecla f)
- Trecho da linha sem plantas com pelo menos ~10 px (~15 cm), maior que o espaço normal
  entre plantas vizinhas. Clicar onde a planta acaba e onde recomeça.
- Linha inteira vazia: uma falha do começo ao fim dela.

## Não anotar
Plantas soltas fora das linhas (daninhas), manchas escuras de solo e o espaço entre parcelas.

## Saída
- `anotacoes-feijao-inicial/<id>.json`: "regiao" [x0, y0, x1, y1], "linhas" e "falhas"
  [x1, y1, x2, y2], em pixels da imagem RGB original.
- `imagens/drybean-estagio-inicial/anotadas/<id>.png`: cópia com as anotações desenhadas.
