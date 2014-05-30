# Dockerfile for [gogits/gogs](https://github.com/gogits/gogs)
* This dockerfile installs ssh, curl, unzip, git, supervisord and Gogs(Go Git Service)

## Usage
```
git clone https://github.com/brimstone/docker-gogits
cd docker-gogits
docker build -t brimstone/gogits .
data_dir="$(HOME)docker_data"
docker run --name="gogits" -d -p 2222:22 -p 3000:3000 -v $data_dir/gogits:/home/git brimstone/gogits
```
