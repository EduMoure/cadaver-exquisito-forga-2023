# Instruccións

__😱 Non modifiques este arquivo 😱__

Le atentamente este documento.
## Preparando a contorna
Clona o repositorio no teu ordenador.
```sh
git clone https://github.com/Diseno-de-Aplicaciones-Web/cadaver-exquisito-forga-2023.git
```
Le atentamente o arquivo en [`./src/README.md`](./src/README.md).

Busca a parte do documemto que te tocou completar. Decide qué vai suceder nesa pasaxe da historia.

Cambiate á rama `develop`.
```sh
git switch develop
```
Crea unha rama de traballo. Emprega o nome da pasaxe que che tocou completar. Por exemplo, se tes que facer a pasaxe `Mr McGregor chega a casa`:
```sh
git switch -c feature/mr-mcgregor-chega-a-casa
```
## Engadindo os contidos
Escribe o texto da túa sección. Vai creando commits según fagas avances e correccións. Intenta crear polo menos tres ou catro commits.
```sh
git add ./src/README.md
git commit -m "Enlaza coa pasaxe anterior"
...
git add ./src/README.md
git commit -m "Acontece algo inesperado"
...
git add ./src/README.md
git commit -m "Enlaza coa pasaxe seguinte"
```
## Preparando o envío dos contidos
Unha vez estés satisfeita co resultado, trae á túa rama os contidos das túas compañeiras para detectar posibles conflictos e mirar de solucionalos.
```sh
git switch develop
git pull
git switch - # Este é un atallo para regresar á rama anterior
git merge develop
```
Outro xeito de facer a maniobra anterior sería:
```sh
git pull origin develop
```
É posible que neste momento Git te indique que existen conflictos entre os contidos que aportas e os aportados por alguén máis. __Tómate o tempo necesario para solucionalo__. Se é necesario busca axuda e pide a cooperación da persoa autora dos contidos cos que se producen conflictos. 🤝

Se tiveches que dedicar un tempo a solucionar conflictos é posible que se engadisen novos contidos en `develop` en ese tempo. Trae novamente á túa rama os contidos de `develop` para asegurarte de que seguen sen existir conflictos.

## Entrega os teus contidos
Fusiona os teus contidos na rama `develop`.
```sh
git switch develop
git merge feature/aqui-vai-o-nome-da-tua-rama
```
Non deberían de terse producido conflictos, pero se así fose, será necesario solucionalos para poder seguir adiante.

Envía as entregas cos teus cambios ó repositorio remoto.
```sh
git push
```

## Limpa a casa
Xa non necesitamos máis a rama de traballo. Imos borrala.
```sh
git branch -d feature/aqui-vai-o-nome-da-tua-rama
```
## Segue a evolución da narración

Podes regresar ó proxecto de cando en vez e revisar os cambios chegados ó documento para ver cómo remata a historia de McGregor.
```sh
git switch develop # Non é necesario se xa estás na rama develop
git pull
```

__💕 Se ves erros neste arquivo, podes abrir unha rama de traballo para correxilo e fusionar os teus cambios en `develop` 💕__