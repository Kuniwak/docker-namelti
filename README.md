namelti on Docker
=================

Usage
-----

### Oneshot

```console
$ echo 太郎 | docker run -i --rm kuniwak/debian-namelti:latest
タロウ(1), フトシロウ(1), フトロウ(1), タイロウ(1),
```


### Interactive

```console
$ docker run -it --rm kuniwak/debian-namelti:latest
太郎
タロウ(1), フトシロウ(1), フトロウ(1), タイロウ(1),
花子
ハナコ(1), ハナシ(1),
```

### License

See [LICENSE](./LICENSE).
