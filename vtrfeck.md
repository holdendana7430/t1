代发 wailian999

[U89] JS：数组去重
来源：http://rm.shxzukj.cn

[...new Set(arr)]
来源：http://mb.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://bm.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://ku.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://iv.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ik.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://uk.chemitech.net.cn

structuredClone(obj)
来源：http://kd.gzmigu.cn

[U93] JS：模板字符串
来源：http://rc.bookmarksfly.cn

`共 ${n} 条`
来源：http://oz.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://tc.yuntaijiaju.cn

const double = x => x * 2;
来源：http://bb.nszjky.cn

[U95] JS：Promise 包装
来源：http://yq.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://ef.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://jx.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gi.newstarts.cn

[U97] JS：并发请求
来源：http://xb.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ys.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://nh.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://od.huanxung.cn

[U99] JS：事件监听
来源：http://nm.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://wq.szxytkj.cn

[U100] JS：DOM 查询
来源：http://rc.yuexingan06.cn

document.querySelector(".item")
来源：http://br.szxytkj.cn

[U101] JS：classList 操作
来源：http://tt.jctech888.com.cn

el.classList.toggle("active")
来源：http://mz.bookmarksfly.cn

[U102] JS：本地存储
来源：http://mw.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ea.asd995.cn

[U103] JS：定时器
来源：http://ml.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rc.shxzskj.cn

[U104] JS：防抖
来源：http://qa.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xr.huanxung.cn

[U105] JS：节流
来源：http://op.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zw.haigaiapp.cn

[U106] JS：日期格式化
来源：http://rq.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cp.newstarts.cn

[U107] JS：数字千分位
来源：http://mt.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yy.jctech888.com.cn

[U108] JS：随机整数
来源：http://am.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qy.haigaiapp.cn

[U109] JS：数组分组
来源：http://rb.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://fs.nszjky.cn

[U110] JS：数组分块
来源：http://jr.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qb.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://mt.9csxet.cn

new Map(Object.entries(obj))
来源：http://qz.jctech888.com.cn

[U112] JS：字符串补位
来源：http://rc.szxytkj.cn

"7".padStart(3, "0")
来源：http://fc.szsharing.cn

[U113] JS：正则替换全部
来源：http://uc.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://en.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://qg.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bn.nszjky.cn

[U115] JS：生成 UUID
来源：http://wk.shxzskj.cn

crypto.randomUUID()
来源：http://tb.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://se.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://vw.nicolike.cn

[U117] JS：单元测试
来源：http://ks.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://hw.colortex.cn

[U118] JS：开发服务器
来源：http://cc.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://ry.hahajie.cn

[U119] JS：生产构建
来源：http://pr.jctech888.com.cn

npx vite build
来源：http://xu.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://uc.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://vs.lnxyls.cn

================================================================================
来源：http://tt.haigaiapp.cn

统计汇总
来源：http://wc.gzmigu.cn

================================================================================
来源：http://mo.hnjuh.cn

按语言统计（条）：
来源：http://mg.bookmarksfly.cn

Python ......... 252
来源：http://ps.muxihuayi.cn

PHP ............ 252
来源：http://sp.bookmarksfly.cn

JavaScript ..... 252
来源：http://lp.yuexingan06.cn

TypeScript ..... 212
来源：http://zy.hnjuh.cn

Java ........... 212
来源：http://qm.shtwfgs.cn

Go ............. 212
来源：http://ve.gzmigu.cn

Ruby ........... 212
来源：http://dk.shxzskj.cn

C# ............. 212
来源：http://wx.panjiajie.cn

C .............. 30
来源：http://ji.huanxung.cn

C++ ............ 30
来源：http://qw.gzmigu.cn

SQL ............ 90
来源：http://az.jctech888.com.cn

Bash ........... 80
来源：http://do.panjiajie.cn

Kotlin ......... 15
来源：http://jh.panjiajie.cn

Swift .......... 15
来源：http://zf.jctech888.com.cn

Lua ............ 10
来源：http://db.gzmigu.cn

Perl ........... 10
来源：http://va.colortex.cn

Scala .......... 10
来源：http://jf.colortex.cn

------------------------------------
来源：http://wo.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://xp.huixiangedu.cn

按章节统计：
来源：http://oi.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gx.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nx.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ii.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sg.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nq.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://js.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ve.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zi.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fu.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ci.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ma.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rh.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nm.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yp.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://km.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ac.szxytkj.cn

Q SQL 专题                              90
来源：http://pv.shxzskj.cn

R Bash 专题                             80
来源：http://yw.nicolike.cn

S C / C++ 专题                          60
来源：http://uq.haigaiapp.cn

T 其他语言补充                          60
来源：http://bt.colortex.cn

U 高频实用片段                         120
来源：http://fs.jianghongdianzi.cn

------------------------------------
来源：http://ag.asd995.cn

合计                                  2106 条
来源：http://go.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://oa.shxzskj.cn

使用提醒
来源：http://re.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://js.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bd.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pl.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://on.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qm.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ya.jctech888.com.cn

—— 文件结束 ——
来源：http://hm.9csxet.cn

================================================================================
来源：http://gc.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://sb.szsharing.cn

Common Programming Examples Cheat Book
来源：http://be.nszjky.cn

================================================================================
来源：http://wl.nszjky.cn

【收录内容】
来源：http://sr.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vu.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bw.nicolike.cn

SQL · Bash · C · C++
来源：http://es.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ig.colortex.cn

【使用说明】
来源：http://va.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xe.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ir.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://un.jianghongdianzi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vl.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ui.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gq.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pn.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vy.521024.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gi.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hj.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qc.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yx.9csxet.cn

【文件统计】
来源：http://ws.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://do.szsharing.cn

--------------------------------------------------------------------------------
来源：http://lz.asd995.cn

目  录
来源：http://ru.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://fq.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wn.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://av.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ho.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://an.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yh.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ti.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ci.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rr.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zx.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xu.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ts.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jw.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ae.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cl.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://th.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://in.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lt.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vt.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tu.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://it.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rh.huixinmuqiang.cn

================================================================================
来源：http://rj.wgjwhj.cn

A. 基础语法与类型
来源：http://kl.bookmarksfly.cn

================================================================================
来源：http://gg.shxzukj.cn

[A01] Hello World
来源：http://of.lnxyls.cn

Py:   print("Hello, World!")
来源：http://ea.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://hu.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://ak.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://em.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://sa.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://mn.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://id.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ee.nicolike.cn

[A02] 变量声明与赋值
来源：http://ek.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yk.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qw.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hn.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vg.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://mx.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://ce.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://zl.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yg.nicolike.cn

[A03] 常量定义
来源：http://fu.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pq.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://gx.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://kk.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://kc.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://vt.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://dd.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://kd.521024.cn

C#:   const double PI = 3.14159;
来源：http://zk.gzmigu.cn

[A04] 判断变量类型
来源：http://zn.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jy.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lg.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oz.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://ma.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://db.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gt.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fw.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://gv.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://iq.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gi.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wt.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://um.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sx.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://lt.521024.cn

Go:   7 / 2; 7 % 2
来源：http://ov.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://dj.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://on.521024.cn

[A06] 字符串转数字
来源：http://eb.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://gf.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ca.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pw.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zk.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zf.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pd.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ao.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zv.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://uy.lnxyls.cn

Py:   str(42)
来源：http://gb.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://iy.521024.cn

JS:   String(42); (42).toString()
来源：http://if.yuexingan06.cn

TS:   String(42)
来源：http://rt.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ir.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://ic.shtwfgs.cn

Ruby: 42.to_s
来源：http://nw.hahajie.cn

C#:   42.ToString()
来源：http://oe.szxytkj.cn

[A08] 取整与四舍五入
来源：http://sc.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ed.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oe.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iy.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dm.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lb.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hm.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://af.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yg.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://ka.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nu.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yu.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kb.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dw.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nk.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mt.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mq.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hq.shxzukj.cn

[A10] 生成随机数
来源：http://kl.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://fi.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://fi.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vq.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nl.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://iq.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://he.jctech888.com.cn

Ruby: rand(1..100)
来源：http://ch.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://fx.nicolike.cn

[A11] 条件表达式（三元）
来源：http://dh.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://ja.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ti.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qm.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yl.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://ib.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wp.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yk.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ys.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://xo.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ri.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lt.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://hc.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://ly.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://iv.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vp.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://do.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://za.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ez.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://iw.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://nz.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://mw.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://fq.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://lw.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://cw.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://ml.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://uz.huixiangedu.cn

[A14] 注释写法
来源：http://mp.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://en.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sc.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://hw.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://ke.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sd.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://rw.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lw.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://ub.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://fz.shxzskj.cn

Py:   value = data or "默认值"
来源：http://iv.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://mb.521024.cn


<!-- 参考信息 -->