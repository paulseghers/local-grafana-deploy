### For locally testing prometheus metrics endpoint
Be careful of the required permissions of the stuff inside `/grafana`
To find out:
```
docker run --rm -it --entrypoint sh grafana/grafana-oss
```
Look at the id that `id` command returns in the container's runtime, then 
```
sudo chown <id>:<id> -R grafana
```
with the id that you got above
