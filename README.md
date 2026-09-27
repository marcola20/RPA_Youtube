# RPA_Youtube

Sobe os vídeos gravados do PES para o YouTube Studio, já programados como
estreia, com título, descrição, miniatura e playlist da competição.

## Instalação

```
pip install playwright
```

(Usa o Google Chrome instalado no PC, não precisa de `playwright install`.)

## Primeira vez

1. Rode `python login.py`. Na primeira execução ele cria o `caminhos.ini` e
   para. Abra esse arquivo e ajuste:
   - `pasta_videos`: onde a NVIDIA salva as gravações do PES (a mesma do
     Auto_PES21).
   - `chrome`: em branco para achar sozinho.
2. Rode `python login.py` de novo, entre na conta Google do canal, confira o
   YouTube Studio e feche o Chrome. O login fica salvo em `perfil_chrome/`
   (que **nunca** vai para o GitHub).

## Uso

```
python upar_videos.py
```

Edição, temporada, playlists e intervalo entre estreias ficam em `config.py`.
Descrições e capas são os arquivos `descricao_*.txt` e `capa_*.jpg`.
