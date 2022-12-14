# Challenge AWS
## _Introduccion_

He tomado como reto el challenge AWS del siguiente [link](https://cloudresumechallenge.dev/docs/the-challenge/aws/) que consta de crea un sitio web con cloudfront combinado route53.
Un contador de visita usando lambda con apigateway y dynamodb para almacenar el valor del contador.

### Caracteristicas

- HTML y CSS.
- Cloudfront con Route53.
- Lambda, Apigateway con Dynamodb.
- El lambda esta python.
- Iaas con CDK con TypeScript.

## Arquitectura general

![infra_general](https://user-images.githubusercontent.com/46139464/184558724-0fd0fd61-d615-491d-b8e2-2fca9190390f.png)

## CDK

```
cdk synth
```
```
cdk bootstrap
cdk deploy
```
```
cdk destroy
```

## Comments

the second redirect for the bucket is only necessary if you want people to still find your site when they type "www" in front of it. I recommend people follow that tutorial straight through without skipping any steps because often when they try to use just one bucket, they get confused by the later instructions and start wiring things up wrong