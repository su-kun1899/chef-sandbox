# chef-sandbox

## Setup

1. chef-workstation の[ダウンロード](https://downloads.chef.io/chef-workstation/0.9.42#mac_os_x)
1. knife-solo のインストール
  - `chef gem install knife-solo`

## Vagrant による Sandbox 環境

### 起動

```
cd vagrant
vagrant up
```

### setup ssh

```
vagrant ssh-config --host chef-sandbox >> ~/.ssh/config
```

これで `ssh chef-sandbox` できるようになる。
