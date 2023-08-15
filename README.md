# netfilter

# 명령어 
gcc -o nfqnl_test nfqnl_test.c -lnetfilter_queue

sudo ./nfqnl_test

# 빌드 
"./nfqnl_test 0" 명령어를 실행하면 netfilter를 코드상에서 처리하여 IP packet이 ACCEPT이 되는 것을 확인할 수 있다. 

-> nfq_set_verdict 함수의 3번째 인자를 NF_ACCEPT 에서 NF_DROP으로 고치면 DROP과 똑같은 
결과가 나오는 것을 확인할 수가 있다. 


->nfq_set_verdict 함수를 3번째 인자에서 NF_ACCEPT 하거나 NF_DROP값으로 호출하면 
패킷을 accept하거나 DROP 할 수 있다 .
