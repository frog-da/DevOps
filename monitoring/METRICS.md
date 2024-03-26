# Configured Prometheus: 
![image](https://github.com/frog-da/DevOps/assets/84839431/496d89dd-7cc5-4441-a525-0476e63fe4d6)

# Dasboards screenshots:
## Loki:
![image](https://github.com/frog-da/DevOps/assets/84839431/5ac7e10c-34d1-447f-ae41-10714dc09fcc)
![image](https://github.com/frog-da/DevOps/assets/84839431/713c6906-27c8-4444-a3ec-6dcd6f868641)
![image](https://github.com/frog-da/DevOps/assets/84839431/16f1c77f-e8ed-40f7-90ac-1cbcdacc886e)

## Prometheus:
![image](https://github.com/frog-da/DevOps/assets/84839431/92fe84c9-d260-4b1b-ab6a-70c9c2c3dce6)
![image](https://github.com/frog-da/DevOps/assets/84839431/339beb1a-a530-4beb-a9df-0f45cd39a964)
![image](https://github.com/frog-da/DevOps/assets/84839431/1b51fb1a-cf7c-4a24-acb5-b352126b7d98)

## Service Configuration Updates:

- Log rotation is implemented by specifying the `max-size` and `max-file` options of logging with `json-file` driver.
- Memory limits are specified by adding such field to containers:

```yaml
deploy:
  resources:
    limits:
      memory: 500M
```

that limits container memory usage to 500MB
