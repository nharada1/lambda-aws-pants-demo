FROM public.ecr.aws/lambda/python:3.9

WORKDIR /build
RUN yum install unzip -y
COPY project.inner/lambda.zip ${LAMBDA_TASK_ROOT}
ENV PYTHONPATH ${LAMBDA_TASK_ROOT}/lambda.zip
CMD ["__pex__.inner.lambda_example.example_handler"]