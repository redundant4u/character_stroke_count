# character_stroke_count
한글, 영어 획순 계산 프로그램

# 기능
**process()**: 처음으로 실행되는 함수. `characterScan()`과 `characterStrokecount()` 함수를 실행함.

**characterScan(text)**: 문자 text를 `charCodeAt()` 함수로 유니코드로 변환 뒤 한글이 아닐 경우 `characterArr` 배열에 저장하고
한글일 경우 초성, 중성, 종성으로 나누어서 `characterArr` 배열에 저장한다.

**characterStrokecount(source)**: 문자 source를 정규식을 이용해서 한글, 소문자, 대문자로 구분하고 `funcOfstrokeCount`로 넘겨
획순을 계산한다.

**funcOfstrokeCount(alphabetArr, alphabetStrokeCountArr, alphabet)**: 문자 정보를 가지는 alphabetArr, 문자 획순를 가지고 있는 alphabet
StrokeCountArr, 문자인 alphabet를 인자로 받아 alphabet와 같은 alphabetArr에서 찾아서 alphabetStrokeCountArr을 통해 획순을 찾아 더한다.
