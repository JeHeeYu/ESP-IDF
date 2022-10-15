# ESP-IDF NETIF Reference 정리

## esp_err_t esp_netif_init(void)
<b>Header</b> : /esp_netif/include/esp_netif.h
<br>
<b>Parameter</b>
<br>
　　void
<br>
<b>Description</b> : 기본 TCP/IP 스택 메모리 초기화 함수로 Application 시작 시 한 번만 호출되어야 함
<br>
<b>Return</b>
<br>
　　ESP_OK : 성공
<br>
　　ESP_FAIL : 실패
<br>
<br>


## esp_err_t esp_netif_create_default_wifi_ap (void)
<b>Header</b> : /esp_netif/include/esp_netif.h
<br>
<b>Parameter</b>
<br>
　　void
<br>
<b>Description</b> : WiFi AP 생성. AP Mode에 대한 Initialize 및 Event Handler 등록. 이 핸들러를 생성해야 AP Mode 동작 가능
<br>
<b>Return</b>
<br>
　　esp_netif Instance : AP Mode에 관한 포인터
<br>
<br>


## esp_err_t esp_netif_create_default_wifi_sta(void)
<b>Header</b> : /esp_netif/include/esp_netif.h
<br>
<b>Parameter</b>
<br>
　　void
<br>
<b>Description</b> : WiFi STA 생성. STA Mode에 대한 Initialize 및 Event Handler 등록. 이 핸들러를 생성해야 STA Mode 동작 가능
<br>
<b>Return</b>
<br>
　　esp_netif Instance : STA Mode에 관한 포인터
<br>
<br>
