# Docker image for git

[Git](https://git-scm.com/) is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

## Supported tags and respective `Dockerfile` links

- [`latest` (*Dockerfile*)](https://github.com/eea/eea.docker.git-scm/blob/master/Dockerfile)

## Usage

```console
$ docker run --rm -v /path/to/code:/code eeacms/git clone https://github.com/eea/eea.docker.git-scm.git .
```

## Advanced usage

Add:

```console
$ docker run --rm -v /path/to/code:/code -w /code eeacms/git add . 
```

Commit:

```console
$ docker run --rm -v /path/to/code:/code -w /code eeacms/git commit -m "Hello" 
```

Push:

```console
$ docker run --rm -v /path/to/code:/code -w /code eeacms/git push -u origin master 
```

See git `--help` for more options:

```console
$ docker run --rm eeacms/git --help
```
