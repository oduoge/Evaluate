- &

<code>&</code>的意思是在后台运行。
在命令后添加 <code>&</code> 后，即使按下<code>Ctrl C</code>，命令也会正常运行，即对SIGINT信号免疫，
但此时如果直接关掉<code>Shell</code>Shell，先前输入的命令进程也会消失，对<code>SIGUP</code>信号不免疫。

- nohup

<code>nohup</code>是忽略SIGHUP信号，所当在命令前面添加<code>nohup</code>时，关闭<code>Shell</code>后，命令进程仍然在运行(对SIGUP信号免疫）
但是，这时如果直接在shell中输入<code>Ctrl C</code>,那之前的命令进程就会消失，因为它对SIGINT信号免疫.

所以通常二者一些使用
