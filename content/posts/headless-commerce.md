---
date: 2020-05-30T23:12:07Z
hero_image: "/content/images/sarah-dorweiler-9Z1KRIfpBTM-unsplash.jpg"
title: Headless Commerce
author: Ben Morris

---
Here is a headless commerce example with a buy button

'code'

<div id='product-component-1589836932696'></div>
<script type="text/javascript">
/_<!\[CDATA\[_/
(function () {
var scriptURL = 'https://sdks.shopifycdn.com/buy-button/latest/buy-button-storefront.min.js';
if (window.ShopifyBuy) {
if (window.ShopifyBuy.UI) {
ShopifyBuyInit();
} else {
loadScript();
}
} else {
loadScript();
}
function loadScript() {
var script = document.createElement('script');
script.async = true;
script.src = scriptURL;
(document.getElementsByTagName('head')\[0\] || document.getElementsByTagName('body')\[0\]).appendChild(script);
script.onload = ShopifyBuyInit;
}
function ShopifyBuyInit() {
var client = ShopifyBuy.buildClient({
domain: 'powderla.myshopify.com',
storefrontAccessToken: 'bd1d2ecff566e0d41355e73be4204e35',
});
ShopifyBuy.UI.onReady(client).then(function (ui) {
ui.createComponent('product', {
id: '4412851880011',
node: document.getElementById('product-component-1589836932696'),
moneyFormat: '%24%7B%7Bamount%7D%7D',
options: {
"product": {
"styles": {
"product": {
"@media (min-width: 601px)": {
"max-width": "calc(25% - 20px)",
"margin-left": "20px",
"margin-bottom": "50px"
}
}
},
"text": {
"button": "Add to cart"
}
},
"productSet": {
"styles": {
"products": {
"@media (min-width: 601px)": {
"margin-left": "-20px"
}
}
}
},
"modalProduct": {
"contents": {
"img": false,
"imgWithCarousel": true,
"button": false,
"buttonWithQuantity": true
},
"styles": {
"product": {
"@media (min-width: 601px)": {
"max-width": "100%",
"margin-left": "0px",
"margin-bottom": "0px"
}
}
},
"text": {
"button": "Add to cart"
}
},
"cart": {
"text": {
"total": "Subtotal",
"button": "Checkout"
}
}
},
});
});
}
})();
/_\]\]>_/
</script>

    <div id='product-component-1589836932696'></div>
    <script type="text/javascript">
    /*<![CDATA[*/
    (function () {
      var scriptURL = 'https://sdks.shopifycdn.com/buy-button/latest/buy-button-storefront.min.js';
      if (window.ShopifyBuy) {
        if (window.ShopifyBuy.UI) {
          ShopifyBuyInit();
        } else {
          loadScript();
        }
      } else {
        loadScript();
      }
      function loadScript() {
        var script = document.createElement('script');
        script.async = true;
        script.src = scriptURL;
        (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(script);
        script.onload = ShopifyBuyInit;
      }
      function ShopifyBuyInit() {
        var client = ShopifyBuy.buildClient({
          domain: 'powderla.myshopify.com',
          storefrontAccessToken: 'bd1d2ecff566e0d41355e73be4204e35',
        });
        ShopifyBuy.UI.onReady(client).then(function (ui) {
          ui.createComponent('product', {
            id: '4412851880011',
            node: document.getElementById('product-component-1589836932696'),
            moneyFormat: '%24%7B%7Bamount%7D%7D',
            options: {
      "product": {
        "styles": {
          "product": {
            "@media (min-width: 601px)": {
              "max-width": "calc(25% - 20px)",
              "margin-left": "20px",
              "margin-bottom": "50px"
            }
          }
        },
        "text": {
          "button": "Add to cart"
        }
      },
      "productSet": {
        "styles": {
          "products": {
            "@media (min-width: 601px)": {
              "margin-left": "-20px"
            }
          }
        }
      },
      "modalProduct": {
        "contents": {
          "img": false,
          "imgWithCarousel": true,
          "button": false,
          "buttonWithQuantity": true
        },
        "styles": {
          "product": {
            "@media (min-width: 601px)": {
              "max-width": "100%",
              "margin-left": "0px",
              "margin-bottom": "0px"
            }
          }
        },
        "text": {
          "button": "Add to cart"
        }
      },
      "cart": {
        "text": {
          "total": "Subtotal",
          "button": "Checkout"
        }
      }
    },
          });
        });
      }
    })();
    /*]]>*/
    </script>