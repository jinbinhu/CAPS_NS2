# Description: 
  
These are simple implementations of CAPS and CAPS-dark on ns-2.35.  
  
# Usage:
  
### 1. Place the patch file 
All the patch files ('CAPS.patch' and 'CAPS-dark.patch') should be patched on the original ns-2.35.  
Please put the patch files outside the 'ns-2.35' folder, but inside the 'ns-allinone-2.35' folder.   
  
### 2. Patching
Type  'patch -p5 < CAPS.patch' for CAPS;  
      'patch -p5 < CAPS-dark.patch' for CAPS-dark.  
  
### 3. The following listed files will be changed successfully if the previous operations are done properly.  
  
patching file ns-2.35/classifier/classifier-mpath.cc  
patching file ns-2.35/classifier/hjbextra.h  
patching file ns-2.35/tcl/lib/ns-default.tcl  
patching file ns-2.35/tcp/tcp.h  
patching file ns-2.35/tcp/tcp.cc  
patching file ns-2.35/tcp/tcp-sink.h  
patching file ns-2.35/tcp/tcp-sink.cc  
patching file ns-2.35/common/agent.cc  
patching file ns-2.35/common/agent.h  
patching file ns-2.35/queue/mydrop-tail.h  
patching file ns-2.35/queue/mydrop-tail.cc  
patching file ns-2.35/Makefile  

### 4. Compile the codes:  
	cd ns-2.35  
	make  
  
### 5. Now you can run the simple testcases in ns-2.35 directory.  
	./ns many-to-many.tcl  
	./ns many-to-one.tcl  
  
If you have any questions, please email to jinbinhu@csu.edu.cn.  
