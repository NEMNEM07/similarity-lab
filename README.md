# 유사도 비교 실험

코사인 유사도, 자카드 유사도, 유클리드 거리 중 어느 방법이 수능 독서 지문의 정답 선지를 더 잘 찾는지 비교하는 인공지능 수학 탐구 페이지.

- 기출 지문과 선지 원문은 저작권 때문에 저장소에 넣지 않고, 계산한 수치만 담았다.
- 원문은 내 컴퓨터에서 `kice_extract.py`로 뽑아 브라우저 안에서만 본다.

## 원문이 보이는 내 컴퓨터용 페이지 만들기

기출 문제지 PDF(2024, 2025, 2026학년도)를 이 폴더에 두고 실행한다.

```
pip install pdfplumber
python kice_extract.py --dir . --page index.html --html-out similarity-lab-원문.html
```

만들어진 `similarity-lab-원문.html`을 열면 지문과 선지가 텍스트로 보인다. 이 파일과 `kice_items.json`에는 원문이 들어 있으므로 인터넷에 올리지 않는다. (`.gitignore`가 막아 준다.)
