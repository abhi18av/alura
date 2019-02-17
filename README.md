# alura_dl

This is inspired from `edx-dl` and downloads the courses from `alura.com.br`

## Development Setup


```
brew install pipenv 
pipenv lock
git flow init

pipenv install # uses the already generated Pipfile.lock
```


## ToDos

- Find a way to download stuff using `youtube-dl` from `vimeo` videos
```
youtube-dl https://player.vimeo.com/play/807833333 --referer https://cursos.alura.com.br/course/shellscripting/task/28942

```

- This works 

```
youtube-dl https://vimeo.com/309964196 --ignore-config
```