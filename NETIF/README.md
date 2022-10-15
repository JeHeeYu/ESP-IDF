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
