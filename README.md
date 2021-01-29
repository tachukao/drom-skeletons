# drom skeletons

## Getting started

```sh
opam install drom
git clone https://github.com/tachukao/drom-skeletons.git ~/Library/Application\ Support/com.ocamlpro.drom/skeletons # on macOS
git clone https://github.com/tachukao/drom-skeletons.git ~/.config/drom/skeletons # on Linux
```

## Create a new paper

```sh
drom new [paper-name] --skeleton paper
```

## Create a new note

```sh
drom new [note-name] --skeleton paper
```

## Adding a new figure template and genearting the pdf inside a paper or note

```sh
cd [paper-name]
drom package [fig-name] --new=figure
cd figures
make [fig-name]
```
