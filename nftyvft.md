代发 wailian999

[U93] JS：模板字符串
来源：http://fx.haigaiapp.cn

`共 ${n} 条`
来源：http://ft.shxzukj.cn

[U94] JS：箭头函数
来源：http://ea.huixinmuqiang.cn

const double = x => x * 2;
来源：http://sr.szxytkj.cn

[U95] JS：Promise 包装
来源：http://rm.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://dz.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://ex.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mr.huixiangedu.cn

[U97] JS：并发请求
来源：http://yz.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xe.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://ux.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://es.asd995.cn

[U99] JS：事件监听
来源：http://ng.521024.cn

el.addEventListener("click", e => {})
来源：http://nw.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://gb.haigaiapp.cn

document.querySelector(".item")
来源：http://wj.haigaiapp.cn

[U101] JS：classList 操作
来源：http://ez.lnxyls.cn

el.classList.toggle("active")
来源：http://jt.gzmigu.cn

[U102] JS：本地存储
来源：http://ie.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yx.jianghongdianzi.cn

[U103] JS：定时器
来源：http://nt.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ds.szxytkj.cn

[U104] JS：防抖
来源：http://zq.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bp.bjjhwx.cn

[U105] JS：节流
来源：http://lc.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sf.hahajie.cn

[U106] JS：日期格式化
来源：http://ey.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://md.chemitech.net.cn

[U107] JS：数字千分位
来源：http://nx.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gi.newstarts.cn

[U108] JS：随机整数
来源：http://nr.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jl.szsharing.cn

[U109] JS：数组分组
来源：http://ig.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://uj.szxytkj.cn

[U110] JS：数组分块
来源：http://hl.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kl.521024.cn

[U111] JS：对象转 Map
来源：http://ns.asd995.cn

new Map(Object.entries(obj))
来源：http://rs.wgjwhj.cn

[U112] JS：字符串补位
来源：http://qn.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://cx.hnjuh.cn

[U113] JS：正则替换全部
来源：http://jy.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://nn.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://bj.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pk.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://br.lnxyls.cn

crypto.randomUUID()
来源：http://ye.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://cs.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://jw.haigaiapp.cn

[U117] JS：单元测试
来源：http://vq.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://av.lnxyls.cn

[U118] JS：开发服务器
来源：http://lp.9csxet.cn

npm i -D vite;  npx vite
来源：http://rc.yuexingan06.cn

[U119] JS：生产构建
来源：http://xy.nszjky.cn

npx vite build
来源：http://qs.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://xy.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://og.chemitech.net.cn

================================================================================
来源：http://rx.bjjhwx.cn

统计汇总
来源：http://nx.nszjky.cn

================================================================================
来源：http://ks.panjiajie.cn

按语言统计（条）：
来源：http://nk.huixiangedu.cn

Python ......... 252
来源：http://lq.nszjky.cn

PHP ............ 252
来源：http://ju.muxihuayi.cn

JavaScript ..... 252
来源：http://yc.nszjky.cn

TypeScript ..... 212
来源：http://cd.lnxyls.cn

Java ........... 212
来源：http://ol.521024.cn

Go ............. 212
来源：http://aj.wgjwhj.cn

Ruby ........... 212
来源：http://it.asd995.cn

C# ............. 212
来源：http://aa.newstarts.cn

C .............. 30
来源：http://rt.9csxet.cn

C++ ............ 30
来源：http://vp.huanxung.cn

SQL ............ 90
来源：http://th.jianghongdianzi.cn

Bash ........... 80
来源：http://dg.jianghongdianzi.cn

Kotlin ......... 15
来源：http://pp.huanxung.cn

Swift .......... 15
来源：http://lm.chemitech.net.cn

Lua ............ 10
来源：http://wr.hahajie.cn

Perl ........... 10
来源：http://to.nszjky.cn

Scala .......... 10
来源：http://ls.jctech888.com.cn

------------------------------------
来源：http://la.hnjuh.cn

合计 ........... 2106 条
来源：http://jc.newstarts.cn

按章节统计：
来源：http://cr.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gc.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fh.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wk.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wn.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fm.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ym.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rf.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nj.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ie.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ev.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ci.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hw.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qj.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vq.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tf.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bi.wgjwhj.cn

Q SQL 专题                              90
来源：http://xc.lnxyls.cn

R Bash 专题                             80
来源：http://pa.szxytkj.cn

S C / C++ 专题                          60
来源：http://nm.shxzskj.cn

T 其他语言补充                          60
来源：http://iy.bjjhwx.cn

U 高频实用片段                         120
来源：http://rs.yuntaijiaju.cn

------------------------------------
来源：http://js.chemitech.net.cn

合计                                  2106 条
来源：http://vj.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://vu.jianghongdianzi.cn

使用提醒
来源：http://wy.nszjky.cn

--------------------------------------------------------------------------------
来源：http://ar.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tt.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wq.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bl.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fk.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ld.nicolike.cn

—— 文件结束 ——
来源：http://kp.jianghongdianzi.cn

================================================================================
来源：http://ot.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://hn.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://pj.muxihuayi.cn

================================================================================
来源：http://fr.wgjwhj.cn

【收录内容】
来源：http://vl.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jw.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jg.szxytkj.cn

SQL · Bash · C · C++
来源：http://io.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://te.shtwfgs.cn

【使用说明】
来源：http://jj.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lw.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cg.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hy.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://st.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jh.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tj.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vh.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ym.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vh.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qi.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://td.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bu.asd995.cn

【文件统计】
来源：http://tz.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bs.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://tj.szsharing.cn

目  录
来源：http://hm.newstarts.cn

--------------------------------------------------------------------------------
来源：http://qt.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rr.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zy.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dm.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fp.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qz.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ri.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ri.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xe.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tj.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nf.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://og.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ed.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zw.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ox.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uy.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nv.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zf.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pf.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vn.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xs.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://at.shxzskj.cn

================================================================================
来源：http://ji.hnjuh.cn

A. 基础语法与类型
来源：http://hm.huanxung.cn

================================================================================
来源：http://xx.gzmigu.cn

[A01] Hello World
来源：http://qj.colortex.cn

Py:   print("Hello, World!")
来源：http://jd.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://yi.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://px.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uw.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://xx.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://wl.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://wv.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ox.9csxet.cn

[A02] 变量声明与赋值
来源：http://py.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xa.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xx.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pw.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mi.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://fp.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://ju.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://xm.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mu.jianghongdianzi.cn

[A03] 常量定义
来源：http://ts.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yp.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://zx.asd995.cn

JS:   const PI = 3.14159;
来源：http://ad.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://nn.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://ob.gzmigu.cn

Go:   const PI = 3.14159
来源：http://up.hahajie.cn

Ruby: PI = 3.14159
来源：http://ic.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://ls.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://lq.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://od.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yb.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://do.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://dw.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ss.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fb.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oy.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://ep.shxzskj.cn

[A05] 整数除法与取模
来源：http://hv.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cz.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://il.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ru.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zo.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://gc.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://eg.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://yg.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://ol.jctech888.com.cn

[A06] 字符串转数字
来源：http://pc.asd995.cn

Py:   int("42"); float("3.14")
来源：http://bz.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fs.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fl.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sc.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yx.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ny.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://km.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bo.newstarts.cn

[A07] 数字转字符串
来源：http://co.yuntaijiaju.cn

Py:   str(42)
来源：http://tr.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://gd.newstarts.cn

JS:   String(42); (42).toString()
来源：http://pe.huixiangedu.cn

TS:   String(42)
来源：http://pe.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pl.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://ck.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://dp.chemitech.net.cn

C#:   42.ToString()
来源：http://wk.huanxung.cn

[A08] 取整与四舍五入
来源：http://kg.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://th.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uv.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ag.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kk.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dj.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mb.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ic.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ps.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://lf.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kv.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uu.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ib.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tq.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lk.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://be.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xp.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zh.muxihuayi.cn

[A10] 生成随机数
来源：http://nw.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://ff.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://ur.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zf.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://um.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://ru.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dc.huixiangedu.cn

Ruby: rand(1..100)
来源：http://bj.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://jh.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://bq.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://jr.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rc.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tn.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qv.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://zu.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://up.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gq.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bk.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://rt.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tx.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://df.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://os.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://uv.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://by.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ud.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://qw.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://iz.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ob.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://is.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://bi.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://pp.colortex.cn

TS:   "第一行\n第二行"
来源：http://lo.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://wa.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://bi.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://ou.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://ho.haigaiapp.cn

[A14] 注释写法
来源：http://of.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://la.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zf.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://gk.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://mw.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rv.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://qy.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fx.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://vg.hahajie.cn

[A15] 空值判断与默认值
来源：http://nj.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://cq.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://ke.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://ag.521024.cn

TS:   const value = data ?? "默认值";
来源：http://st.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eo.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://pa.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://aa.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://ei.haigaiapp.cn

[A16] 真假值判断规则
来源：http://nb.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lx.szsharing.cn


<!-- 参考信息 -->