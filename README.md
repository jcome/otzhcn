# otzhcn
 OpenToonz Chinese UI Translation

## Toolchain and workflow

### Grab TS files into OmegaT source dir
- colorfx.ts
- image.ts
- tnzcore.ts
- tnztools.ts
- toonz.ts
- toonzlib.ts
- toonzat.ts


### Convert TS to PO with lconvert (Qt)
```
lconvert colorfx.ts -o colorfx.po && lconvert image.ts -o image.po && lconvert tnzcore.ts -o tnzcore.po && lconvert tnztools.ts -o tnztools.po && lconvert toonz.ts -o toonz.po && lconvert toonzlib.ts -o toonzlib.po && lconvert toonzqt.ts -o toonzqt.po
```
### Translate with OmegaT
Version: OmegaT-4.3.3_0_924066809

### Convert PO back to TS with lconvert in OmegaT target dir
```
lconvert colorfx.po -o colorfx.ts && lconvert image.po -o image.ts && lconvert tnzcore.po -o tnzcore.ts && lconvert tnztools.po -o tnztools.ts && lconvert toonz.po -o toonz.ts && lconvert toonzlib.po -o toonzlib.ts && lconvert toonzqt.po -o toonzqt.ts
```

### Convert translated TS to QM (Optional)
```
lconvert colorfx.ts -o colorfx.qm && lconvert image.ts -o image.qm && lconvert tnzcore.ts -o tnzcore.qm && lconvert tnztools.ts -o tnztools.qm && lconvert toonz.ts -o toonz.qm && lconvert toonzlib.ts -o toonzlib.qm && lconvert toonzqt.ts -o toonzqt.qm
```

### Push final TS and QM files to OpenToonz official repo
github workflow

---

## 常规
### 标点符号的使用
- 直接暴露在界面的短语使用西文标点符号
- 提示语，警告报错等对话性完整语句用中文标点符号

## 常见词汇

### 坐标和方向
- X，Y，Z， H，V：横向，竖向，纵深

## 专业词汇
请查看 Glossary.txt


