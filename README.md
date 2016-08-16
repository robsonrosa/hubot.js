# hubot.js [![Build Status](https://travis-ci.org/robsonbittencourt/hubot.js.svg?branch=master)](https://travis-ci.org/robsonbittencourt/hubot.js)

> A small robot written in Javascript (He doesn't like coffeescript)

[![nodesource/node](http://dockeri.co/image/robsonbittencourt/hubot.js)](https://registry.hub.docker.com/u/robsonbittencourt/hubot.js/)

Hello! My name is Hubot. I'm a robot and my job is to do stuff in Slack chats. At first, I don't know many things, but when gears are attached everything is possible. I love new gears. Feel free to create them.

-- colocar gif mostrando em funcionamento

## How to turn me on?

The first step is to create a bot user on Slack. For this, you can follow [these steps](https://api.slack.com/bot-users). With a bot user created and the token on hand we can go to the next step.

To enable me, it's a piece of cake. I have a recipe of how to build me in [Dockerhub](https://hub.docker.com/r/robsonbittencourt/hubot.js/). Just run the following command:

```
docker run -e BOT_API_KEY=YOUR_SLACK_API_KEY \
   -e BOT_NAME=NAME_OF_YOUR_BOT
   --name=hubot \
   robsonbittencourt/hubot.js
```

## Usage

For now, I don't know how to do many things. But I'm able to understand and to use new gears (features). You can create your own gears. If you think they can be useful for other users, please share it with the world.

### Jenkins

I know  how to invoke your jobs in Jenkins. For this, you need to enter your authorization link to build me.

```
docker run -e BOT_API_KEY=YOUR_SLACK_API_KEY \
   -e BOT_NAME=NAME_OF_YOUR_BOT
   -e JENKINS_AUTH_URL=YOUR_JENKINS_AUTH_URL \
   --name=hubot \
   robsonbittencourt/hubot.js
```

It can be obtained from `yourJenkinsUrl/me/configure`. After that, you can ask me to do your jobs.

```
hubot start job my-deploy
```

--colocar imagem de exemplo

### Help

If you have doubt about the available commands, please ask me for help. I'll be glad to use my gears and knowledge to answer your questions.

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
