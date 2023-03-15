# Nomad demo

- Install nomad on vagrant follow [hashcorp official](https://developer.hashicorp.com/nomad/tutorials/get-started/get-started-install)


- Run vagrant

```
vagrant up
```

- Do chay nomad trong vagrant machine nen cac lenh lien quan nomad deu thuc hien trong machine.

- Check nomad node status:
```
nomad node status
```

- Check server members:

```
nomad server members
```


- Create job:

```
nomad job init
```

- De bo qua comment dung `-short`: 
```
nomad job init -short
```

- Run nomad job: 
```
nomad job run example.nomad
```

- Check job status:

```
nomad job status example
```

- To check allocation use command:
```
nomad alloc status <alloc_id>
```

- To check logs of allocation:

```
nomad alloc logs <alloc_id>
```