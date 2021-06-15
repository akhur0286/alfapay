Библиотека для приема платежей через интернет для Альфабанк.
===========================================================
Библиотека для приема платежей через интернет для Альфабанк.

Установка с помощью Composer
------------


```
php composer.phar require akhur/yii2-alfapay "*"
```

или добавьте в composer.json

```
"akhur/yii2-alfapay": "*"
```

Подключение компонента
-----

Once the extension is installed, simply use it in your code by  :

```php
[
    'components' => [
        'alfapay' => [
            'class' => 'akhur0286\alfapay\Merchant',
            'sessionTimeoutSecs' => 60 * 60 * 24 * 7,
            'merchantLogin' => '',
            'merchantPassword' => '',
            'orderModel' => '', //модель таблицы заказов
            'isTest' => false,
            'registerPreAuth' => false,
            'returnUrl' => '/site/result-payment', //страница обработки
            'failUrl' => '/site/error-payment', //страница ошибки
        ],
        //..
    ],
];
```
