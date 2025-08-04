# python-linux-windows
---

## Test - wydajność Python'a w Windows 10 vs Linux Ubuntu 24.04 LTS
=======


![logo](linux-vs-windows.jpg)

To subiektywny test mojego autorstwa, wykorzystuje Python i biblitekę numpy. Wykonuje 10 000 iteracji obliczeń, za każdą iteracją tworzy plik danych, zapisuje go na dysku, a następnie generuje obrazek i również zapisuje go na dysku.

---

## Wyniki testowe dla komputera:


### Linux - Kubuntu 24.04 LTS:

```
{
  "Aplikacja": "Program testowy",
  "Autor": "Adam Jurkiewicz",
  "sys.version": " linux -> 3.12.3 (main, Feb  4 2025, 14:48:35) [GCC 13.3.0] | hexversion 51119088 | api 1013",
  "sys.version_info": "sys.version_info(major=3, minor=12, micro=3, releaselevel='final', serial=0)",
  "os.uname": "posix.uname_result(sysname='Linux', nodename='linux', release='6.11.0-26-generic', version='#26~24.04.1-Ubuntu SMP PREEMPT_DYNAMIC Thu Apr 17 19:20:47 UTC 2', machine='x86_64')",
  "Start": "2025-06-15 12:45:17.843542",
  "Stop": "2025-06-15 13:12:03.721535",
  "Delta_time": "0:26:45.877993",
  "Czasy co 1000 enumeracji": {
    "0": "0:00:00.000277",
    "1000": "0:02:45.552031",
    "2000": "0:05:26.502691",
    "3000": "0:08:06.684872",
    "4000": "0:10:46.613255",
    "5000": "0:13:26.327691",
    "6000": "0:16:06.305770",
    "7000": "0:18:46.443818",
    "8000": "0:21:26.036031",
    "9000": "0:24:05.697044",
    "10000": "0:26:45.398852"
  }
}
```

### Windows:

```
{
  "Aplikacja": "Program testowy",
  "Autor": "Adam Jurkiewicz",
  "sys.version": " win32 -> 3.12.3 (tags/v3.12.3:f6650f9, Apr  9 2024, 14:05:25) [MSC v.1938 64 bit (AMD64)] | hexversion 51119088 | api 1013",
  "sys.version_info": "sys.version_info(major=3, minor=12, micro=3, releaselevel='final', serial=0)",
  "os.uname": "",
  "Start": "2025-08-04 14:27:10.612784",
  "Stop": "2025-08-04 15:07:03.290102",
  "Delta_time": "0:39:52.677318",
  "Czasy co 1000 enumeracji": {
    "0": "0:00:00.015619",
    "1000": "0:03:58.350859",
    "2000": "0:07:58.457796",
    "3000": "0:11:57.860209",
    "4000": "0:15:53.594582",
    "5000": "0:19:51.242922",
    "6000": "0:23:52.493432",
    "7000": "0:27:50.030732",
    "8000": "0:31:56.766755",
    "9000": "0:35:55.044221",
    "10000": "0:39:51.937696"
  }
}
```

## A więc ostateczny wynik:

- W systemie Linux Ubuntu 24.04 LTS: `"Delta_time": "0:26:45.877993"`
- W systemie Windows 10: ` "Delta_time": "0:39:52.677318"`

### System Linux jest ok. 35% szybszy niż Windows w typowych zadaniach języka Python na komputerze testowym.
