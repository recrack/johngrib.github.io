---
layout  : wiki
title   : date 명령어
summary : 날짜나 시간을 출력하거나 설정한다
date    : 2018-08-03 05:19:22 +0900
updated : 2019-12-07 13:29:45 +0900
tag     : bash command
toc     : true
public  : true
parent  : command-line
latex   : false
---
* TOC
{:toc}

## Examples
### BSD(macOS)

```sh
 # 현재 날짜, 시간
date

 # 현재 날짜, 시간 포매팅
date '+%Y-%m-%d %H:%M:%S %a %Z'

 # 오늘은 1년 중 몇 번째 주(week)인가?
date +%V

 # unix timestamp를 읽기 쉬운 날짜로 변환
date -r 1572511074
```

## Format

* 명령어 예제를 실행한 결과의 기준은 `2018년 8월 3일 금요일 05시 49분 37초`.

| 포맷 옵션 | 설명                 | 명령어 예제 | 실행 결과                |
|-----------|----------------------|-------------|--------------------------|
| `%`       | %                    | `date +%`   | `%`                      |
| `%n`      | `\n`                 | `date +%n`  | 공백 라인이 출력된다.    |
| `%t`      | `\t`                 | `date +%n`  | 탭 문자가 출력된다.      |
| `%s`      | epoch 타임           | `date +%s`  | `1533242977`             |
| `%Y`      | 4자리 년도           | `date +%Y`  | `2018`                   |
| `%y`      | 2자리 년도           | `date +%y`  | `18`                     |
| `%A`      | 요일 이름(locale)    | `date +%A`  | `금요일`                 |
| `%a`      | 요일 이름(locale)    | `date +%a`  | `금`                     |
| `%B`      | 월 이름(locale)      | `date +%B`  | `8월`                    |
| `%b`      | 월 이름(locale)      | `date +%b`  | `8`                      |
| `%m`      | 월(01 ~ 12)          | `date +%m`  | `08`                     |
| `%c`      | 날짜 및 시간(locale) | `date +%c`  | `금  8/ 3 05:49:37 2018` |
| `%d`      | Month 날짜(01 ~ 31)  | `date +%d`  | `03`                     |
| `%j`      | Year 날짜(001 ~ 366) | `date +%j`  | `215`                    |
| `%w`      | 요일 숫자(0: 일요일) | `date +%w`  | `5`                      |
| `%H`      | 시간(00 ~ 23)        | `date +%H`  | `05`                     |
| `%M`      | 분(00 ~ 59)          | `date +%M`  | `49`                     |
| `%S`      | 초(00 ~ 59)          | `date +%S`  | `37`                     |
| `%V`      | week 숫자            | `date +%V`  | `31`                     |
| `%Z`      | 타임존               | `date +%Z`  | `KST`                    |


