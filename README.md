# vagrant-awscli
A simple repo to have awscli installed on a VM

## pre-requirements
- [x] vagrant installed
- [x] virtualbox installed
- [x] git available, to do `git clone`

## how to create this VM

- clone this repo
```
git clone https://github.com/kikitux/vagrant-awscli
```
- change into the directory
```
cd vagrant-awscli
```
- create this vm
```
vagrant up
```

## how to use
- connect to the vm
```
vagrant ssh
```

- set credentials
```
export AWS_ACCESS_KEY_ID=<ID>
export AWS_SECRET_ACCESS_KEY=<KEY>
```

- change to the vagrant folder
```
cd /vagrant
```

- now you can perform commands on S3 like list/copy
```
aws s3 ls s3://<bucket>/<path>/
aws s3 cp s3://<bucket>/<path>/<file.zip> .
```
