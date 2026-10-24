# manabi-life-assets（非公開）

「まなびライフ」の公開リポジトリ（nochi-jpg/manabi-life）に置けない素材。

| フォルダ | 中身 | ライセンス |
|---|---|---|
| `sounds/bgm/` | BGM 7曲（title / baby / school / work / retire / result / history） | MusMus（素材そのものの再配布は禁止） |
| `sounds/se/` | 効果音 8種（click / decide / up / cheer / shock / chime / crash / heartbeat） | 効果音ラボ（素材そのものの再配布は禁止） |

どの音をどこで使うかは、公開側の `data/audio.json` に書いてある。

## 使い方
公開側と同じ階層に clone して、公開側に `sounds` のシンボリックリンクを張る（公開側の `.gitignore` に `sounds/` が入っているので、公開リポジトリには上がらない）。

```
git clone https://github.com/nochi-jpg/manabi-life.git
git clone https://github.com/nochi-jpg/manabi-life-assets.git
cd manabi-life && ln -s ../manabi-life-assets/sounds sounds
```

最後の単一HTMLには、ここの音を（BGMは軽く圧縮しなおして）埋め込む。
