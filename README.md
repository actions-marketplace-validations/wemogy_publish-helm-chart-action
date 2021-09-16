# ![wemogy](https://wemogyimages.blob.core.windows.net/logos/wemogy-github-tiny.png) Publish Helm Chart (GitHub Action)

A GitHub Action to publish Helm Charts to the wemogy Helm repository

## Usage

```yaml
- name: Publish Helm Chart
  uses: wemogy/publish-helm-chart-action@1.0.1
  with:
    name: wemogy-demo
    path: env/helm/wemogy-demo/wemogy-demo-1.0.0.tgz
    token: ${{ secrets.HELM_REPO_TOKEN }}
```

## Inputs

| Input            | Description                                  |
| ---------------- | -------------------------------------------- |
| `name`           | **Required** Name of the Helm Chart     |
| `path` | **Required** Path to the packaged Helm Chart cluster |
| `token` | **Required** Access Token to the Helm Git repository |

## Outputs

None.
