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

## 플러그인 추가하기

`.claude-plugin/marketplace.json`의 `plugins`에 항목을 하나 더합니다. 플러그인 저장소에는 `.claude-plugin/plugin.json`만 있으면 됩니다.

```json
{
  "name": "phro-새-플러그인",
  "description": "한 줄 설명",
  "source": { "source": "github", "repo": "ThatsHoon/새-플러그인-저장소" }
}
```

## 라이선스

목록 파일은 [MIT](LICENSE). 각 플러그인의 라이선스는 해당 저장소를 따릅니다.
