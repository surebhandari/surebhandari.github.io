K8s
Create the Persistent Volume (PV): In the PV definition, you should label the PV with the desired label (type=logs) so that the PVC can select it based on this label:

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

