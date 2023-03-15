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

- Check config change:
```
nomad job plan example.nomad
```

- After that run, `-check-index` is output of command above:

```
nomad job run -check-index 21 example.nomad
```

- Neu ko the truy cap nomad ben trong vagrant check [here](https://developer.hashicorp.com/nomad/tutorials/get-started/get-started-ui#troubleshooting)
    - Chay nomad dev agent voi `-bind 0.0.0.0`
    - Co the port `4646` bi xung dot. Can check lai terminal se thay port duoc doi lai

- 