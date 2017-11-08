# stripe_js_facade
Dart JS wrappers for Stripe.js v3 3.0.

## Type definitions
https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/stripe-v3

## Usage
Include the Stripe.js in your HTML:
```html
<script src="https://js.stripe.com/v3/"></script>
...
<div id="card-element"></div>
```

Create simple card element:
```dart
import 'package:stripe_js_facade/stripe_js_facade.dart';
...
final stripe = Stripe(yourStripePublicKey);
final elements = stripe.elements();
final card = elements.create('card', new ElementsOptions());
card.mount('#card-element');
```