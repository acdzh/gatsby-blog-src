---
title: "ShortCode 测试页"
date: 2020-04-24T22:52:10+08:00
draft: false
comment: true
slug: shortcode_test
description: ""
tags: []
series: []
categories: [其他]
---

>test page

## 网易云音乐

```tsx
type propsType = {
  id: string;
  type?: 1 | 2 | 3; // default: 2
  autoPlay?: boolean; // default: false
  showInfo?: boolean; // default: true
};

<netease-music id="5264842" autoPlay={false} showInfo={false} />
<netease-music id="2064167949" type={3} />
```

<netease-music id="5264842" autoPlay={false} showInfo={false} />
<netease-music id="2064167949" type={3} />

## YouTube

```tsx
type propsType = {
  id: string;
  width?: number;  // default: 16
  height?: number; // default: 9
  start?: number; // default: 0
  showControls?: boolean; // default: true
};

<youtube id="Ap0huJwyT7g" width={560} height={315} start={64} />
```

<youtube id="Ap0huJwyT7g" width={560} height={315} start={64} />

## 哔哩哔哩

```tsx
type propsType = {
  aid?: string;
  bid?: string;
  page?: number; // default: 1
  width?: number; // default: 16
  height?: number; // default: 9
};

<bilibili aid="47480567" />
<bilibili bid="BV19b411s7dY" page={2} />
```

<bilibili aid="47480567" />
<bilibili bid="BV19b411s7dY" page={2} />

## CodePen

<codepen id="OJRvrzO" theme="dark" />

## video

<video src="video/test.mp4" type="mp4" />
```
