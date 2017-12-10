# hubot-miniyon

## Installation

```
$ npm install -g yo generator-hubot
$ mkdir hubot-miniyon && cd hubot-miniyon
$ yo hubot
```

## Running Locally

```
$ bin/hubot
hubot-miniyon> hubot-miniyon help
```

## Infrastructure

Cloud Foundary with IBM Bluemix.

> Ref. [Qiita: IBM Bluemixを使って、Slackで動くHubotを構築する手順](https://qiita.com/Amebayashi/items/ca979ec6f925abc7713f)

## Deployment

Install bx cli.

> Ref. [Bluemix CLI](https://console.bluemix.net/docs/cli/index.html)

```
$ bx app push
$ bx app env-set hubot-miniyon HUBOT_SLACK_TOKEN {SLACK_TOKEN}
$ bx app env-set hubot-miniyon HUBOT_GOOGLE_CSE_ID {GOOGLE_CSE_ID}
$ bx app env-set hubot-miniyon HUBOT_GOOGLE_CSE_KEY {GOOGLE_CSE_KEY}
$ bx app env-set hubot-miniyon HUBOT_SLACK_BOTNAME {hubot-name}
$ bx app restage hubot-miniyon
```

> Ref. [Qiita: hubot-google-image で Google Custom Search API を利用する設定](https://qiita.com/hoto17296/items/f27ebf62c6015befdaa8)

## Log

```
$ bx app logs hubot-miniyon --recent
```

## Author

kadoyama.keisuke@gmail.com
