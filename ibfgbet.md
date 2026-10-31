代发 wailian999

[U91] JS：对象键值遍历
来源：http://ml.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ev.yuexingan06.cn

[U92] JS：深拷贝
来源：http://rd.jianghongdianzi.cn

structuredClone(obj)
来源：http://iw.szxytkj.cn

[U93] JS：模板字符串
来源：http://zz.shxzukj.cn

`共 ${n} 条`
来源：http://yh.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://nx.lnxyls.cn

const double = x => x * 2;
来源：http://oo.lnxyls.cn

[U95] JS：Promise 包装
来源：http://zu.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://qt.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://rj.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ph.nszjky.cn

[U97] JS：并发请求
来源：http://oa.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xf.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://wh.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dn.gzmigu.cn

[U99] JS：事件监听
来源：http://eg.hahajie.cn

el.addEventListener("click", e => {})
来源：http://id.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://sm.jianghongdianzi.cn

document.querySelector(".item")
来源：http://ro.wgjwhj.cn

[U101] JS：classList 操作
来源：http://kh.hnjuh.cn

el.classList.toggle("active")
来源：http://js.hnjuh.cn

[U102] JS：本地存储
来源：http://eq.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mk.huixinmuqiang.cn

[U103] JS：定时器
来源：http://ts.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oy.colortex.cn

[U104] JS：防抖
来源：http://gb.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xv.lnxyls.cn

[U105] JS：节流
来源：http://xh.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mx.yuexingan06.cn

[U106] JS：日期格式化
来源：http://zp.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ue.szsharing.cn

[U107] JS：数字千分位
来源：http://wj.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eh.colortex.cn

[U108] JS：随机整数
来源：http://vv.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mj.newstarts.cn

[U109] JS：数组分组
来源：http://bn.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://ib.shtwfgs.cn

[U110] JS：数组分块
来源：http://us.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gp.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://ip.521024.cn

new Map(Object.entries(obj))
来源：http://br.nicolike.cn

[U112] JS：字符串补位
来源：http://vr.panjiajie.cn

"7".padStart(3, "0")
来源：http://ea.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://kx.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://lz.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://gf.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mj.nszjky.cn

[U115] JS：生成 UUID
来源：http://fu.chemitech.net.cn

crypto.randomUUID()
来源：http://yp.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://db.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://tt.hnjuh.cn

[U117] JS：单元测试
来源：http://xn.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://of.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://la.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://on.jctech888.com.cn

[U119] JS：生产构建
来源：http://hn.9csxet.cn

npx vite build
来源：http://ef.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://ea.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://gf.nszjky.cn

================================================================================
来源：http://pq.newstarts.cn

统计汇总
来源：http://nw.bookmarksfly.cn

================================================================================
来源：http://ht.szxytkj.cn

按语言统计（条）：
来源：http://qe.jianghongdianzi.cn

Python ......... 252
来源：http://dv.bjjhwx.cn

PHP ............ 252
来源：http://ng.gzmigu.cn

JavaScript ..... 252
来源：http://wk.colortex.cn

TypeScript ..... 212
来源：http://nj.newstarts.cn

Java ........... 212
来源：http://bc.bjjhwx.cn

Go ............. 212
来源：http://wb.nicolike.cn

Ruby ........... 212
来源：http://sn.yuexingan06.cn

C# ............. 212
来源：http://oh.haigaiapp.cn

C .............. 30
来源：http://by.yuntaijiaju.cn

C++ ............ 30
来源：http://nz.bookmarksfly.cn

SQL ............ 90
来源：http://ky.jctech888.com.cn

Bash ........... 80
来源：http://il.nicolike.cn

Kotlin ......... 15
来源：http://tn.asd995.cn

Swift .......... 15
来源：http://bh.shxzskj.cn

Lua ............ 10
来源：http://jr.bjjhwx.cn

Perl ........... 10
来源：http://bf.gzmigu.cn

Scala .......... 10
来源：http://bx.lnxyls.cn

------------------------------------
来源：http://ux.yuexingan06.cn

合计 ........... 2106 条
来源：http://sm.szsharing.cn

按章节统计：
来源：http://un.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ss.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qb.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uj.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lr.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yp.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zf.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wj.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://to.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rb.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jr.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bu.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gs.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hm.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mp.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kj.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nf.huanxung.cn

Q SQL 专题                              90
来源：http://rg.lnxyls.cn

R Bash 专题                             80
来源：http://ab.panjiajie.cn

S C / C++ 专题                          60
来源：http://ee.jctech888.com.cn

T 其他语言补充                          60
来源：http://xc.gzmigu.cn

U 高频实用片段                         120
来源：http://oy.shxzskj.cn

------------------------------------
来源：http://gu.panjiajie.cn

合计                                  2106 条
来源：http://nt.9csxet.cn

--------------------------------------------------------------------------------
来源：http://vh.szxytkj.cn

使用提醒
来源：http://mh.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ul.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lu.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://if.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oy.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://od.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vy.huixinmuqiang.cn

—— 文件结束 ——
来源：http://ut.panjiajie.cn

================================================================================
来源：http://mq.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://gj.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://hl.9csxet.cn

================================================================================
来源：http://bb.nicolike.cn

【收录内容】
来源：http://ya.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tl.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eh.9csxet.cn

SQL · Bash · C · C++
来源：http://ta.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ma.gzmigu.cn

【使用说明】
来源：http://lk.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qe.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mt.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ig.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eb.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ip.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zd.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oo.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pd.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pk.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mz.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xv.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uc.shxzskj.cn

【文件统计】
来源：http://wx.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sy.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://nd.huixinmuqiang.cn

目  录
来源：http://cd.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://mq.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qe.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gt.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vw.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pk.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hq.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gi.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wq.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://be.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ox.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vj.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hl.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ga.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yd.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mo.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lm.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mp.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pg.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sw.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iv.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dg.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ba.haigaiapp.cn

================================================================================
来源：http://xb.shxzskj.cn

A. 基础语法与类型
来源：http://qu.lnxyls.cn

================================================================================
来源：http://et.lnxyls.cn

[A01] Hello World
来源：http://dq.jctech888.com.cn

Py:   print("Hello, World!")
来源：http://px.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://io.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://ht.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gi.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://tj.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://mb.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://bd.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rs.521024.cn

[A02] 变量声明与赋值
来源：http://fw.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sn.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://iw.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gb.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://at.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://ev.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://zf.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://dt.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://it.521024.cn

[A03] 常量定义
来源：http://dz.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rc.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://jp.newstarts.cn

JS:   const PI = 3.14159;
来源：http://rp.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://rv.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://zq.newstarts.cn

Go:   const PI = 3.14159
来源：http://sw.9csxet.cn

Ruby: PI = 3.14159
来源：http://pk.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://zi.haigaiapp.cn

[A04] 判断变量类型
来源：http://ws.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qt.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://px.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wr.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://zw.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vr.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://se.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://se.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://kn.szsharing.cn

[A05] 整数除法与取模
来源：http://ij.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fz.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://af.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mg.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rw.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://ao.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://rk.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://jb.521024.cn

C#:   7 / 2; 7 % 2
来源：http://cs.huanxung.cn

[A06] 字符串转数字
来源：http://mj.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://vy.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nw.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bz.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pu.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gg.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bh.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eu.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zq.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://oy.huanxung.cn

Py:   str(42)
来源：http://wi.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://sh.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://du.bookmarksfly.cn

TS:   String(42)
来源：http://xy.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xb.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://dl.yuexingan06.cn

Ruby: 42.to_s
来源：http://tc.yuexingan06.cn

C#:   42.ToString()
来源：http://uw.asd995.cn

[A08] 取整与四舍五入
来源：http://om.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dq.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sy.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ad.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yw.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sa.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pi.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lf.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lv.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://ad.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fx.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://le.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ov.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ap.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kq.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xo.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mz.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gu.chemitech.net.cn

[A10] 生成随机数
来源：http://eo.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://ig.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://yu.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nr.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pz.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://sc.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xt.lnxyls.cn

Ruby: rand(1..100)
来源：http://xm.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://ga.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://dl.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://ou.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wn.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cj.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ei.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://gq.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gp.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ib.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qv.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://mi.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fl.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pe.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://ey.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://bo.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://lo.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mq.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://wy.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://se.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fw.9csxet.cn

Py:   "第一行\n第二行"
来源：http://wx.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://vr.521024.cn

JS:   "第一行\n第二行"
来源：http://tz.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://xo.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://ai.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://ne.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://wi.colortex.cn

C#:   "第一行\n第二行"
来源：http://nw.yuexingan06.cn

[A14] 注释写法
来源：http://gh.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vx.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sv.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://hv.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://yb.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sz.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://jh.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kv.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://xk.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://yi.newstarts.cn

Py:   value = data or "默认值"
来源：http://hs.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://ss.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://hi.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://dx.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://he.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://mq.jctech888.com.cn


<!-- 参考信息 -->