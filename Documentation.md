`docker pull pandoc/latex`
`docker run --rm --volume "`pwd`:/data" --user `id -u`:`id -g` pandoc/latex <file-name>.md -o <file-name>.pdf`
