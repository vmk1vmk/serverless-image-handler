FROM public.ecr.aws/lambda/nodejs:12
# https://github.com/aws/aws-lambda-base-images/blob/nodejs12.x/Dockerfile.nodejs12.x

COPY index.js thumbor-mapping.js image-*.js package*.json ./
RUN npm install

CMD [ "index.handler" ]