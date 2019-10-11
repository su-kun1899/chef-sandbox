# chef-sandbox

## Requirements

1. [chef-workstation 2.4.17](https://downloads.chef.io/chefdk/stable/2.4.17)
1. bundler 1.17

## Quick start

**Setup**
```
$ chef gem install knife-solo
$ cd {project_root}/chef-repo
$ bundle install
```

**確認環境の立ち上げ**
```console
$ cd {project_root}/vagrant
$ vagrant up
```

**ssh 出来るようにしておく**
```
$ vagrant ssh-config --host chef-sandbox >> ~/.ssh/config
```

これで `ssh chef-sandbox` できるようになる。

**レシピの実行**
```console
$ cd {project_root}/chef-repo
$ knife solo cook chef-sandbox
```
