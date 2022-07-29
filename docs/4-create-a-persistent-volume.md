## Purpose of Persistent Volume and Persistent Volume Claim
Data will be independent from our pods. It allows data to be stored that will never be lost. 

## List Storage Cube
`kubectl get sc`

## 1. Apply Persistent Volume File
`apply -f=host-pv.yaml`

## 2. Apply Persistent Volume Claim File
`apply -f=host-pvc.yaml`

## 3. Apply Deployment File
`apply -f=host-deployment.yaml`

## 4. List All Persistent Volumes
Check if PV is succesfully created.
`kubectl get pv`

## 4. List All Persistent Volume Claims
Check if PVC is succesfully created.
`kubectl get pvc`