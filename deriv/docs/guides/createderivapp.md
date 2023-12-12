# Create a Deriv application

## Create a Deriv account
If you don't have a Deriv account yet, you can easily create one by visiting our signup page or using the new_account_virtual API call. It's completely free. And if you have an account already, please log in using your account details. To avoid any accidental loss of funds during testing, we recommend using your demo account instead of a real account.

To earn markup, get a Deriv real account to receive your monthly earnings. You can also create a real account using new_account_real or new_account_maltainvest API calls.

> **Important** To create Deriv applications, you'll need an API token with the Admin scope for the account you wish to use for your application.

## Create a Deriv API token
To create your API token, simply go to the Dashboard and select the **Manage Tokens** tab. From there, create a new token that matches the access level needed for your application's features.

To create a new API token, follow these steps:

1. Select the scopes you need.
2. Provide a name for your token.
3. Click **Create**.

Alternatively, you can create an API token via the api_token API call.

## Deriv application
To create your application with the appropriate configuration options, select the **Register Application** tab in the **Dashboard**. You can make changes to your application's configuration at anytime in the **Manage Applications** tab.

### Create a Deriv application
1. Select the account you want to create the application with.
2. Select the API token added to your account ( it must have the `Admin` scope ).
3. Provide a name for your application.
4. Fill the **Markup** and **OAuth details** fields.
5. Select the **Authorisation Scopes** needed by your application.
6. Click **Register Application**.

Make sure the **Authorisation** and **Verification URLs** are correct based on your implementation.

For example, if your domain is `https://example.com` and your authorisation and authentication are handled by `verfiy`, your URLs will be:

`https://example.com/verify`

| App information field     | Description |
| ----------- | ----------- |
| Account | The account you want to create the application with. |
| API Token | The API token you want to create the application with. |
| App Name | The API token you want to create the application with. |
| Markup	| The commission added to the trade price to earn additional income. |
| Authorisation URL	| The URL that enables clients to log in to your app using their Deriv accounts without an API token. |
| Verification URL	| The OAuth redirect URL for the OAuth authorisation. |
