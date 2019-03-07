# Firebase Cloud Functions Boilerplate

Template for having split up cloud functions (_triggers_/_endpoints_) with included `jest` testing.

## Usage

Requires **firebase-tools**:

```sh
$ npm i -g firebase-tools
```

Install all dependencies:

```sh
$ npm install
```

add your firebase project

```sh
$ firebase use --add
```

Add your `service-account.json` to the `functions` folder:

```diff
{
+    "type": "service_account",
+    "project_id": "",
+    "private_key_id": "",
+    "private_key": "",
+    "client_email": "",
+    "client_id": "",
+    "auth_uri": "",
+    "token_uri": "",
+    "auth_provider_x509_cert_url": "",
+    "client_x509_cert_url": "",
}
```

Fill in your API details in `config/*.json`

Development: `firebase serve` with hot-reloading

```sh
$ npm run dev
```

Testing: jest

```sh
$ npm test
```

## Config

### Node.js v8

Currently in beta. If you experience issues feel free to remove from `package.json`

```diff
-  "engines": {
-    "node": "8"
-  },
```

## Useful links

- [Develop Apps Script using TypeScript](https://developers.google.com/apps-script/guides/typescript)
- [Firebase CLI Reference](https://firebase.google.com/docs/cli/)
- [Unit testing of Cloud Functions](https://firebase.google.com/docs/functions/unit-testing)
- [How to Test Firebase Cloud Functions With Jest](https://angularfirebase.com/lessons/testing-cloud-functions-in-firebase/)

## License

MIT
