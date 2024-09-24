# ESXI 6.0 and low RAM (MEMORY_SIZE ERROR)

When you get error MEMORY_SIZE ERROR, press ALT+F1 and fix upgrade_precheck.py, line MEM_MIN_SIZE.  
User root without password.	

steps:

cd /usr/lib/vmware/weasel/util	
rm upgrade_precheck.pyc		
mv upgrade_precheck.py upgrade_precheck.py.old	
cp upgrade_precheck.py.old upgrade_precheck.py		
chmod 666 upgrade_precheck.py		
vi upgrade_precheck.py 		
ps -c | grep weasel 	
kill -9 PID		
