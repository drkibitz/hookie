hookie
===================

wraps a few of github's v3 API webhooks calls

#### install
```bash
$ pip install https://github.com/smlstvnh/hookie/archive/master.zip
```

#### dev/install
```
(fork it)
$ git clone git@github.com:<your-username>/hookie
$ cd hookie
$ pip install -e .
```

#### usage
set up your `hookie/hookie.yaml` and go

see existing hooks and their parameters
```bash
$ hookie show -u smlstvnh -r hookie
```

create a new hook which triggers on a new pull request or issue comment (currently the default)
```bash
$ hookie run --create http://jenkins.hookie.net:8080/ghprbhook/ -u smlstvnh -r hookie
```


