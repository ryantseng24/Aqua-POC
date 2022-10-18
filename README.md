# container_sec_lab。
一 映像檔 (Image) 掃描  
4. 掃描 Image 是否有惡意程式/挖擴程式/無檔案執行/系統提權腳本  
5. 掃描 Image 是否有存在明碼的敏感資訊，如private key  
二 容器運行 (Container Runtime) 威脅偵測與保護   
1.容器於運行時是否能偵測到容器跳脫 (container escape)  
2.容器於運行時是否能偵測run as root 及特權容器  
3.偵測惡意容器，如無檔案於記憶體執行程式，植入惡意程式，變更容器內系統設定檔案。  
4.偵測容器中跑非image 定義的執行程式或是連接惡意FQDN或是IP  
