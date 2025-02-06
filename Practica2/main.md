<div align="center">
<h1>PRACTICA 1</h1> 
<h3>Nombre: Antonio López Martínez</h3>  
<h3>Numero Control: 22121322</h3>  
<h3>Maestra: Brenda</h3> 
<img src="portada.jpeg" alt="Portada"></img> 
</div>

--- 

Primero identificamos los procesos que se esten ejecutando

```bash
mutablename96@mutablename96-Nitro-AN515-54:~$ top

top - 13:09:26 up 11 min,  1 user,  load average: 1,59, 1,72, 1,05
Tareas: 359 total,   1 ejecutar,  358 hibernar,    0 detener,    0 zombie
%Cpu(s):  1,9 us,  0,9 sy,  0,0 ni, 97,1 id,  0,0 wa,  0,0 hi,  0,1 si,  0,0 st 
MiB Mem :  15832,5 total,   7933,3 libre,   4463,7 usado,   4473,8 búf/caché     
MiB Intercambio:   4096,0 total,   4096,0 libre,      0,0 usado.  11368,8 dispon Mem 

    PID USUARIO   PR  NI    VIRT    RES    SHR S  %CPU  %MEM     HORA+ ORDEN                                                                                                             
   6326 mutable+  20   0  852272  54652  43188 S   7,9   0,3   0:01.57 gnome-terminal-                                                                                                   
   2229 mutable+  20   0   25,0g 168848 111156 S   7,3   1,0   0:40.83 Xorg                                                                                                              
   2497 mutable+  20   0 4604824 306908 135168 S   4,6   1,9   0:53.74 gnome-shell                                                                                                       
    911 avahi     20   0   14056   8960   3840 S   4,0   0,1   1:24.84 avahi-daemon                                                                                                      
    967 root      20   0  345804  19184  16496 S   2,0   0,1   0:11.41 NetworkManager                                                                                                    
    275 root     -51   0       0      0      0 S   1,3   0,0   0:07.12 irq/136-SYNA7DB5:01                                                                                               
    628 root     -51   0       0      0      0 S   1,3   0,0   0:12.58 irq/146-iwlwifi                                                                                                   
   5006 mutable+  20   0 1156,1g 183656 120888 S   1,3   1,1   0:13.67 msedge                                                                                                            
   6423 mutable+  20   0   23424   6144   3840 R   1,0   0,0   0:00.11 top                                                                                                               
   2586 mutable+  20   0  236056   7808   7040 S   0,7   0,0   0:00.33 at-spi2-registr                                                                                                   
   5278 mutable+  20   0 4596228 291488 188600 S   0,7   1,8   0:04.34 spotify                                                                                                           
     24 root      20   0       0      0      0 S   0,3   0,0   0:02.03 ksoftirqd/1                                                                                                       
   3581 mutable+  20   0   32,9g 400284 260256 S   0,3   2,5   1:22.35 msedge                                                                                                            
   3631 mutable+  20   0   32,5g 111584  84680 S   0,3   0,7   0:16.80 msedge                                                                                                            
   4374 mutable+  20   0 1157,9g 215872 146444 S   0,3   1,3   0:13.72 code                                                                                                              
   4775 mutable+  20   0 1157,7g 163420  79104 S   0,3   1,0   0:07.98 code                                                                                                              
   5702 mutable+  20   0   32,6g  90192  62484 S   0,3   0,6   0:03.99 whatsapp-linux-                                                                                                   
   5723 mutable+  20   0   32,4g  74480  63472 S   0,3   0,5   0:01.24 whatsapp-linux-                                                                                                   
   5778 mutable+  20   0 1134,2g 205964 125628 S   0,3   1,3   0:22.26 whatsapp-linux-                                                                                                   
      1 root      20   0   23620  13720   8984 S   0,0   0,1   0:02.91 systemd                                                                                                           
      2 root      20   0       0      0      0 S   0,0   0,0   0:00.00 kthreadd                                                                                                          
      3 root      20   0       0      0      0 S   0,0   0,0   0:00.00 pool_workqueue_release                                                                                            
      4 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-rcu_g                                                                                                   
      5 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-rcu_p                                                                                                   
      6 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-slub_                                                                                                   
      7 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-netns                                                                                                   
      9 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/0:0H-events_highpri                                                                                       
     12 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-mm_pe                                                                                                   
     13 root      20   0       0      0      0 I   0,0   0,0   0:00.00 rcu_tasks_kthread                                                                                                 
     14 root      20   0       0      0      0 I   0,0   0,0   0:00.00 rcu_tasks_rude_kthread                                                                                            
     15 root      20   0       0      0      0 I   0,0   0,0   0:00.00 rcu_tasks_trace_kthread                                                                                           
     16 root      20   0       0      0      0 S   0,0   0,0   0:00.02 ksoftirqd/0                                                                                                       
     17 root      20   0       0      0      0 I   0,0   0,0   0:01.55 rcu_preempt                                                                                                       
     18 root      rt   0       0      0      0 S   0,0   0,0   0:00.00 migration/0                                                                                                       
     19 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/0                                                                                                     
     20 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/0                                                                                                           
     21 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/1                                                                                                           
     22 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/1 
```
Y pues como todos unos Ing en sistemas identificamos procesos para matar a ojo, y clasificandolos separando los de procesos del sistema identificamos estos procesos y tambien el de vsCode porque esto se esta haciendo en VsCode seria pegarse un tiro en el pie matar el proceso.
Con los procesos identificados pues los matamos con el comando `kill`


```bash
    PID USUARIO   PR  NI    VIRT    RES    SHR S  %CPU  %MEM     HORA+ ORDEN 
   6326 mutable+  20   0  852272  54652  43188 S   7,9   0,3   0:01.57 gnome-terminal-text                                                                                               
   5278 mutable+  20   0 4596228 291488 188600 S   0,7   1,8   0:04.34 spotify                                                                                                           
   5006 mutable+  20   0 1156,1g 183656 120888 S   1,3   1,1   0:13.67 msedge                                                                                                            
   3581 mutable+  20   0   32,9g 400284 260256 S   0,3   2,5   1:22.35 msedge                                                                                                            
   3631 mutable+  20   0   32,5g 111584  84680 S   0,3   0,7   0:16.80 msedge                                                                                                            
   5702 mutable+  20   0   32,6g  90192  62484 S   0,3   0,6   0:03.99 whatsapp-linux-                                                                                                   
   5723 mutable+  20   0   32,4g  74480  63472 S   0,3   0,5   0:01.24 whatsapp-linux-                                                                                                   
   5778 mutable+  20   0 1134,2g 205964 125628 S   0,3   1,3   0:22.26 whatsapp-linux-                                                                                                   

```
de aqui mataremos a por ejemplo la aplicacion de whatsapp, para ello usamos kill con su PID
```bash
mutablename96@mutablename96-Nitro-AN515-54:~$ kill 5702
mutablename96@mutablename96-Nitro-AN515-54:~$ 

```

y analizando nuevamente con top... vemos que aun sigue ahi whatsapp, bicho malo nunca muere pero la explicacion de esta puede estar en que necesitamos matar todos los procesos relacionados con whatsapp-linux muchas aplicaciones dividen su funcionamiento en múltiples procesos, y matar solo uno puede no ser suficiente.

```bash
mutablename96@mutablename96-Nitro-AN515-54:~$ top

top - 13:27:48 up 29 min,  1 user,  load average: 0,49, 1,11, 1,17
Tareas: 355 total,   1 ejecutar,  354 hibernar,    0 detener,    0 zombie
%Cpu(s):  1,6 us,  0,8 sy,  0,0 ni, 97,6 id,  0,0 wa,  0,0 hi,  0,0 si,  0,0 st 
MiB Mem :  15832,5 total,   7810,7 libre,   4564,9 usado,   4458,4 búf/caché     
MiB Intercambio:   4096,0 total,   4096,0 libre,      0,0 usado.  11267,6 dispon Mem 

    PID USUARIO   PR  NI    VIRT    RES    SHR S  %CPU  %MEM     HORA+ ORDEN                                                                                                             
    911 avahi     20   0   14848   9856   3840 S   6,3   0,1   6:25.25 avahi-daemon                                                                                                      
   7177 mutable+  20   0   32,6g  86552  61824 S   5,0   0,5   0:00.49 whatsapp-linux-                                                                                                   
   2229 mutable+  20   0   25,0g 176028 118336 S   4,3   1,1   1:33.33 Xorg                                                                                                              
   2497 mutable+  20   0 4676984 306932 135808 S   4,0   1,9   1:51.40 gnome-shell                                                                                                       
   6326 mutable+  20   0  854764  56956  43188 S   3,0   0,4   0:19.27 gnome-terminal-                                                                                                   
    275 root     -51   0       0      0      0 S   1,7   0,0   0:16.72 irq/136-SYNA7DB5:01                                                                                               
   6549 mutable+  20   0 1157,8g 289700 133452 S   1,3   1,8   3:18.23 msedge                                                                                                            
   7223 mutable+  20   0   23424   6144   3840 R   1,0   0,0   0:00.47 top                                                                                                               
    967 root      20   0  345804  19184  16496 S   0,7   0,1   0:29.19 NetworkManager                                                                                                    
   3631 mutable+  20   0   32,5g 111480  85012 S   0,7   0,7   0:39.67 msedge                                                                                                            
    628 root     -51   0       0      0      0 S   0,3   0,0   0:32.45 irq/146-iwlwifi                                                                                                   
    851 systemd+  20   0   17556   7424   6656 S   0,3   0,0   0:01.16 systemd-oomd                                                                                                      
   2412 mutable+  20   0    9608   4992   4608 S   0,3   0,0   0:00.33 dbus-daemon                                                                                                       
   3581 mutable+  20   0   32,9g 404588 261416 S   0,3   2,5   2:08.38 msedge                                                                                                            
   3694 mutable+  20   0 1157,7g 152264 105120 S   0,3   0,9   0:03.90 msedge                                                                                                            
   3745 root      20   0       0      0      0 I   0,3   0,0   0:05.39 kworker/1:2-mm_percpu_wq                                                                                          
   4775 mutable+  20   0 1157,7g 174468  79104 S   0,3   1,1   0:27.86 code                                                                                                              
   5582 mutable+  20   0 1132,2g 163408 122376 S   0,3   1,0   0:23.15 whatsapp-linux-                                                                                                   
   6505 root       0 -20       0      0      0 I   0,3   0,0   0:01.04 kworker/u25:0-rb_allocator                                                                                        
      1 root      20   0   23620  13720   8984 S   0,0   0,1   0:02.96 systemd                                                                                                           
      2 root      20   0       0      0      0 S   0,0   0,0   0:00.00 kthreadd                                                                                                          
      3 root      20   0       0      0      0 S   0,0   0,0   0:00.00 pool_workqueue_release                                                                                            
      4 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-rcu_g                                                                                                   
      5 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-rcu_p                                                                                                   
      6 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-slub_                                                                                                   
      7 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-netns                                                                                                   
      9 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/0:0H-events_highpri                                                                                       
     12 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-mm_pe                                                                                                   
     13 root      20   0       0      0      0 I   0,0   0,0   0:00.00 rcu_tasks_kthread                                                                                                 
     14 root      20   0       0      0      0 I   0,0   0,0   0:00.00 rcu_tasks_rude_kthread                                                                                            
     15 root      20   0       0      0      0 I   0,0   0,0   0:00.00 rcu_tasks_trace_kthread                                                                                           
     16 root      20   0       0      0      0 S   0,0   0,0   0:00.05 ksoftirqd/0                                                                                                       
     17 root      20   0       0      0      0 I   0,0   0,0   0:03.25 rcu_preempt                                                                                                       
     18 root      rt   0       0      0      0 S   0,0   0,0   0:00.01 migration/0                                                                                                       
     19 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/0                                                                                                     
     20 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/0                                                                                                           
     21 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/1                                                                                                           
     22 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/1  
```
Volvemos a hacer el kill con los PID relacionados con whatsapp y ahora porfin se cierra.
```bash
mutablename96@mutablename96-Nitro-AN515-54:~$ kill 7177 5582
mutablename96@mutablename96-Nitro-AN515-54:~$ top

top - 13:33:32 up 35 min,  1 user,  load average: 1,14, 1,19, 1,18
Tareas: 351 total,   2 ejecutar,  349 hibernar,    0 detener,    0 zombie
%Cpu(s):  1,7 us,  0,7 sy,  0,0 ni, 97,4 id,  0,1 wa,  0,0 hi,  0,1 si,  0,0 st 
MiB Mem :  15832,5 total,   7952,5 libre,   4423,4 usado,   4408,3 búf/caché     
MiB Intercambio:   4096,0 total,   4096,0 libre,      0,0 usado.  11409,1 dispon Mem 

    PID USUARIO   PR  NI    VIRT    RES    SHR S  %CPU  %MEM     HORA+ ORDEN                                                                                                             
    911 avahi     20   0   14848   9856   3840 S  13,7   0,1   7:44.20 avahi-daemon                                                                                                      
   2229 mutable+  20   0   25,0g 184124 118696 S   2,8   1,1   1:53.05 Xorg                                                                                                              
   6326 mutable+  20   0  855952  58364  43188 S   2,4   0,4   0:25.56 gnome-terminal-                                                                                                   
   2497 mutable+  20   0 4695252 332192 135824 S   1,6   2,0   2:13.36 gnome-shell                                                                                                       
   7506 mutable+  20   0   23424   6144   3840 R   1,6   0,0   0:00.09 top                                                                                                               
   3631 mutable+  20   0   32,5g 111408  85012 S   1,2   0,7   0:45.91 msedge                                                                                                            
    275 root     -51   0       0      0      0 R   0,8   0,0   0:20.22 irq/136-SYNA7DB5:01                                                                                               
    628 root     -51   0       0      0      0 S   0,8   0,0   0:37.74 irq/146-iwlwifi                                                                                                   
    967 root      20   0  345804  19184  16496 S   0,8   0,1   0:33.91 NetworkManager                                                                                                    
   2697 mutable+  20   0  397844  11924   7040 S   0,8   0,1   0:09.47 ibus-daemon                                                                                                       
   3581 mutable+  20   0   32,9g 408616 263660 S   0,8   2,5   2:18.38 msedge                                                                                                            
   3142 mutable+  20   0 3215564  62276  44100 S   0,4   0,4   0:03.85 gjs                                                                                                               
   4775 mutable+  20   0 1157,7g 176828  79104 S   0,4   1,1   0:36.75 code                                                                                                              
   6549 mutable+  20   0 1157,8g 297668 133612 S   0,4   1,8   3:48.13 msedge                                                                                                            
      1 root      20   0   23620  13720   8984 S   0,0   0,1   0:03.02 systemd                                                                                                           
      2 root      20   0       0      0      0 S   0,0   0,0   0:00.00 kthreadd                                                                                                          
      3 root      20   0       0      0      0 S   0,0   0,0   0:00.00 pool_workqueue_release                                                                                            
      4 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-rcu_g                                                                                                   
      5 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-rcu_p                                                                                                   
      6 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-slub_                                                                                                   
      7 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-netns                                                                                                   
      9 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/0:0H-events_highpri                                                                                       
     12 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/R-mm_pe                                                                                                   
     13 root      20   0       0      0      0 I   0,0   0,0   0:00.00 rcu_tasks_kthread                                                                                                 
     14 root      20   0       0      0      0 I   0,0   0,0   0:00.00 rcu_tasks_rude_kthread                                                                                            
     15 root      20   0       0      0      0 I   0,0   0,0   0:00.00 rcu_tasks_trace_kthread                                                                                           
     16 root      20   0       0      0      0 S   0,0   0,0   0:00.05 ksoftirqd/0                                                                                                       
     17 root      20   0       0      0      0 I   0,0   0,0   0:03.72 rcu_preempt                                                                                                       
     18 root      rt   0       0      0      0 S   0,0   0,0   0:00.01 migration/0                                                                                                       
     19 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/0                                                                                                     
     20 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/0                                                                                                           
     21 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/1                                                                                                           
     22 root     -51   0       0      0      0 S   0,0   0,0   0:00.00 idle_inject/1                                                                                                     
     23 root      rt   0       0      0      0 S   0,0   0,0   0:00.13 migration/1                                                                                                       
     24 root      20   0       0      0      0 S   0,0   0,0   0:04.67 ksoftirqd/1                                                                                                       
     25 root      20   0       0      0      0 I   0,0   0,0   0:00.00 kworker/1:0-inet_frag_wq                                                                                          
     26 root       0 -20       0      0      0 I   0,0   0,0   0:00.00 kworker/1:0H-events_highpri                                                                                       
     27 root      20   0       0      0      0 S   0,0   0,0   0:00.00 cpuhp/2  
```