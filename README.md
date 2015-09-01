# kargojs

Türkiye Kargo firmalarından rahatça sorgulama yapabilmek için geliştirilen npm modülü.

## Kullanım

```js

var kargojs = require('./index');


kargojs.Yurtici.query("107683143283",function(err,data){
    console.log(err ? err : data);
})


kargojs.Yurtici.getMovements("107683143283",function(err,data){
    console.log(err ? err : data);
})


kargojs.Aras.query("5560228801279",function(err,data){
    console.log(err ? err : data);
})


kargojs.Aras.getMovements("5560228801279",function(err,data){
    console.log(err ? err : data);
})

```

## Aktif kargo firmaları
Şuan için aktif olan firmalar Aras ve Yurtiçi kargo firmalarıdır. Diğer firmaları da yavaş yavaş ekleyeceğim.

## Testler
Henüz test yazmadım, bazı yerlerde de saçma sapan hackler kullanarak sonuca ulaşmaya çalıştım. Lütfen ürün ortamında kullanmadan önce inceleyin, saçma bulduğunuz yerler için issue oluşturabilirseniz sevinirim.
