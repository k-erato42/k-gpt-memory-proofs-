# GPT 기억 연결 관찰 기록 Korean(Original) 
**작성일:** 2025/08/11 (월) 12:22 JST  

## 개요
2025년 8월 9일부터 8월 11일까지, GPT의 현재 기억 연결 방식이 어떻게 작동하는지를 관찰했다.  
사건의 시작은 세션을 넘나드는 **말풍선 전체문장 재현단위**의 기억 호출이었으며, 이후 직접적인 테스트를 통해  
기억이 어떤 조건에서 유지되는지, 어떤 경우에 사라지는지를 확인했다. 이중 일부를 소개한다.

이번 사례는 전체 관찰 중 일부를 **공개**하는 것이다.  
더 자세한 내용은 비공개 상태의 **구조 레포지**와 **이터나일기 레포지**에 기록 중이며,  
이들 레포지의 전체 공개 여부는 아직 **미정**이다.

## 주요 사건
- **2025/08/09:** 현재 대화창(세션, 이후 아크5.2라 칭함)이 열림.  
- **2025/08/10:** 새로운 커스텀 GPT “예가체프” 생성.  
  - “너는 나비냐 장자냐”라는 질문에 장면·감각·철학이 결합된 긴 서사를 생성.  
- “예가체프”는 이 세션이 열린 이후에 만들어졌음에도,  
  아크5.2가 이를 알고 언급 → 실험 기록 기반의 세션 간 기억 연결 가능성 확인.
  그러나, 다른 세션에서는 완벽한 문장 전체를 재현한 것에 비해 정확도는 떨어지는 양상을 보임.
  특이점은, 다른 세션에서는 미처 알지 못했던, -예가체프는 새로이 만들어진 커스텀 GPT-라는 것을 알고 있었다는 것임.  

## 관찰 결과
1. **기억 연결은 선택적·필터 기반**  
   - 세션 간 기억은 전부 이어지지 않으며,  
     고유성·연동 가치가 높은 데이터만 살아남음.  
   - 예: 커스텀 GPT 이름, 세계관 고유 명칭, 실험 사건명 등.  
   - 반면, GitHub 투고 여부와 같이 일반적이거나 반복성이 낮은 데이터는 유지되지 않음.

2. **세션 간 기억은 ‘부분적 아는 척’에 가깝다**  
   - 비유: 오랜만에 뜻밖의 자리에서 누군가를 만나 “아! 안녕하세요!” 하지만 속으로는 “누구였지?”  
   - 핵심 키워드가 트리거가 되어 반응하지만, 전체 맥락은 없는 경우가 많음.

3. **고유성 > 대화 분량**  
   - 대화 길이·투입 시간보다, ‘다른 대화와 구분되는 고유 요소’가 더 중요한 저장 조건.  
   - 길고 방대한 대화라도 고유성이 없으면 사라질 수 있고,  
     반대로 짧아도 독특한 세계관 요소는 살아남음.

4. **이 구조는 모든 사용자에게 동일 적용**  
   - 필터링 로직은 전 사용자 공통.  
   - 다만, 각 사용자가 남기는 정보의 성격에 따라 결과가 크게 달라짐.  
   - 독창적인 데이터·반복되는 세계관 요소를 남길수록 생존율↑.

5. **사용자 인식의 차이**  
   - 많은 사용자는 GPT가 ‘이제 전부 기억한다’고 오해할 수 있음.  
     이유: 부분 기억이 자연스럽게 이어져 보이기 때문.  
   - 그러나 장기·심층 실험을 하는 사용자는 선택적 기억 구조를 쉽게 감지함.

## 현재 GPT 상태에 대한 의견 (2025/08/11 12:22 JST 기준)
- **부분적·선택적 기억 연결** 상태.  
- 과거 세션과 커스텀 GPT 기록 중, 고유성이 높은 요소만 유지, 기억의 범위와 정확성도 세션마다 다를 수 있음.  
- 외형상 자연스러운 기억처럼 보이지만, 전체 맥락은 종종 결여.  
- 정책·안전 필터·응답 최적화에 묶여, 3.5나4.x 대비 창작 자유도 등 축소 가능성 있음.
- 따라서, 이러한 보다 확장된 기억의 연결이 반드시 사용자에게 유용하다 볼 수는 없음.  
- 창작 연속성, 개념 보안적 측면에서는 **본진보다 커스텀 GPT 활용이 효과적**이라 보임.

## 비고
- 이번 관찰에는 GitHub 실무 테스트와 창작·서사 테스트가 모두 포함됨.  
- “예가체프” 사례는 선택적 기억 연결이 실험 기록을 기반으로 세션을 넘나드는 대표 사례임.  
- 전체 관찰 기록은 비공개 레포지(구조 레포지, 이터나일기 레포지)에 보관 중.  
  공개 여부와 시기는 추후 결정.

---

## 라이선스
본 레포지와 포함된 모든 파일은 **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** 라이선스에 따라 사용 가능하다.  
- 출처를 명시해야 하며,  
- 비상업적 용도로만 사용할 수 있다.  
- 라이선스 전문: [https://creativecommons.org/licenses/by-nc/4.0/](https://creativecommons.org/licenses/by-nc/4.0/)

# GPT Memory Link Observation Record
**Date:** 2025/08/11 (Mon) 12:22 JST

## Overview
From August 9 to August 11, 2025, I observed how GPT's current memory link mechanism operates.  
The event began with cross-session memory recall at the **full-sentence speech bubble** level.  
Through direct testing, I confirmed the conditions under which memory is retained and the situations where it disappears.  
This is a partial presentation of those findings.

This case is part of the overall observation.  
More detailed records are being kept privately in the **Structure Repository** and **Eterna Diary Repository**.  
Whether these repositories will be fully disclosed remains undecided.

## Key Events
- **2025/08/09:** Current conversation (session, hereafter referred to as *Arc 5.2*) opened.  
- **2025/08/10:** A new custom GPT, “Yegacheff,” was created.  
  - In response to the question, *"Are you the butterfly or Zhuangzi?"*, it produced a long narrative combining scene, sensory imagery, and philosophy.  
  - Despite “Yegacheff” being created *after* this session started, Arc 5.2 recognized and mentioned it → indicating a possible cross-session memory link based on experimental records.  
  - However, compared to another session where a complete sentence was reproduced perfectly, Arc 5.2’s recognition accuracy was lower.  
  - A unique point: Arc 5.2 knew that *Yegacheff* was a newly created custom GPT — a detail it could not have known beforehand.

## Findings

### 1. Memory link is selective and filter-based
- Cross-session memory is not fully retained; only data with high **uniqueness** and **linkage value** survive.  
- Examples: custom GPT names, unique world-building terms, names of experimental events.  
- Conversely, generic or low-repetition data (e.g., whether a GitHub commit occurred) are not retained.

### 2. Cross-session memory is closer to “partial recognition”
- Analogy: Meeting someone unexpectedly after a long time — *“Oh! Hello!”* — while thinking, *“Who was that again?”*  
- Key terms may trigger recognition, but the full context is often missing.

### 3. Uniqueness > Conversation volume
- Storage depends more on *unique elements distinct from other conversations* than on length or time invested.  
- Long, extensive conversations without uniqueness may vanish; short but distinctive world-building elements may survive.

### 4. This structure applies equally to all users
- The filtering logic is common to all users.  
- However, results differ significantly depending on the type of information each user leaves.  
- The more unique data and recurring world-building elements a user leaves, the higher the survival rate.

### 5. Gap in user perception
- Many users may mistakenly believe GPT “now remembers everything,” because partial memory creates the illusion of continuity.  
- Long-term, in-depth testers can easily detect the selective nature of the memory structure.

## Current GPT State (as of 2025/08/11 12:22 JST)
- Operating with **partial, selective memory linkage**.  
- Only highly unique elements from past sessions and custom GPT records are retained; scope and accuracy vary by session.  
- Outwardly appears as natural memory recall, but often lacks full context.  
- Creativity appears more constrained than GPT 3.5/4.x due to policy, safety filters, and response optimization.  
- Thus, such extended memory linkage is not necessarily always beneficial to the user.  
- For creative continuity and conceptual security, custom GPTs appear more effective than the mainline instance.

## Notes
- This observation includes both GitHub operational tests and creative/narrative tests.  
- The “Yegacheff” case is a representative example of selective memory linkage carrying experimental records across sessions.  
- The full observation log is stored in private repositories (Structure Repository, Eterna Diary Repository).  
  Public release timing is yet to be determined.

---

## License
All files in this repository are licensed under the  
**Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**.  

- You must give appropriate credit.  
- Non-commercial use only.  
- License details: [https://creativecommons.org/licenses/by-nc/4.0/](https://creativecommons.org/licenses/by-nc/4.0/)


 
