# Bazel with Golang

1. Clone this repo.

2. Install Bazel.

Or, if you don't want to install Bazel locally, you can run it in a Docker container e.g.:

```bash
docker-compose run hello bash
```

3. Generate the Bazel BUILD.bazel file(s) for any Go code using gazelle:

```bash
bazel run //:gazelle
```

Notice that this generates hello/BUILD.bazel.

Now we can run the Hello World Go code:

```
bazel run //hello
```
