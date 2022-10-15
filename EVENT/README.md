# ESP-IDF Event Loop API Reference 정리

## esp_err_t esp_event_loop_create_default(void)
<b>Header</b> : components/esp_event/include/esp_event.h
<br>
<b>Parameter</b>
<br>
　　void
<br>
<b>Description</b> : 기본 이벤트 루프 생성. 시스템 사용 전 이벤트 루프를 생성해야 이벤트가 동작할 수 있음
<br>
<b>Return</b>
<br>
　　ESP_OK : 성공
<br>
　　Other : 실패
<br>
<br>
