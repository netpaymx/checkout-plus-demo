# CheckoutPlusDemo

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 14.0.6.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Documentation

[NetPay Docs](https://docs.netpay.com.mx/reference/netpay-checkout-plus).

## Get started

[Configure library](https://github.com/netpaymx/checkout-plus-demo/blob/main/src/index.html).

Test mode:
```javascript
<script src="https://docs.netpay.mx/cdn/js/latest/checkout.plus.dev.js"></script>
```

Live mode:
```javascript
<script src="https://docs.netpay.mx/cdn/js/latest/checkout.plus.dev.js"></script>
```

Set the public key of checkout product:
```javascript
NetPay.init('pk_netpay_sScJQohbaNyOpjRxZJEQUhEXY')
```

Receive the response:
```javascript
function onPaymentSuccess (r) {
    console.log('Success!', r)
}

function onPaymentError (r) {
    console.log('Error!', r)
}
```

[Configure button](https://github.com/netpaymx/checkout-plus-demo/blob/main/src/app/app.component.html).


```javascript
<button id='netpay-checkout'
  data-button-title='Continuar'
  data-street1='Calle y numero'
  data-country='MX'
  data-city='Ciudad'
  data-postal-code='12345'
  data-state='Estado'
  data-token='tokenAmount_hIFFpuUAlvAFxWsvOGFfSFFvX'
  data-phone-number='1234567890'
  data-email='email@dominio.com.mx'
  data-merchant-reference-code='77777777'
  data-onsuccess='onPaymentSuccess'
  data-onerror='onPaymentError'
  data-product-count='1'
  data-commerce-name='Netpay Sandbox'>Pagar
</button>
```