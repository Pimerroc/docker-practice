# To execute it run the folowing
```bash
docker buildx build --builder=container-builder --platform=linux/amd64,linux/arm64 -t pimerroc/ddd-book:ch8.1 --push .
```
If you don`t have one, then create it via
```bash 
docker buildx create --name container-builder --driver docker-container --bootstrap --use
```
Create a cloud builder (only with subscription):
```bash
docker buildx create --driver cloud pimerroc/zzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz
```

