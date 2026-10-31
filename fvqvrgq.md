代发 wailian999

[U93] JS：模板字符串
来源：http://jx.yuexingan06.cn

`共 ${n} 条`
来源：http://ad.521024.cn

[U94] JS：箭头函数
来源：http://mr.chemitech.net.cn

const double = x => x * 2;
来源：http://qx.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://gl.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://sh.newstarts.cn

[U96] JS：async/await 与异常
来源：http://bz.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pn.shxzskj.cn

[U97] JS：并发请求
来源：http://in.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yo.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://th.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qr.wgjwhj.cn

[U99] JS：事件监听
来源：http://ao.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://sq.nicolike.cn

[U100] JS：DOM 查询
来源：http://gu.wgjwhj.cn

document.querySelector(".item")
来源：http://jq.huanxung.cn

[U101] JS：classList 操作
来源：http://ga.newstarts.cn

el.classList.toggle("active")
来源：http://ec.asd995.cn

[U102] JS：本地存储
来源：http://zh.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zw.lnxyls.cn

[U103] JS：定时器
来源：http://ce.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fe.shxzskj.cn

[U104] JS：防抖
来源：http://yh.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ss.yuntaijiaju.cn

[U105] JS：节流
来源：http://xu.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mk.newstarts.cn

[U106] JS：日期格式化
来源：http://eh.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pv.newstarts.cn

[U107] JS：数字千分位
来源：http://yo.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://po.wgjwhj.cn

[U108] JS：随机整数
来源：http://pk.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ic.bjjhwx.cn

[U109] JS：数组分组
来源：http://un.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://wq.yuexingan06.cn

[U110] JS：数组分块
来源：http://fo.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gd.newstarts.cn

[U111] JS：对象转 Map
来源：http://ve.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://bv.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://bb.muxihuayi.cn

"7".padStart(3, "0")
来源：http://vs.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://jm.newstarts.cn

s.replaceAll("a", "b")
来源：http://cl.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://uz.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rf.colortex.cn

[U115] JS：生成 UUID
来源：http://xy.muxihuayi.cn

crypto.randomUUID()
来源：http://vx.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://qf.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://ci.shxzukj.cn

[U117] JS：单元测试
来源：http://go.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://nq.colortex.cn

[U118] JS：开发服务器
来源：http://mw.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://dt.yuexingan06.cn

[U119] JS：生产构建
来源：http://eu.jianghongdianzi.cn

npx vite build
来源：http://ez.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://vu.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://he.haigaiapp.cn

================================================================================
来源：http://kt.asd995.cn

统计汇总
来源：http://yz.hahajie.cn

================================================================================
来源：http://bv.hahajie.cn

按语言统计（条）：
来源：http://jn.szxytkj.cn

Python ......... 252
来源：http://wu.huixiangedu.cn

PHP ............ 252
来源：http://ch.colortex.cn

JavaScript ..... 252
来源：http://bb.9csxet.cn

TypeScript ..... 212
来源：http://ea.szxytkj.cn

Java ........... 212
来源：http://rd.szxytkj.cn

Go ............. 212
来源：http://tw.wgjwhj.cn

Ruby ........... 212
来源：http://mk.nicolike.cn

C# ............. 212
来源：http://gz.newstarts.cn

C .............. 30
来源：http://qs.chemitech.net.cn

C++ ............ 30
来源：http://yz.newstarts.cn

SQL ............ 90
来源：http://hk.hnjuh.cn

Bash ........... 80
来源：http://ky.haigaiapp.cn

Kotlin ......... 15
来源：http://we.panjiajie.cn

Swift .......... 15
来源：http://aa.wgjwhj.cn

Lua ............ 10
来源：http://ql.521024.cn

Perl ........... 10
来源：http://rw.lnxyls.cn

Scala .......... 10
来源：http://zt.yuntaijiaju.cn

------------------------------------
来源：http://sd.shxzskj.cn

合计 ........... 2106 条
来源：http://de.gzmigu.cn

按章节统计：
来源：http://ib.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kv.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yu.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://by.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qr.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rp.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sv.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hq.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ie.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dz.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uy.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://py.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ak.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dy.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yd.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rx.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://we.jctech888.com.cn

Q SQL 专题                              90
来源：http://au.newstarts.cn

R Bash 专题                             80
来源：http://gy.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://gs.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://ek.haigaiapp.cn

U 高频实用片段                         120
来源：http://ei.szsharing.cn

------------------------------------
来源：http://bm.wgjwhj.cn

合计                                  2106 条
来源：http://kl.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://vi.9csxet.cn

使用提醒
来源：http://qx.nszjky.cn

--------------------------------------------------------------------------------
来源：http://tr.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zf.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://he.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dn.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qy.newstarts.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pl.jctech888.com.cn

—— 文件结束 ——
来源：http://qx.newstarts.cn

================================================================================
来源：http://fd.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://vn.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://vt.newstarts.cn

================================================================================
来源：http://hx.521024.cn

【收录内容】
来源：http://yk.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uz.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ha.lnxyls.cn

SQL · Bash · C · C++
来源：http://ib.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qk.nicolike.cn

【使用说明】
来源：http://vr.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yi.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kx.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uc.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bp.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pz.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vv.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qv.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ki.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://il.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qv.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oi.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gh.shxzskj.cn

【文件统计】
来源：http://vi.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://og.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://dn.shtwfgs.cn

目  录
来源：http://jb.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://aw.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://io.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hf.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cl.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fn.colortex.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lw.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://no.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fd.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pf.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://or.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zb.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bg.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sg.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://st.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://em.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gl.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bn.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://by.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lx.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iv.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pz.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gd.haigaiapp.cn

================================================================================
来源：http://vl.bjjhwx.cn

A. 基础语法与类型
来源：http://yt.gzmigu.cn

================================================================================
来源：http://ya.shxzukj.cn

[A01] Hello World
来源：http://dw.panjiajie.cn

Py:   print("Hello, World!")
来源：http://jh.asd995.cn

PHP:  echo "Hello, World!";
来源：http://go.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://wf.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fo.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://kl.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://zo.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://ar.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ij.asd995.cn

[A02] 变量声明与赋值
来源：http://ij.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dr.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yr.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fh.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zg.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://go.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://ca.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://ly.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hq.muxihuayi.cn

[A03] 常量定义
来源：http://tx.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://se.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://pm.colortex.cn

JS:   const PI = 3.14159;
来源：http://fy.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://mh.521024.cn

Java: static final double PI = 3.14159;
来源：http://yj.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://xw.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://na.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://im.hnjuh.cn

[A04] 判断变量类型
来源：http://cd.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ws.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://al.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oz.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://mx.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bi.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pp.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hp.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://bn.panjiajie.cn

[A05] 整数除法与取模
来源：http://ot.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tq.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://za.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pt.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tg.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://xa.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://qw.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://dt.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://xb.muxihuayi.cn

[A06] 字符串转数字
来源：http://se.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://va.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ma.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zv.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ey.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hn.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ce.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wj.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fq.lnxyls.cn

[A07] 数字转字符串
来源：http://jt.yuntaijiaju.cn

Py:   str(42)
来源：http://jy.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://oy.521024.cn

JS:   String(42); (42).toString()
来源：http://ap.shtwfgs.cn

TS:   String(42)
来源：http://ve.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ig.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://vf.haigaiapp.cn

Ruby: 42.to_s
来源：http://py.chemitech.net.cn

C#:   42.ToString()
来源：http://ry.gzmigu.cn

[A08] 取整与四舍五入
来源：http://vh.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://um.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hr.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://om.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vw.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zv.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vy.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qo.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pc.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://jw.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jc.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lk.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ul.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sf.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://io.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ai.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hx.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lv.hahajie.cn

[A10] 生成随机数
来源：http://ck.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://dr.9csxet.cn

PHP:  random_int(1, 100);
来源：http://rc.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mr.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oq.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://jb.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cv.nszjky.cn

Ruby: rand(1..100)
来源：http://gm.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://hh.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://mj.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://nb.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cv.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ku.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vm.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://vp.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vh.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cu.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hw.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://td.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ka.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://es.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://xc.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://yz.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://wa.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fa.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://zh.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://jl.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vg.nszjky.cn

Py:   "第一行\n第二行"
来源：http://cx.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://ef.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://wl.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://xc.huanxung.cn

Java: "第一行\n第二行"
来源：http://bc.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://jy.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://ui.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://he.nszjky.cn

[A14] 注释写法
来源：http://zw.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ye.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ce.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://gl.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://tp.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mj.521024.cn

Go:   // 单行；/* 多行 */
来源：http://za.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://he.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://sc.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://kp.hnjuh.cn

Py:   value = data or "默认值"
来源：http://iz.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://jw.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://ba.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://ka.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tg.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://sc.521024.cn

Ruby: value = data || "默认值"
来源：http://jk.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://mg.hahajie.cn

[A16] 真假值判断规则
来源：http://fl.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://si.521024.cn


<!-- 参考信息 -->