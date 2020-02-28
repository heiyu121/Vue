# travel

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

## git

```py
# 查看本地分支
$ git branch
* master

# 查看远程分支
git branch -r

# 查看所有分支
git branch -a

# 本地创建新的分支
git branch [branch name]

# 切换到新的分支
git checkout [branch name]

# 创建+切换分支
git checkout -b [branch name]

# 将新分支推送到github
git push origin [branch name]

# 删除本地分支
git branch -d [branch name]

# 查看自己所在分支
git status
```

### Github 本地分支合并到线上主分支

```py
https://www.cnblogs.com/aiyr/p/10055448.html
如果是在本地index-swiper分支上，已经写好了那么：

1，git add .         　　　　　　　　　　   //提交到本地缓冲区

2，git commit -m "project init" 　　　　//把本地缓冲区提交到本地仓库

3，git push 　　　　　　　　　　　　　//把分支推送至到github         如果是第一次提交： git push  --set-upstream origin index-icons，放心如果不加的话也提交不成功。

4，git checkout master 　　　　　　　　// 先切换到master分支
5，git merge origin/index-swiper 　　　　// 把线上index-swiper分支上的内容合并到本地master分支          这里origin/index-swiper代表线上的Index-swiper分支，git merge代表想跟哪个分支合并。在哪个环境下就合并哪个
6，git push　　　　 　　　　　　　　　　// 将本地master分支push到线上master分支
```



