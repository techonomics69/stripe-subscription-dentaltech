# Using Checkout for subscriptions

Combining Checkout and Billing is the fastest way to get a subscription payment page up and running on Stripe.

[Checkout](https://stripe.com/docs/payments/checkout) is a pre-built payment page that lets you accept cards and Apple Pay while [Billing](https://stripe.com/docs/payments/checkout) is a suite of APIs that lets you model complex subscription plans. Together they bring you subscription superpowers by letting you creating subscriptions for your products -- in some cases without the need for a server 🥳.

Once your customer is ready to pay, use Stripe.js to redirect them to the URL of your Stripe hosted payment page with the ID of your Billing [Plan](https://stripe.com/docs/api/plans).

<img src="./checkout-demo.gif" alt="A gif of the Checkout payment page rendering" align="center">

**Features:**

- Localization in 14 different languages 🌍
- Built-in Apple Pay support 🍎
- Built-in dynamic 3D Secure (ready for SCA) 🔔
- Plans to support more payment methods 🔮

For more features see the [Checkout documentation](https://stripe.com/docs/payments/checkout/subscriptions).

There are two integrations: [client-only](./client-only) and [client-and-server](./client-and-server).

This CodeSandbox shows the client-and-server integration to see the code for a client-only integration, please see the GitHub repository:

https://github.com/stripe-samples/checkout-single-subscription/tree/master/client-only

## How to run locally

If you want to run the recipe locally, copy the .env.example file to your own .env file in this directory:

```
cp .env.example .env
```

You will need a Stripe account with its own set of [API keys](https://stripe.com/docs/development#api-keys).

## FAQ

Q: Why did you pick these frameworks?

A: We chose the most minimal framework to convey the key Stripe calls and concepts you need to understand. These demos are meant as an educational tool that helps you roadmap how to integrate Stripe within your own system independent of the framework.

Q: Can you show me how to build X?

A: We are always looking for new recipe ideas, please email dev-samples@stripe.com with your suggestion!

## Author(s)

[@adreyfus-stripe](https://twitter.com/adrind)
