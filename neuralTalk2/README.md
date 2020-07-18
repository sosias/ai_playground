# NeuralTalk2

RNN to tag images with an articulated sentence. Source repo https://github.com/karpathy/neuraltalk2 docker container repo https://github.com/SaMnCo/docker-neuraltalk2

## How to run it

download the model from http://cs.stanford.edu/people/karpathy/neuraltalk2/checkpoint_v1_cpu.zip

extract the `.t7` file inside the `data/model` directory

put the images that you want to tag inside the `data/images` directory. The images need to have a `.jpg` exstension

run
```
$ docker-compose up
```

in browser go to http://localhost:8000/vis

## Re-run on new images

simply restart the container

or

```
docker exec neuraltalk2 /run.sh
```