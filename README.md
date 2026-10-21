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
@misc{CropRowsDataset2019,
  author = {Pereira Junior, P.C. and von Wangenheim, A.},
  title = {Orthomosaic Dataset of RGB aerial Images for Crop Rows Detection},
  year = {2019},
  publisher = {LAPIX/UFSC},
  journal = {INCoD Datasets Repository},
  howpublished = {\url{http://www.lapix.ufsc.br/weed-mapping-sugar-cane}}
}
```

```bibtex
@misc{WeedMappingDataset2019,
  author = {Monteiro, A.A.O. and von Wangenheim, A.},
  title = {Orthomosaic Dataset of RGB aerial Images for Weed Mapping},
  year = {2019},
  publisher = {LAPIX/UFSC},
  journal = {INCoD Datasets Repository},
  howpublished = {\url{http://www.lapix.ufsc.br/weed-mapping-sugar-cane}}
}
```