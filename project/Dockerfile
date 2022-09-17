FROM public.ecr.aws/lambda/python:3.9

WORKDIR /build
RUN yum install unzip -y
COPY project/lambda.zip /build
RUN unzip /build/lambda.zip -d /app
WORKDIR /app
CMD ["/app/lambdex_handler.handler"]