# Security and Privacy

- Never commit credentials, tokens, private keys, `secrets.yaml`, customer data, or private commercial information.
- Keep local machine paths out of public documentation where possible; absolute paths are used here only for operational setup.
- Use `.env.example` or a documented configuration template for non-secret defaults.
- Review Git history as well as the working tree before publishing a repository; removing a file from the current tree does not remove it from history.
- Product repositories own their own secret handling and must not rely on platform defaults to protect credentials.
