sysex message received on any change of any parameter  
NB: some messages may be program changes, with bank selects, or other messages like cc messages  

onmidimessagereceived  
if Sysex ✔️  
if JDxi ✔️  
check part address 
check param address 

hex math add offsets ✔️ 
int_to_hex - variable padding (test) 

-- on init create index key per param part,and retain sysex bytes, to reduce unnecessary computation at runtime on update 

parse values  
enums  
parameter size lookup?


onmidisendsysexrequest  
  parse values 

on_init
  build Pam, integer value key per part?

eg analog temp tone
part [{19 42 00 00}

param.a
param.b

OR: CHECK PART (19 42)  
THEN: CHECK OFFSET (00 2D)


IF (PART AND OFFSET).>>> parameter_change

unregistered_controller event: offer mapping 

---

hidden controllers grid 
max_controls?
existing_mappings : ...  



### controller reset 
on press reset 
on long press reset no_send. 


get/set read and request value update per controller (sync) to update controller(s) with values from sysex messages 

- initially test send/receive/update controller values for multiple controls, re update time, latency,stack overflow issues 

-programchange bank select 
tone select 




