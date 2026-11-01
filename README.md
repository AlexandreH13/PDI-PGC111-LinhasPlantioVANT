# PDI-PGC111-LinhasPlantioVANT

## Detecção de Linhas de Plantio em Imagens de VANT

**Descrição**

Este repositório apresenta a aplicação de métodos de processamento digital de imagens para identificação de linhas de plantio em imagens de VANT (drones). Tem como objetivo avaliar diferentes métodos, comparar os resultados e realizar uma análise crítica sobre os mesmos.

**Etapas**

- Índice de vegetação por cor (ExG);
- Segmentação vegetação x solo (O que é vegetação o que é solo)
- Orientação dominante, espaçamento e falhas (projeção ou Hough)

**Comparações**

- Índice de cor distintos (ExG, ExGR, canal a* do L* a* b*); projeções x transformada de Hough

**Métricas**

Erro de espaçamento e de orientação; precisão e revocação das falhas detectadas.

**Referências**

```bibtex
@inproceedings{aslahishahri2021rgb,
  title={From RGB to NIR: Predicting of near infrared reflectance from visible spectrum aerial images of crops},
  author={Aslahishahri, Masoomeh and Stanley, Kevin G and Duddu, Hema and Shirtliffe, Steve and Vail, Sally and Bett, Kirstin and Pozniak, Curtis and Stavness, Ian},
  booktitle={Proceedings of the IEEE/CVF international conference on computer vision},
  pages={1312--1322},
  year={2021}
}
```