# Central de Materiais

Site estático simples: uma página inicial (`index.html`) lista materiais
gratuitos, cada um atrás de um formulário de nome/e-mail/whatsapp (modal de
captação). Ao enviar, o lead vai pro webhook (Gridlabs/n8n) e o material abre
numa nova aba.

## Estrutura

- `index.html` — central de materiais (hub)
- `pastor-uai.html` — primeiro material: raio-x do caso "Pastor da UAI" (Edney Ulisses)
- `assets/` — imagens usadas nas páginas

## Paleta atual (provisória)

Creme (`#FAF8F4`) + azul (`#1D9BF0`). Ainda não é identidade visual final —
"depois definimos certinho".

## Adicionar um novo material

1. Criar a página do material (HTML autocontido, mesma paleta).
2. Adicionar um card em `index.html` dentro de `.grid`, com
   `onclick="abrirGate('Tipo','Título','arquivo.html')"`.
