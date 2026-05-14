# 실전 타로 상담 ✦ TOP 3%

---

## 🚀 GitHub + Vercel 배포 (파일을 루트에 직접 업로드)

### 1단계 — GitHub 저장소 만들기
1. github.com 로그인
2. 우측 상단 **`+`** → **New repository**
3. Repository name: **`tarot-counselor`**
4. **Public** 선택 → **Create repository**

### 2단계 — 파일 직접 업로드 (폴더 없이!)
1. 저장소 화면에서 **`uploading an existing file`** 클릭
2. ZIP 압축 해제 후 **안에 있는 파일과 폴더들을** 선택해서 드래그
   ```
   ✅ 이렇게 올라가야 함 (저장소 루트에 바로):
   tarot-counselor/           ← GitHub 저장소
   ├── pages/
   │   ├── index.js
   │   ├── _app.js
   │   └── api/
   │       └── tarot.js
   ├── styles/
   │   └── globals.css
   ├── package.json
   ├── next.config.js
   ├── vercel.json
   └── .gitignore
   ```
3. **Commit changes** 클릭

### 3단계 — Vercel Import
1. vercel.com → GitHub 로그인
2. **Add New Project** → `tarot-counselor` 선택 → **Import**
3. Root Directory: 비워두거나 **`.`** 입력 (기본값 그대로)

### 4단계 — API 키 환경변수 ⭐
```
Name:  ANTHROPIC_API_KEY
Value: sk-ant-api03-...
```
→ **Add** 클릭

### 5단계 — Deploy!
→ `https://tarot-counselor-xxx.vercel.app` 🎉

---

## 📁 저장소 구조
```
tarot-counselor/     ← GitHub 저장소 루트 = 파일들이 바로 여기
├── pages/
│   ├── index.js     ← 실전 타로 상담 앱 (TOP 3%)
│   ├── _app.js
│   └── api/
│       └── tarot.js ← Anthropic API 프록시 (CORS 해결)
├── styles/
│   └── globals.css
├── package.json
├── next.config.js
├── vercel.json
└── .gitignore
```
