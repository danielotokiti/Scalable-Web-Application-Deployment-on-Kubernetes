# Day 3: High Availability & Backup
  
## Tasks Completed:
  - Verified 3 replicas of currency-api deployment were running
  - Deleted one pod to simulate a failure
  - Observed Kubernetes automatically recreate the pod (self-healing)
  - Exported all cluster resources into a backup file (backup.yaml)
  - Verified backup file was saved locally

# Screenshots:
  - kubectl get pods before and after deleting a pod (showing self-healing)
  - kubectl delete pod <pod-name> command output
  - Local directory showing backup.yaml file created
