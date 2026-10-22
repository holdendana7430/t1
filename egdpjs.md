代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mcnmqwkd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vfjjuhuv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2rpwkgkhp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2czanrwud.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nkaxbzvi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uvyyquwg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rasxohxb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2saffrful.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2rpmpbwgg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rhcghxvh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rybbgmah.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jdolgirl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2aglnlfim.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ufcxdgyn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wbdevqvn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tbshxpvt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2bvtkomfy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2mydwcjqw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2uphxvkrn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yuqdpofh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2pefxndmi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oxwsmhfx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2yzmnuibw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2blkkmqmx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2sgzbcmch.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yyzpkcru.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pfyqsrqi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2tpjbavdz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ypksusou.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2odvmwdnc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zsgvjchd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ovdqxhhz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cyxbotia.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2tctuaick.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2oxciyihs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kmdjtbdm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2umypqhib.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cjotqefi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qsoiizsh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qanznhbh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dpdvkqnf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xkhxcwpt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xisnnxkn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2otcliidr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gisvygkv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2quebdkch.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2dzxcvbms.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jwgtuljm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qngbwzkb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2cltrgjbi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2gpiyupms.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zrnsdnac.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hywbfmck.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2feejyhve.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xkwnrqtw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pxccykqz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ehmxfumd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bqqmfeob.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qbtlajoc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwiiluso.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gkqiucrz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sonzyuac.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2cnrvafzn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ldiwixct.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ogctftlz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2eowdmhxm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rtbypvup.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ukyltyxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xotifrzv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vwduakex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wepenzbe.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xlnlubpd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rncgonwc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2zykdmhht.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ucjaybyd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tuzpynfm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pssistjo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bmwoskll.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xwtyzobl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jwhwpage.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2cxtboomd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2faizjavy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dqkpoazh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2efhympzx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2emayydtj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qocsnmyi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2fdlcwwyb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2gownpdeu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tjukvebe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jrqaqslq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qbpqrfqa.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2pizzgtsl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hzwaqwdv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2curyoyxr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pcwrjmgz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hpeyhinu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vaitthlo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qseidlbm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nionegqd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2oklawrza.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hpauwreb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lqpaxjzo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bixxijct.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yvsestqu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pdympcyh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xfyvyfot.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2wmasjuxg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2folyzugz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2uyuwmmzg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bniiikon.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2dlggkbnt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dtvagqau.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2vtlnhfhy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ozibbfiq.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2pleyacbh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mojomwrl.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wcueogyt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tcfpiztl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2woyxxwur.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2rjbchmtk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2qeudbbgw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2yvnwshoa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2hgwwmtxf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jehzbmgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylxnmubu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2hqdhmcbt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wizeidhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhlglvls.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2cvypxvay.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ljzhufro.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2nssyeiqt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2bcxbbbxo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2wnfmkgni.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2fzokqrhg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rimopzdb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gvfzzmpe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2chaczwjn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2khyaihwm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2jjfxoumv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ecdskvjl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2pyxesame.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2rutoaolt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2slnstntc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2cwwspdkm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2bajetkhi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2pwmyudkz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mggfcrgx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2gtdufwew.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mkzgegqx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2sukxjanj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ttweefuc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2osgovmng.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ftljxymq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xcaxsney.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2byzoqpvm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2igqwaqnh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dxuqdiiz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yglblshh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wfyqyxvn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kfrcwefq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qhfybdgp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lrviwckp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wqymiaqi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bighjkex.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fmjikazq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2cnaiadqj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2coeoreju.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yfxnqvph.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tcxlwtrk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dzbvlqlz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2elzuibjn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2amancbmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuqnswpz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2quneqkas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufjgjwah.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tsapjxyr.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gvjzbxlo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2erelxiye.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qzawjtri.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2etrwhwbw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qmufwqeu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rixqaogk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2opxdezhz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bypyxaob.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2zohqirti.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2kawkehhm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gmywborj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uoqqjclm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2bhoicnoe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2veljfcfa.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2lgkkmgij.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2sstadrny.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fpvidfpd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2kabhnuzc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2vjzajzub.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2axyymfwh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pzthjzqn.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2drekrwnl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2edvghghz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pwllgmri.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rxozggpm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bycyvrzq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zunvroir.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2bzdcwidc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fsycufyv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yeyxldez.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2iodogygc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2qnqikzbx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vvhfuhkj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2gcuqypsl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2tscoqyda.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2romhgzto.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2skajfbvl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ciowqyvo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ocfuckvx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mjopynqf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hqloywmy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tvxnniwr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xfimoior.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2coxdhytv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ylfpskyc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oedtptun.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2oezqmhgo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2arsoqrmg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2svjwbsdz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qphuksgi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2juehhhog.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2lzdwfizv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kfjahrht.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jnqutqrj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2odhnryso.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2kbgdkntt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2cfbkuhnz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jrallfwk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2fpegctsl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2cawgestv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2jdueteax.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2auvmkbfa.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2vwzyizbg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dapitqsc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2gwnqtosz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yuayqfxb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vjhdaglr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uwsuangw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vnairhfc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2vmhmeoel.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2svgezfrf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2luubtcra.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2npfuaulr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evhrkqld.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eqksbsgy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ieryocns.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nmsdncic.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2oitgfwml.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ktuwfzwm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehyksjqv.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2oeohzoby.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2cobpmxfj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2zuwfulvt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wlurdaay.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvzzprqk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eadjsnos.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2rswofyvn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2uznhqvxp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2uejtygpz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wsiafvdo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hlhjjyzn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2drtkxaqk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hwxjkska.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zqcsuhui.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bzcagzxo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2vytudbbi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2clzijpnk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jeicnhgh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wupzbjgq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xzyyewwn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2uqrvaiha.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zrnarzut.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hiowkpcc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ljnmncjw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2muwkwpuf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2btassvtt.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2kqfcdcck.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ssfpejjo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zxnaljdw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ddffcvcb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2savpnkot.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ftmgnfqj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pycvjddq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lppsmviy.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xyylaezn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2chmrgxov.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2mlnasrfg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2hedddqri.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pjrelwqc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2djpchzcb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xviaujpw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2kjmxplne.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kkaetgzr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vkedzpio.html


<!-- 参考信息 -->