---
title: "工具页"
date: 2019-01-01T00:00:00+08:00
draft: false
comment: false
description: ""
tags: []
series: []
categories: []
nolicense: true
toc: true
---

## aria2


<section onLoad={() => {
  window.aria2ButtonsOnclick = function(type) {
    let val = document.getElementById('secret').value;
    const oldAria2Key = localStorage.getItem('aria2key');
    if (val === '') { val = oldAria2Key; }
    else { localStorage.setItem('aria2key', val); }
    open( type === 'panel' 
      ? val === '' 
        ? 'tools/aria2ng/' 
        : 'tools/aria2ng/#!/settings/rpc/set/wss/acdzharia2.herokuapp.com/443/jsonrpc/'+btoa(val)
      : 'https://acdzharia2.herokuapp.com/downloads/'+btoa(val)+'/',
      '_blank'
    );
  };
}}>
    <label for="secret">Password:</label>
    <input id="secret" type="text" />
    <button id="panel" onClick={() => { aria2ButtonsOnclick('panel'); }}>前往Aria2面板</button>
    <button id="downloads" onClick={() => { aria2ButtonsOnclick('downloads'); }}>查看下载文件</button>
</section>