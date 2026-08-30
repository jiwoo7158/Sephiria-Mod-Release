# Sephiria Mod Release Repository

이 저장소는 Sephiria Mod Manager가 읽는 공개 배포 저장소입니다.

## 저장소 루트

- `mods.json`: Mod Manager가 보여줄 모드 목록과 최신 버전 정보
- 소스코드를 올릴 필요는 없습니다.

## Release 예시

### Sephiria Trials 1.0.0

- Tag: `trials-v1.0.0`
- Asset: `SephiriaTrials.zip`

ZIP 내부:

```text
SephiriaTrials.zip
├─ SephiriaTrials.dll
└─ SephiriaTrials/
   └─ 이미지 파일들...
```

### Sephiria Inventory Sort 1.0.0

- Tag: `inventory-sort-v1.0.0`
- Asset: `SephiriaInventorySort.zip`

ZIP 내부:

```text
SephiriaInventorySort.zip
├─ SephiriaInventorySort.dll
└─ SephiriaInventorySort/
   └─ 이미지 파일들...
```

ZIP 안에 `BepInEx` 또는 `plugins` 폴더를 넣지 마세요.

## 업데이트 순서

1. 새 DLL과 이미지 폴더로 ZIP을 만듭니다.
2. GitHub에서 새 Release를 만들고 새 Tag를 지정합니다.
3. ZIP을 Release Asset으로 첨부하고 Release를 게시합니다.
4. **마지막으로** `mods.json`에서 해당 모드의 `version`과 `releaseTag`를 새 값으로 수정합니다.

`mods.json`을 마지막에 수정해야 사용자가 아직 존재하지 않는 Release를 다운로드하려는 시간을 피할 수 있습니다.
