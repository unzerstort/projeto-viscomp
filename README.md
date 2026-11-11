# Projeto de Visualização Computacional

Projeto para a disciplina de Visualização Computacional.

## Estrutura

- `scrapy.cfg`: configuração do Scrapy
- `scraper/`: pacote principal do scraper
  - `scraper/disciplinas/`: código do scraper
  - `scraper/disciplinas/spiders/`: spiders
  - `scraper/disciplinas/config/`: URLs e constantes
- `data/`: arquivos brutos gerados pelo scraper
- `notebooks/`: notebooks de análise e exploração

## Instalação

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Execução

```bash
cd scraper
scrapy list
scrapy crawl janus_disciplinas -o ../data/disciplinas.json
```
