# Cloud Starts Modules Project  

## 框架模块开发项目  

方便地进行子模块管理与开发

## 首次下载后更新所有子模块

```
git submodule update --init --recursive
```

## 更新所有子模块  

```
git submodule update --recursive --remote
git submodule foreach git pull origin master
```
## 检出所有子模块到指定分支

```
git submodule foreach --recursive 'git checkout master'
```
## 提交所有子模块的变更
```
git submodule foreach --recursive 'git add .'
git submodule foreach --recursive 'git add *'
git submodule foreach --recursive 'git commit -a -m "Update"'
git submodule foreach --recursive 'git push origin master'

```


