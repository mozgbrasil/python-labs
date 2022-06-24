[checkmark]: https://raw.githubusercontent.com/mozgbrasil/mozgbrasil.github.io/master/assets/images/logos/logo_32_32.png "MOZG"

![valid XHTML][checkmark]

# python-labs 👉️

https://docs.python.org/

## Contribuição

Caso queira contribuir para melhoria da documentação de um Fork no repositório e envie um pull request ou edite no github

## Requerimentos

- https://www.docker.com/
- https://code.visualstudio.com/
- https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack

## Executando local

```bash
git clone ☝️

cd <directory>

code --new-window .
```

## Executando no container

## pytube

````bash
cd /workspaces/python-labs/src/pytube/

python -V

python helloworld.py

python3 "helloworld.py"

#pip install -r requirements.txt

pytube --version

echo -e '' '\n'

cd /workspaces/python-labs/src/pytube/0-input

# pytube

- https://github.com/pytube/pytube

PATH_FILE="/workspaces/python-labs/src/pytube/playlists.txt"
while IFS= read -r line; do
  if [[ ! "$line" || "$line" == '#'* ]]; then continue ; fi
  echo -e 'pytube' $line '\n'
done < $PATH_FILE

# mp4tomp3.py

- https://github.com/andyp123/mp4_to_mp3

```bash
🛑️ https://brew.sh/

brew install mplayer
brew install lame
````

```bash
clear && find \
  /workspaces/python-labs/src/pytube/0-input/* \
  -type d | while read ITEM; do
  # echo -e "\e[38;2;255;0;0m $ITEM \e[0m"
  BASENAME_ITEM="$(basename "${ITEM}")"
  # echo "👉️ BASENAME_ITEM: ${BASENAME_ITEM}"
  INPUT="${ITEM}"
  # echo "👉️ INPUT: ${INPUT})"
  OUTPUT="/workspaces/python-labs/src/pytube/1-ouput/${BASENAME_ITEM}"
  # echo "👉️ OUTPUT: ${OUTPUT})"
  mkdir -p "$OUTPUT"
  # echo "✅️👇️"
  echo -e 'python' '/workspaces/python-labs/src/pytube/mp4tomp3.py' \'"$INPUT"\' \'"$OUTPUT"\' '\n'
done
```

# "FAQ" Perguntas mais frequentes

## There was an error with video: <pytube.__main__.YouTube object: videoId=9iksInipOD8>
__init__: could not find match for ^\w+\W

https://exerror.com/pytube-exceptions-regexmatcherror-__init__-could-not-find-match-for-ww/

/opt/python/latest/lib/python3.10/site-packages/pytube/cipher.py

        # var_regex = re.compile(r"^\w+\W")
        var_regex = re.compile(r"^\$*\w+\W")

##