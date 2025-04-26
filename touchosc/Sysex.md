sysex message received on any change of any parameter  
NB: some messages may be program changes, with bank selects, or other messages like cc messages  

onmidimessagereceived  
if Sysex ✔️  
if JDxi ✔️  
check part address 
check param address 

hex math add offsets ✔️ 
int_to_hex - variable padding (test)  

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



