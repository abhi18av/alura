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

- This works (separate video)

```
youtube-dl https://vimeo.com/309964196 --ignore-config
```

- This doesn't
```
youtube-dl https://vimeo.com/807833333 --referer https://cursos.alura.com.br
```

- Main video URL 

```
https://player.vimeo.com/play/807833333?s=229132790_1550455353_52faa799e25281c3a8cb20107a4d86f9&loc=external&context=Vimeo%5CController%5CApi%5CResources%5CVideoController.&download=1&filename=640-shell-video1.1-Introduc%25CC%25A7a%25CC%2583o164.mp4
```


- Clues 

```
alura.userId: 141337

Referer: https://cursos.alura.com.br/course/shellscripting/task/28942


```


wget --referer "https://cursos.alura.com.br/course/shellscripting/task/28942" "https://player.vimeo.com/video/807833333"


- This works
Video URL from the actual page - got it by it's page `html` rather than `inspect element`
https://player.vimeo.com/video/229132790


youtube-dl https://player.vimeo.com/video/229132790 --referer https://cursos.alura.com.br/course/shellscripting/task/28942



youtube-dl https://player.vimeo.com/video/229133282 --referer https://cursos.alura.com.br/course/shellscripting/task/28945 





