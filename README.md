https://docs.gitlab.com/omnibus/docker/
https://docs.gitlab.com/omnibus/docker/#install-gitlab-using-docker-compose

docker build -t gitlab .

docker run --detach -e GITLAB_OMNIBUS_CONFIG="external_url 'http://gitlab.example.com:8012'" -e 'GITLAB_PORT=8012' -e 'GITLAB_HOST=192.168.33.10' --hostname gitlab.example.com --publish 8012:80 --publish 2001:22 --name gitlab --restart always gitlab

docker exec {����ƥ�ID or tagname} gitlab-ctl start

vi /etc/gitlab/gitlab.rb

docker-compose up

sudo vi /etc/hosts
127.0.0.1 gitlab.example.com

�ѥ���`�ɉ���������

�m���˥�ݥ��ȥ�����

�ܥ��`������

setting -> CI/CD -> runner
�� http://blog.catalyst-system.jp/environment-0003/

docker exec -it {runner�Υ���ƥ�ID} gitlab-runner register
http://gitlab.example.com:8018/
qTGLVgK4ENtXJC1oTUVe
docker
docker:latest

�_�J
docker exec -it 9fba9accda3d vi /etc/gitlab-runner/config.toml

cat ~/.ssh/id_rsa.pub
�N�긶����

----- rails

https://qiita.com/reflet/items/efb624996f8876f8167e
