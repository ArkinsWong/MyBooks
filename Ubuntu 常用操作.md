## Ubuntu 切换国内源

> `vi /etc/apt/sources.list`
>
> 将以下文字添加到 `source.list`
>
> `deb http://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse`
>
> `deb http://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse`
>
> `deb http://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse`
>
> `deb http://mirrors.aliyun.com/ubuntu/ focal-proposed main restricted universe multiverse`
>
> `deb http://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse`
>
> `deb-src http://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse`
>
> `deb-src http://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse`
>
> `deb-src http://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse`
>
> `deb-src http://mirrors.aliyun.com/ubuntu/ focal-proposed main restricted universe multiverse`
>
> `deb-src http://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse`

---

## GitHub上传超过100M的大文件流程

> 查询当前文件夹下大于100M的文件：`find ./ -type f -size +100M`
>
> 将 xxx/aaa 标记为大文件：`git lfs track "xxx/aaa"`
>
> `git add .`
>
> `git commit -m "add big file aaa to the github"`
>
> `git push -u origin main/master`

