<h1>Managing Ephemeral and Persistent Volumes in Kubernetes for Reliable Storage</h1>


<h2>Description</h2>
This project demonstrates Kubernetes volume management by deploying a MySQL database with persistent storage and an Nginx app using ephemeral storage. It helps verify how data is retained or lost when pods are restarted or deleted. 
<br />


<h2>Tools and Technologies</h2>

- Kubernetes
- kubectl
- YAML
- PersistentVolume (PV)
- PersistentVolumeClaim (PVC)
- emptyDir

<h2>Project Walk-through</h2>

<p align="center">
Create a PersistentVolume (PV) to define cluster-level storage <br />
<img src="https://i.postimg.cc/hPSftBGk/1.jpg"/>
<br />
<br />
Create a PersistentVolumeClaim (PVC) to request storage <br/>
<img src="https://i.postimg.cc/zfRfcDdg/2.jpg" />
<br />
<br />
Deploy a MySQL app using the PVC to ensure data survives pod restarts  <br/>
<img src="https://i.postimg.cc/x89T8v9v/3.jpg"/>
<br />
<br />
Deploy an app with ephemeral volumes (emptyDir) to test temporary storage <br/>
<img src="https://i.postimg.cc/0yhkDR82/4.jpg" />
<br />
<br />
Validate volume behavior by deleting pods and checking data persistence or loss <br/>
<img src="https://i.postimg.cc/0j5PP9CZ/5.jpg" />
<br />
<br />
Use ConfigMap as a volume to mount configuration files inside a pod. <br/>
<img src="https://i.postimg.cc/sx0dz7xD/6.jpg" />
<br />
<br />




</p>

