'''
문제 3번은 쿠버네티스가 깔려있는 우분투를 이용하여 사용을 했습니다.
제가 만든 이미지를 활용하여 런을 하였고 레플리카를 20개로 늘렸습니다

'''


문제 3번 ------------''' [root@node1 ~]# kubectl run nginxtest --image=euisoo413/nginxtest --port=80 kubectl run --generator=deployment/apps.v1 is DEPRECATED and will be removed in a future version. Use kubectl run --generator=run-pod/v1 or kubectl create instead. deployment.apps/nginxtest created [root@node1 ~]# kubectl get deploy NAME READY UP-TO-DATE AVAILABLE AGE nginx 2/2 2 2 6h42m nginxtest 1/1 1 1 21s -------------'''
