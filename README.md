# intellij-codeowners-gem-attribution
attempt to reproduce error for https://github.com/fan-tom/intellij-codeowners/issues/100


# run Docker
Depends on Docker being installed, not going to explain that here

```shell
# To start rails, never local
# docker compose run --no-deps web rails new . --force --database=postgresql
docker compose build
```

1. Set up Docker in JetBrains RubyMine
    1. RubyMine > Settings > Build, Execution, Deployment > Docker
    2. + Add
    3. … Docker for Mac etc
2. Select remote interpreter
   1. RubyMine > Settings > Languages & Frameworks > Ruby SDK and Gems
   2. + Add Remote Interpreter or Version Manager
   3. Docker Compose
   4. Service: web
