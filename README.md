![header](https://capsule-render.vercel.app/api?type=waving&color=0,0aa6b8,ff2fd0&height=140&section=header)

```cpp
#pragma once
#include <array>
#include <string_view>

// 아직 만족할 게임이 없어서, 직접 만들기로 했습니다.

class Developer {
public:
    static constexpr std::string_view Name  = "최범수";
    static constexpr std::string_view Email = "qjaqjaqja1877@gmail.com";
    static constexpr std::string_view Goal  = "Game Client Developer";

    enum class Proficiency : uint8_t { Learning, Familiar, Proficient };

    struct Skill {
        std::string_view Name;
        Proficiency      Level;
    };

    static constexpr std::array TechStack = {
        Skill{ "C++20",         Proficiency::Proficient },
        Skill{ "Unreal Engine", Proficiency::Proficient },
        Skill{ "DirectX 12",    Proficiency::Learning   },
        Skill{ "C#",            Proficiency::Familiar   },
    };

    static constexpr bool bBlueprintEnabled = false;  // and proud of it
};
```

<br>

![C++](https://img.shields.io/badge/C%2B%2B-20-ff2fd0?style=flat-square&logo=cplusplus)
![Unreal Engine](https://img.shields.io/badge/Unreal%20Engine-5.8-0aa6b8?style=flat-square&logo=unrealengine)
![DirectX](https://img.shields.io/badge/DirectX-12-0078d4?style=flat-square)
![Unity](https://img.shields.io/badge/Unity-100000?style=flat-square&logo=unity&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## 지금 하고 있는 것

- Unreal Engine 5 C++ — 게임 루프·상태머신·물리 시스템 직접 구현
- DirectX 12 렌더링 파이프라인 학습 중
- GCC사관학교 3기 수강 중

---

## 교육

**GCC사관학교 3기** — 언리얼엔진 기반 게임콘텐츠 제작과정 `2026.04 ~ 2026.10` `수강 중`
> 문화체육관광부 · 광주광역시 · 광주정보문화산업진흥원 주관

Unreal Engine 5 기반 게임 개발 전과정을 다루는 실무 중심 부트캠프. C++ 프로그래밍 기초부터 게임 AI, 멀티플레이어 네트워크, 팀 프로젝트를 통한 기획~빌드 패키징까지 게임 개발 전 사이클을 경험하는 과정.

---

## 주요 프로젝트

### 🎮 NEON DRIFT
> 중력 없는 호버바이크로 자원을 채집하고, 포탑에 탑승해 4방향 적을 막는 아케이드 웨이브 디펜스

`Unreal Engine 5.8` `C++20` `Blueprint 0%` `3일 스프린트`

- 전체 게임 로직을 순수 C++로 구현 — `.uasset` 파일 없이 Enhanced Input·HUD를 런타임 생성
- 구현 전 7단계 상태머신 설계 문서 확정 → 3일 내내 아키텍처 수정 0회
- IDamageable 인터페이스로 피격 대상 4종을 단일 캐스트 처리

[소스 코드](https://github.com/iamfreakin/NEON-DRIFT) · [랜딩 페이지](https://iamfreakin.github.io/NEON-DRIFT/) · [실행 파일](https://drive.google.com/file/d/1C71W51GIf9KWpUrPd3QW4Mcj6TCb8lJ-/view?usp=sharing)

![footer](https://capsule-render.vercel.app/api?type=waving&color=0,ff2fd0,0aa6b8&height=100&section=footer)
