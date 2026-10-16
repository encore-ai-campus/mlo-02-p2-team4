# Pandas 분석 입력 데이터

이 폴더의 `분석입력_CSV.zip`은 팀원이 제공한 **합성 데이터 기반 분석용 사본** 3개를 압축한 파일입니다.
원본 수신 데이터나 실제 KREAM 기업 데이터가 아닙니다. 팀의 공개 범위·동의를 확인한 뒤 GitHub에 올리세요.

## 로컬 실행 전 준비

1. `분석입력_CSV.zip`을 압축 해제합니다.
2. ZIP에 들어 있는 CSV **세 개를 이 폴더 바로 아래**에 둡니다. ZIP 이름의 하위 폴더 안에 두면 로더가 찾지 못합니다.
3. 예상 경로는 다음과 같습니다.

```text
analysis/pandas_presentation/데이터/
  clean_kream_inspection_joined.csv
  inspector_master.csv
  valid_workload_counts.csv
  출처_및_연결기록.json
```

| 입력 CSV | 역할 |
| --- | --- |
| `clean_kream_inspection_joined.csv` | 최종 유효 검수의 Pandas 분석용 결합 데이터 |
| `inspector_master.csv` | 정상 검수원 등록 인원·부서·직급 분석용 마스터 |
| `valid_workload_counts.csv` | 유효 최초·재검수 작업량의 부서별 요약 |

`출처_및_연결기록.json`의 테이블·행 수·해시 기록은 유지하고, 팀원 PC의 로컬 절대경로만 상대 식별 정보로 바꿨습니다. 제공된 Python 실행 코드는 변경하지 않았습니다.

입력 CSV는 GitHub 업로드 편의와 중복 적재 방지를 위해 압축 상태로 보관하며, **압축을 풀지 않은 상태에서는 Python 분석이 실행되지 않습니다.**
