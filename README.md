# yii2-widget-linkpager
LinkPager widgets for Yii Framework 2.0
===============================
Increase the pageSize of the page drop-down box
![Effect picture 1](https://github.com/liyunfang/wr/blob/master/images/yii2-widget-linkpager-1.png "Effect picture 1")  
![Effect picture 2](https://github.com/liyunfang/wr/blob/master/images/yii2-widget-linkpager-2.png "Effect picture 2") 




Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
 composer require  life2016/yii2-linkPager
```

or add

```
"life2016/yii2-linkPager": "*"
```

to the require section of your `composer.json` file.

Requirements
------------
This extension require twitter-bootstrap

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

