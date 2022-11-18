## Installation

```
ansible-galaxy install -r requirements.yaml
```

### Example usage

Make sure you're authenticated to your cluster with `kubectl`.

Run a command on all nodes:

```
ansible all -a uptime
```

Run a command on only the controllers:

```
ansible controller -a uptime
```

Run a command on only the compute nodes:

```
ansible compute -a uptime
```

Run a command only on external ingress nodes:

```
ansible external_ingress -a 'ip addr show bond0.2180'
```
