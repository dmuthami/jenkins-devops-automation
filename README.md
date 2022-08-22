## Getting started

To make it easy for you to get started with GitLab, here's a list of recommended next steps.

Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the temp

## Contributing

State if you are open to contributions and what your requirements are for accepting them.

For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables tha

## License

For open source projects, say how it is licensed.

## Project status

If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.

# Build whichever docker file

docker build .
docker-compose build --no-cache

# build considering docker compose configuration file

docker-compose build

## Run

    docker-compose up

## Logs

docker logs --tail 100 <container id>

## Region

Add jentkins configuration

## Remove all exited containers

docker rm $(docker ps -a -f status=exited -q)

## Remove all images

docker rmi $(docker images -a -q)

# Jenkins credentials cloud

token: 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
expiry = Never
Name=Jenkins_v3

token = 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
Expiry= never
Name=Jenkins integration CI/CD
