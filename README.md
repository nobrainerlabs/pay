# Get Paid
Like most engineers, I may have a blog or a personal project page but nothing that offers interested parties a way to buy my services. This project is dedicated to being a fast way to bring up a services site, to show offerings and allow clients to pay you.

## Demo
[https://paid.netlify.app/](https://paid.netlify.app/)

## Stripe Connection
This project connects with your Stripe account and uses the API to pull Products and Plans from your Stripe account. You can use Stripe as your Product management interface.

## Getting Started

### Setup

1. Clone the repository
2. Setup a Stripe account and retrieve Stripe's `publishable` and `secret` key
3. Copy dev.env as .env
4. Update .env with Keys from Stripe

```
STRIPE_PUBLIC_KEY={{publishable}}
STRIPE_PRIVATE_KEY={{secret}}
URL={{the full url of your site}}
```

### Running
To start the project, run,

1. `yarn dev` for development
2. `yarn generate` to create the `./dist` files to publish to CDN (I use netlify and I call generate for build)
