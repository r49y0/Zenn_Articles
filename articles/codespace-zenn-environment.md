---
title: "First Time To Create an Article On Github.dev"
emoji: "💨"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: []
published: true
---

# Flow

1. Open `github.dev`
2. Select Repository to edit Zenn Articles
3. Open Terminal, and type `npm install zenn-cli`. It'll up error.

## Why it happened

Codespaces initial node's tools versions are too old.
So you need to create `devcontainer.json`

# Solution

1. `mkdir -p .devcontainer`
2. `touch .devcontainer/devcontainer.json`
3. edit `devcontainer.json`[^1]

```json:devcontainer.json
{
    "postCreateCommand": "nvm install --lts && nvm use --lts && npm install zenn-cli@latest"
}
```

4. `Shit+Command+P` > `Rebuild Container`
5. Maybe you can run this command on terminal `npx zenn new:article`

I don't know it perfect or there is more elegant method anyway.

[^1]: https://zenn.dev/enlog/articles/efadffc0bfc86b
