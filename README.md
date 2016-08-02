# hubot.js [![Build Status](https://travis-ci.org/robsonbittencourt/hubot.js.svg?branch=master)](https://travis-ci.org/robsonbittencourt/hubot.js)

> A small robot written in Javascript (He does not like coffeescript)

[![nodesource/node](http://dockeri.co/image/robsonbittencourt/hubot.js)](https://registry.hub.docker.com/u/robsonbittencourt/hubot.js/)

Hello my name is Hubot. I'm a robot and I work doing things in Slack chats. At first, I do not know many things, but I love new gears. Feel free to create them.

-- colocar gif mostrando em funcionamento

## How turn on?

The first step is to create a bot user on Slack. For this you can follow [these steps](https://api.slack.com/bot-users). With a bot created and the token in hand we can go to the next step.

To enable me is very simple. I have a recipe of how to build me in [Dockerhub](https://hub.docker.com/r/robsonbittencourt/hubot.js/). Just run the following command:

```
docker run -e BOT_API_KEY=YOUR_SLACK_API_KEY \
   -e BOT_NAME=NAME_OF_YOUR_BOT
   --name=hubot \
   robsonbittencourt/hubot.js
```

## Usage

For now I do not know how to do many things. New gear (features), can they be added in the future. You can create your gears. If you think they can be useful to others, please send a pull request.

### Jenkins

I know invoke their jobs in Jenkins. For this you need to enter your authorization link to build me.

```
docker run -e BOT_API_KEY=YOUR_SLACK_API_KEY \
   -e BOT_NAME=NAME_OF_YOUR_BOT
   -e JENKINS_AUTH_URL=YOUR_JENKINS_AUTH_URL \
   --name=hubot \
   robsonbittencourt/hubot.js
```

It can be obtained from `yourJenkinsUrl/me/configure`. After that you can ask me to do their jobs.

```
hubot start job my-deploy
```

--colocar imagem de exemplo

### Help

If you have questions about the available commands can ask me for help.

```
hubot help
```

--colocar imagem de exemplo

## Development setup
TODO


## Meta
Robson Bittencourt - @rluizv - robson.luizv@gmail.com

Distributed under the MIT license. See [LICENSE](LICENSE) for more information.

https://github.com/robsonbittencourt/hubot.js
