# yii2-linkpager
LinkPager widgets for Yii Framework 2.0
===============================
![Effect picture 1](https://github.com/ran1990/yii2-linkpager/blob/master/image.png "Effect picture 1")  




Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
 composer require  life2016/yii2-linkpager
```

or add
```
"life2016/yii2-linkpager": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

GridView options
```
 <?= GridView::widget([
        'dataProvider' => $dataProvider,
        'columns' => [
        ],
        'pager' => [
            'class' => \components\widgets\LinkPager::className(),
            'template' => '{pageButtons} {customPage}',#默认显示数字+自定义输入框
        ],
    ]); ?>
 ```

