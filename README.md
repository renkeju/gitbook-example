[1]: http://gitbook.zhangjikai.com/bookjson.html
[2]: /images/create_a_new_repository.png

# Gitbook Template

## 项目结构

1. 克隆模版并去掉模版中的历史记录

    ```
    git clone https://github.com/renkeju/gitbook-template
    cd gitbook-template && rm -rf .git
    ```

2. 修改模版

    * `.travis.yml`

        * recipients: 修改为你个人邮件地址
        * REF: 修改为你的 github 项目地址

    * `book.json`

        修改 gitbook 相应配置，可以参考此文档 [book.json配置文件]

    * `SUMMARY.md` 
        
        定义目录结构

3. 在 github 上创建新项目

    比如我对新仓库命名为 l2tp-usage-guide

    ![创建一个新的仓库][2]

    把修改好的模版 push 到新的仓库 

    ```
    git remote add origin git@github.com:renkeju/l2tp-usage-guide.git
    git push -u origin master
    ```

## Github Pages

1. 新建 gh-pages 分支:

    ```
    git checkout -b gh-pages
    git push origin gh-pages
    ```

2. 在项目 `Settings` -> `GitHub Pages`开启 Github Pages 服务:

    
