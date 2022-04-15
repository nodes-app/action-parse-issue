[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/nodes-app/action-issue-to-json)

# action-issue-to-json

## Usage

```yml
- name: Parse Issue to JSON
  uses: nodes-app/action-issue-to-json@v1
  with:
    issue-body: ${{ github.event.issue.body }}
    template: example.md
```

### Outputs

Name | Description
--- | ---
`result` | Issue in JSON format
`error` | Validation Error (empty if no error occurred)
