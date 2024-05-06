![image](https://github.com/helenalee01/iotanomalyclassification/assets/102953075/fc0c8cab-06bb-4509-9541-3a6a0ef5160a)## iotanomalyclassification 
- IoT network traffic attack classification improvement of DL(ResNet 1D)
- Dataset: IoTID20(IOT NETWORK INTRUSION DATASET)
- Source: https://ieee-dataport.org/open-access/iot-network-intrusion-dataset (Free membership/download)
- Features description
  feature Name	feature information
Flow_ID	Flow_ID
Src_IP	source IP
Src_Port	source port
Dst_IP	destination IP
Dst_Port	destination Port
Protocol	Flow protocol
Timestamp	발생 시간
Flow_Duration	Flow duration
Tot_Fwd_Pkts	전체 순방향 패킷
Tot_Bwd_Pkts	전체 역방향 패킷
TotLen_Fwd_Pkts	전체 순방향 패킷 길이
TotLen_Bwd_Pkts	전체 역방향 패킷 길이
Fwd_Pkt_Len_Max	패킷 최대 크기 (순방향)
Fwd_Pkt_Len_Min	패킷 최소 크기 (순방향)
Fwd_Pkt_Len_Mean	패킷 평균 크기 (순방향)
Fwd_Pkt_Len_Std	패킷 크기의 표준편차 (순방향)
Bwd_Pkt_Len_Max	패킷 최대 크기 (역방향)
Bwd_Pkt_Len_Min	패킷 최소 크기 (역방향)
Bwd_Pkt_Len_Mean	패킷 평균 크기 (역방향)
Bwd_Pkt_Len_Std	패킷 크기의 표준편차 (역방향)
Flow_Byts/s	초당 byte의 수
Flow_Pkts/s	초당 패킷의 수
Flow_IAT_Mean	2개의 패킷 사이에 걸린 시간의 평균
Flow_IAT_Std	2개의 패킷 사이에 걸린 시간의 표준편차
Flow_IAT_Max	2개의 패킷 사이에 걸린 시간의 최댓값
Flow_IAT_Min	2개의 패킷 사이에 걸린 시간의 최솟값
Fwd_IAT_Tot	2개의 패킷 사이에 걸린 시간 (순방향)
Fwd_IAT_Mean	2개의 패킷 사이에 걸린 시간의 평균 (순방향)
Fwd_IAT_Std	2개의 패킷 사이에 걸린 시간의 표준편차 (순방향)
Fwd_IAT_Max	2개의 패킷 사이에 걸린 시간의 최댓값 (순방향)
Fwd_IAT_Min	2개의 패킷 사이에 걸린 시간의 최솟값 (순방향)
Bwd_IAT_Tot	2개의 패킷 사이에 걸린 시간 (역방향)
Bwd_IAT_Mean	2개의 패킷 사이에 걸린 시간의 평균 (역방향)
Bwd_IAT_Std	2개의 패킷 사이에 걸린 시간의 표준편차 (역방향)
Bwd_IAT_Max	2개의 패킷 사이에 걸린 시간의 최댓값 (역방향)
Bwd_IAT_Min	2개의 패킷 사이에 걸린 시간의 최솟값 (역방향)
Fwd_PSH_Flags	Push Flag 수 (순방향)
Bwd_PSH_Flags	Push Flag 수 (역방향)
Fwd_URG_Flags	Urgent Flag 수 (순방향)
Bwd_URG_Flags	Urgent Flag 수 (역방향)
Fwd_Header_Len	header에 사용 된 전체 byte 수 (순방향)
Bwd_Header_Len	header에 사용 된 전체 byte 수 (역방향)
Fwd_Pkts/s	초당 패킷의 수 (순방향)
Bwd_Pkts/s	초당 패킷의 수 (역방향)
Pkt_Len_Min	최소 패킷 크기
Pkt_Len_Max	최대 패킷 크기
Pkt_Len_Mean	평균 패킷 크기
Pkt_Len_Std	패킷 크기 표준편차
Pkt_Len_Var	패킷 크기 분산
FIN_Flag_Cnt	패킷의 수 (FIN flag)
SYN_Flag_Cnt	패킷의 수 (SYN_Flag)
RST_Flag_Cnt	패킷의 수 (RST_Flag)
PSH_Flag_Cnt	패킷의 수 (PSH_Flag)
ACK_Flag_Cnt	패킷의 수 (ACK_Flag)
URG_Flag_Cnt	패킷의 수 (URG_Flag)
CWE_Flag_Cnt	패킷의 수 (CWE_Flag)
ECE_Flag_Cnt	패킷의 수 (ECE_Flag)
Down/Up_Ratio	Download and upload ratio
Pkt_Size_Avg	패킷 평균 크기
Fwd_Seg_Size_Avg	Average. size observed in fwd.
Bwd_Seg_Size_Avg	Average. size observed in bwd
Fwd_Byts/b_Avg	Average number. of bytes bulk rate in fwd.
Fwd_Pkts/b_Avg	Average number. of pkts. bulk rate in fwd.
Fwd_Blk_Rate_Avg	Average number. bulk rate in fwd
Bwd_Byts/b_Avg	Average number. of bytes bulk rate in bwd
Bwd_Pkts/b_Avg	Average number. of pkts. bulk rate in bwd
Bwd_Blk_Rate_Avg	Average. bulk rate in the bwd
Subflow_Fwd_Pkts	Average number. of pkts. in a subflow in fwd
Subflow_Fwd_Byts	Average number. of bytes in a subflow in fwd.
Subflow_Bwd_Pkts	Average number. of pkts. in a subflow in bwd
Subflow_Bwd_Byts	Average number. of bytes in a subflow in bwd
Init_Fwd_Win_Byts	Number. of bytes sent in initial window in fwd
Init_Bwd_Win_Byts	Number. of bytes sent in initial window in bwd
Fwd_Act_Data_Pkts	Count of pkts. with at least 1 byte of TCP data payload in the fwd.
Fwd_Seg_Size_Min	Min. segment size observed in fwd
Active_Mean	Mean time flow was active before idle
Active_Std	standard deviation of time flow was active before idle
Active_Max	Max. time flow was active before idle
Active_Min	Min. time flow was active before idle
Idle_Mean	Mean time flow was idle before active
Idle_Std	standard deviation of time flow was idle before active
Idle_Max	Max. time flow was idle before active
Idle_Min	Mix. time flow was idle before active
Label	공격 여부 (normal, anomaly)
Cat	공격 유형 (normal, Dos, Scan, Mirai, MITM ARP Spoofing)
Sub_Cat	세부 공격 유형 (normal, DoS-Synflooding, Scan Port OS, Scan Hostport, Mirai-Ackflooding, Mirai-Hostbruteforceg, Mirai-HTTP Flooding, Mirai-UDP Flooding, MITM ARP Spoofing)
![image](https://github.com/helenalee01/iotanomalyclassification/assets/102953075/5971d6f4-05fb-4daf-ae1d-def40ac670b5)


## Coming soon! feature generation code with training/testing sampels based on IoTID20

