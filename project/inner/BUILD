python_sources()

python_awslambda(
    name="lambda",
    runtime="python3.9",
    handler="lambda_example.py:example_handler"
)

docker_image(
    name="myimage",
    dependencies = [":lambda"],
)
