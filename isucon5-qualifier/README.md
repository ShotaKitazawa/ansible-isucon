# ansible-isucon/isucon5-qualifier

## Overview

Ansible playbook for [ISUCON5-qualifier](http://isucon.net/archives/45166636.html)

## Requirement

- Ubuntu 15.04

## Usage

* Create inventory file
```
cat << '_EOF_' > inventory
[imageservers]
x.x.x.x

[benchservers]
x.x.x.x
_EOF_
```

* Execute
```
ansible-playbook -i inventory playbook.yml
```

## 本来の設定と異なるところ

- ベンチマークはCLIから手動で実行する必要があります
- goのバージョンを依存関係解決のため1.5から1.8に変更しています

## References

- [ISUCON5 予選レギュレーション](http://isucon.net/archives/45347574.html)
- [ISUCON5 予選マニュアル](https://gist.github.com/tagomoris/1a2df5ab0999f5e64cff)
- [isucon/isucon5-qualify](https://github.com/isucon/isucon5-qualify)
- [vagrant-isucon](https://github.com/matsuu/vagrant-isucon)
