# phro

thatshoon의 Claude Code 플러그인 마켓플레이스입니다. 각 플러그인은 자기 저장소에 있고, 이 저장소는 목록만 관리합니다.

## 설치

```bash
claude plugin marketplace add ThatsHoon/phro
claude plugin install <플러그인 이름>@phro
```

새 플러그인이 추가되면 `claude plugin marketplace update phro`로 목록을 갱신합니다.

## 플러그인

| 플러그인 | 설명 | 설치 |
|---|---|---|
| [phro-interactive-demo](https://github.com/ThatsHoon/phro-interactive-demo) | 앱 기획서(기능·플로우·상태 규칙)를 발표용으로 동작하는 데모 시뮬레이터로 만듭니다. | `claude plugin install phro-interactive-demo@phro` |
| [phro-prompt-nudge](https://github.com/ThatsHoon/phro-prompt-nudge) | 입력과 대화 맥락을 관찰해 더 나은 다음 질문·프롬프트를 입력창 위에 제안합니다. | `claude plugin install phro-prompt-nudge@phro` |
| [phro-term-board](https://github.com/ThatsHoon/phro-pm-terms) | Claude 답변에서 AI·IT 전반의 용어·개념·기술을 뽑아 용어 보드로 모으고, 체크하면 보관함으로 옮깁니다. (옛 이름 phro-pm-terms) | `claude plugin install phro-term-board@phro` |
| [phro-trend](https://github.com/ThatsHoon/phro-trend) | Hugging Face 트렌딩 AI 논문 3편을 기존 방식, 문제, 개선, 활용 구조, 예시, 다이어그램을 담은 한국어 실무 설명자료로 만듭니다. | `claude plugin install phro-trend@phro` |

## 플러그인 추가하기

`.claude-plugin/marketplace.json`의 `plugins`에 항목을 하나 더합니다. 플러그인 저장소에는 `.claude-plugin/plugin.json`만 있으면 됩니다. `github` 소스는 SSH로 복제해서 SSH 키가 없는 사용자는 설치에 실패하므로 HTTPS `url` 소스를 씁니다.

```json
{
  "name": "phro-새-플러그인",
  "description": "한 줄 설명",
  "source": { "source": "url", "url": "https://github.com/ThatsHoon/새-플러그인-저장소.git" }
}
```

## 라이선스

목록 파일은 [MIT](LICENSE). 각 플러그인의 라이선스는 해당 저장소를 따릅니다.
