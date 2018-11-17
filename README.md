# An ansible role for setting up a node for ansible role CI [![Build Status](https://travis-ci.com/mafalb/ci.svg?branch=master)](https://travis-ci.com/mafalb/ci)


## Basic Usage

```
before_install:
  ...
  - ansible-playbook -b -D -t all,debug gen_requirements.yml
  - ansible-playbook -b -D -t all,debug before_install.yml
install:
  - ansible-playbook -b -D -t all,debug install.yml
  ...
```

## License

GPLv3

