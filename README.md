# Zapier Push GitHub Action

This GitHub Action pushes changes to Zapier and sets an environment variable.

## Inputs

- `zapier-deployment-key`: The Zapier deployment key. Required.
- `main-id`: The main ID. Required.
- `main-app-key`: The main app key. Required.
- `base-url`: The base URL. Required.

## Usage

To use this action in your workflow, add the following step:

```yaml
- name: Zapier Push
  uses: NourNafea/zapier-push-action@rc3.7.24
  with:
    zapier-deployment-key: ${{ secrets.ZAPIER_DEPLOYMENT_KEY }}
    main-id: ${{ secrets.MAIN_ID }}
    main-app-key: ${{ secrets.MAIN_APP_KEY }}
    base-url: ${{ secrets.BASE_URL }}
