# python-linux-windows
---

## Test - wydajność Python'a w Windows 10 vs Linux Ubuntu 24.04 LTS
=======


![logo](linux-vs-windows.jpg)

To subiektywny test mojego autorstwa, wykorzystuje Python i biblitekę numpy. Wykonuje 10 000 iteracji obliczeń, za każdą iteracją tworzy plik danych, zapisuje go na dysku, a następnie generuje obrazek i również zapisuje go na dysku.

---

## Wyniki testowe dla komputera:


### Linux:

```
{
"Aplikacja": "Program testowy",
"Autor": "Adam Jurkiewicz",
"sys.version": "3.12.3 (main, Feb  4 2025, 14:48:35) [GCC 13.3.0] | hexversion 51119088 | api 1013",
"sys.version_info": "sys.version_info(major=3, minor=12, micro=3, releaselevel='final', serial=0)",
"os.uname": "posix.uname_result(sysname='Linux', nodename='linux', release='6.11.0-26-generic', version='#26~24.04.1-Ubuntu SMP PREEMPT_DYNAMIC Thu Apr 17 19:20:47 UTC 2', machine='x86_64')",
"Start": "2025-06-04 22:30:20.926629",
"Stop": "2025-06-04 22:57:33.092588",
"Delta_time": "0:27:12.165959",
"Czasy co 1000 enumeracji": {
	"1000": "0:02:44.645194",
	"2000": "0:05:27.891284",
	"3000": "0:08:10.903851",
	"4000": "0:10:55.265239",
	"5000": "0:13:37.814131",
	"6000": "0:16:20.518295",
	"7000": "0:19:03.127240",
	"8000": "0:21:45.759054",
	"9000": "0:24:28.695765"
	}
}
```

### Windows:

```
{
"Aplikacja": "Program testowy",
"Autor": "Adam Jurkiewicz",
"sys.version": "3.12.3 (tags/v3.12.3:f6650f9, Apr  9 2024, 14:05:25) [MSC v.1938 64 bit (AMD64)] | hexversion 51119088 | api 1013", "sys.version_info": "sys.version_info(major=3, minor=12, micro=3, releaselevel='final', serial=0)",
"os.uname": "",
"Start": "2025-06-05 13:09:41.165480",
"Stop": "2025-06-05 13:47:47.665295",
"Delta_time": "0:38:06.499815",
"Czasy co 1000 enumeracji": {
	"1000": "0:03:48.065001",
	"2000": "0:07:36.802949",
	"3000": "0:11:28.030274",
	"4000": "0:15:16.301867",
	"5000": "0:19:05.023304",
	"6000": "0:22:53.138487",
	"7000": "0:26:43.257995",
	"8000": "0:30:30.771357",
	"9000": "0:34:18.057072"
	}
}
```

## A więc ostateczny wynik:

- W systemie Linux Ubuntu 24.04 LTS: `"Delta_time": "0:27:12.165959"`
- W systemie Windows 10: `"Delta_time": "0:38:06.499815"`

### System Linux jest ok. 40% szybszy niż Windows w typowych zadaniach języka Python na komputerze testowym.
