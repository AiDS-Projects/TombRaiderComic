# 场景资产表

Mode：cinematic-drama（剧情影像）
作品：第一集试片《龙三角的呼唤》

每个跨片段或调度重要的场景建立 16:9 静态参考图，锁定空间、材质、主辅色与基础光位。

## style 锁

半写实 3D 动画电影（写实电影感）：半写实 3D 渲染，真实材质与物理光照，人物与场景追求照片级可信度，运动与表演自然写实；深海冷调为主（墨蓝、青灰、暗绿、雾白），辅以风暴闪电的冷白高光与遗迹内暖金色微光点缀；整体低饱和、高对比，突出悬疑与冒险氛围。电影化运镜：缓慢推轨、手持跟拍与低角度仰拍建立压迫与探索感，硬切剪辑与快节奏五镜。

| 场景 | 版本 | 时间/天气/光线 | 出现片段 | 参考图 | 确认 |
| --- | --- | --- | --- | --- | --- |
| 龙三角外围海面 | 白昼转阴 v1 | 白昼 · 平静转阴 · 低压阴云 | 01 | 文字定义（一次性） | 待确认 |
| 龙三角核心水域 | 风暴 v1 | 风暴 · 浓雾 · 冷白闪电高光 | 02 | 文字定义（一次性） | 待确认 |
| 龙三角海底遗迹（外部） | 深蓝幽暗 v1 | 海底 · 深蓝幽暗 · 遗迹暖金微光 | 03 | refs/scenes/underwater-ruins.png | 待确认 |
| 海底遗迹内部回廊 | 暗绿冷调 v1 | 内部 · 暗绿冷调 · 异象光晕 | 04 | 文字定义（一次性） | 待确认 |
| 遗迹核心深渊 | 暖金 vs 墨蓝 v1 | 核心 · 暖金微光 vs 墨蓝暗调 | 05 | 文字定义（一次性） | 待确认 |

## 场景生成 Prompt（16:9）

**03 · 龙三角海底遗迹（外部）** — 本阶段已生成参考图

```text
A wide cinematic underwater establishing shot of a lost civilization's massive stone ruins emerging from the deep blue darkness on the ocean floor. Ancient megalithic structures, broken pillars and temple terraces, faint warm golden light glowing from within the ruins, deep blue and ink-black surrounding water, light rays filtering from far above. No people. Semi-realistic 3D cinematic render, physically-based materials and realistic cinematic lighting, low-saturation high-contrast deep-sea cold palette with warm golden accents. No text, no watermark.
```

**01 · 龙三角外围海面（白昼转阴）** — 待生成

```text
A wide cinematic establishing shot of the outer Dragon Triangle sea surface on a calm day turning overcast. A small single-person research boat floats on gently rolling deep-blue water, distant horizon under heavy dark storm clouds and a thick fog bank. No people. Semi-realistic 3D cinematic render, physically-based materials and realistic cinematic lighting, low-saturation high-contrast deep-sea cold palette of ink blue, cyan-grey and fog white. No text, no watermark.
```

**02 · 龙三角核心水域（风暴）** — 待生成

```text
A wide cinematic shot of the Dragon Triangle core waters in a violent storm. Towering dark waves crash around a small research boat, thick fog, dark green-black storm sky torn by cold white lightning, floating shipwreck debris and driftwood on the surface ahead. No people. Semi-realistic 3D cinematic render, physically-based materials and realistic cinematic lighting, low-saturation high-contrast deep-sea cold palette with cold white lightning highlights. No text, no watermark.
```

**04 · 海底遗迹内部回廊** — 待生成

```text
A cinematic shot inside an ancient submerged ruins corridor. Stone hallway with carved relief walls, dark green cold tone, strange shifting light halos and drifting particles in the water, eerie atmosphere, faint warm glow at the far end. No people. Semi-realistic 3D cinematic render, physically-based materials and realistic cinematic lighting, low-saturation high-contrast deep-sea cold palette of dark green and ink blue with subtle warm accents. No text, no watermark.
```

**05 · 遗迹核心深渊** — 待生成

```text
A cinematic shot of the core abyss inside the ancient ruins, a deep dark chasm opening in the ruins floor, warm golden light rising from the depths against ink-blue darkness, monumental scale, the golden glow illuminating the chasm edges. No people. Semi-realistic 3D cinematic render, physically-based materials and realistic cinematic lighting, low-saturation high-contrast palette contrasting warm golden light and ink-blue shadow. No text, no watermark.
```