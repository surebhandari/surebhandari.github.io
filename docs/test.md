Test file
apiVersion: v1
kind: PersistentVolume
metadata:
  name: log-pv
  labels:
    type: logs
spec:
  capacity:
    storage: 1Gi
  accessModes:
    - ReadWriteOnce
  # ... other PV specifications ...

