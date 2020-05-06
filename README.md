# nginxTest1
##
'''
n1, u1 등으로 만들어서 테스트
root@u1:~/nginxTest1# docker ps -a
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS                         PORTS                  NAMES
21d5a460917a        nginx               "nginx -g 'daemon of…"   8 minutes ago       Up 8 minutes                   80/tcp                 nginxTest1
579c069e59f2        nginx               "nginx -g 'daemon of…"   27 minutes ago      Up 27 minutes                  80/tcp                 Test1
b3137723afd1        nginx               "nginx -g 'daemon of…"   36 minutes ago      Exited (0) 35 minutes ago                             n1
462100cbfaeb        ubuntu              "/bin/bash"              47 minutes ago      Exited (127) 45 minutes ago                           u1
d42e421fedad        nginx               "nginx -g 'daemon of…"   About an hour ago   Up About an hour               0.0.0.0:8888->80/tcp   T1
72adcb6f28ee        ubuntu              "/bin/bash"              About an hour ago   Exited (0) About an hour ago                          unruffled_hopper


'''


문제 3번 
------------'''
[root@node1 ~]# kubectl run nginxtest --image=euisoo413/nginxtest --port=80
kubectl run --generator=deployment/apps.v1 is DEPRECATED and will be removed in a future version. Use kubectl run --generator=run-pod/v1 or kubectl create instead.
deployment.apps/nginxtest created
[root@node1 ~]# kubectl get deploy
NAME        READY   UP-TO-DATE   AVAILABLE   AGE
nginx       2/2     2            2           6h42m
nginxtest   1/1     1            1           21s
-------------'''
