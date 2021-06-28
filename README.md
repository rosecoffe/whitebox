# whitebox

[![Data sync](https://github.com/opensourceways/whitebox/actions/workflows/import.yml/badge.svg)](https://github.com/opensourceways/whitebox/actions/workflows/import.yml)

Please add your owner info in data.yaml:

```yaml
- name: 'Your name'
  gitee_id: 'the gitee id'
  github_id: 'the github id'
  gitlab_id: 'the gitlab id'
  alias:
  - "Your alias name"
  - "other alias name"
  # Required, The repo url list you contributed. Only the default branch would be counted.
  repos:
  - https://github.com/opensourceways/whitebox
  - https://gitee.com/opensourceways/whitebox
  # Optional, The repo url list you contributed. All branches would be counted.
  repos_all_branches:
  - https://github.com/apache/spark
```

After your change merged, the repo info would be refreshed in ES index dynamicly.
