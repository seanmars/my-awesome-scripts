
## Docker

### 刪除所有 status={status} 的 container，以下為一些常用的 status 狀態：

- exited
- dead

```shell
docker rm -v $(docker ps --filter status={status} -q)
```

**Note:** `-v` 會刪除 container 的 volume。

### 刪除所有 container

```shell
docker rm -v -f $(docker ps -qa)
```

**Note:**
  - `-v` 會刪除 container 的 volume
  - `-f` 會強制刪除正在運行的 container