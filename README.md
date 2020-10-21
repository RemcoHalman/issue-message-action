## Welcoming message
This GitHub Action will reply to all new Issues and Pull Requests with a custom message

Example usage (you can change the replies for issue-message and pr-message)

```
  welcome:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v1
      - uses: ./src/welcome
        with:
          github-token: ${{ secrets.GITHUB_TOKEN }}
          issue-message: "<h1>It's great having you contribute to this project</h1> Feel free to raise an <strong>Issue</strong>! And of course welcome to the <strong>project</strong> :nerd_face:"
          pr-message: "<h1>It's great having you contribute to this project</h1> Feel free to create a <strong>Pull Request</strong>! And of course welcome to the <strong>project</strong> :nerd_face:"
```

<small>https://github.com/EddieJaoudeCommunity/gh-action-community</small>