# Spring MVC Projectのひな形

STSをインストールしてもプロジェクトが作成できない場合に、プロジェクトのひな形として使用する。

```
PNAME="new project name"

git clone https://github.com/MATSUMOTO-Takashi/spring_mvc_project.git
mv spring_mvc_project $PNAME
cd $PNAME
rm -rf .git
git init

find spring_mvc_project -type f | xargs sed -i "" "s/spring_mvc_project/$PNAME/g"
```

※ sedはMacの場合の書き方
