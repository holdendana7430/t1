代发 wailian999

[U93] JS：模板字符串
来源：http://og.haigaiapp.cn

`共 ${n} 条`
来源：http://dr.shxzukj.cn

[U94] JS：箭头函数
来源：http://id.bjjhwx.cn

const double = x => x * 2;
来源：http://zy.newstarts.cn

[U95] JS：Promise 包装
来源：http://cn.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://ev.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://cq.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lm.bjjhwx.cn

[U97] JS：并发请求
来源：http://ae.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ra.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://ch.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ol.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://dl.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://ws.nicolike.cn

[U100] JS：DOM 查询
来源：http://dp.huixinmuqiang.cn

document.querySelector(".item")
来源：http://ar.shxzskj.cn

[U101] JS：classList 操作
来源：http://lw.shtwfgs.cn

el.classList.toggle("active")
来源：http://iq.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://fs.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://el.shtwfgs.cn

[U103] JS：定时器
来源：http://ad.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zr.gzmigu.cn

[U104] JS：防抖
来源：http://cd.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wf.shxzukj.cn

[U105] JS：节流
来源：http://fa.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ha.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://wf.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yx.huixiangedu.cn

[U107] JS：数字千分位
来源：http://gp.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ik.asd995.cn

[U108] JS：随机整数
来源：http://fm.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qx.gzmigu.cn

[U109] JS：数组分组
来源：http://bk.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://lk.bjjhwx.cn

[U110] JS：数组分块
来源：http://ev.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ut.shxzskj.cn

[U111] JS：对象转 Map
来源：http://hq.lnxyls.cn

new Map(Object.entries(obj))
来源：http://de.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://oo.521024.cn

"7".padStart(3, "0")
来源：http://zj.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://fm.521024.cn

s.replaceAll("a", "b")
来源：http://vp.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://rv.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wt.9csxet.cn

[U115] JS：生成 UUID
来源：http://yi.yuexingan06.cn

crypto.randomUUID()
来源：http://hw.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ye.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://on.newstarts.cn

[U117] JS：单元测试
来源：http://ac.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://af.colortex.cn

[U118] JS：开发服务器
来源：http://ob.lnxyls.cn

npm i -D vite;  npx vite
来源：http://tn.shxzskj.cn

[U119] JS：生产构建
来源：http://ua.huixiangedu.cn

npx vite build
来源：http://tj.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://fz.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://ef.shxzukj.cn

================================================================================
来源：http://wi.wgjwhj.cn

统计汇总
来源：http://wj.lnxyls.cn

================================================================================
来源：http://gg.panjiajie.cn

按语言统计（条）：
来源：http://si.huixinmuqiang.cn

Python ......... 252
来源：http://th.huixinmuqiang.cn

PHP ............ 252
来源：http://ds.jctech888.com.cn

JavaScript ..... 252
来源：http://ue.szsharing.cn

TypeScript ..... 212
来源：http://nj.nicolike.cn

Java ........... 212
来源：http://bm.lnxyls.cn

Go ............. 212
来源：http://qb.521024.cn

Ruby ........... 212
来源：http://lp.chemitech.net.cn

C# ............. 212
来源：http://oo.bookmarksfly.cn

C .............. 30
来源：http://rb.hnjuh.cn

C++ ............ 30
来源：http://xa.shxzskj.cn

SQL ............ 90
来源：http://yt.asd995.cn

Bash ........... 80
来源：http://mb.bjjhwx.cn

Kotlin ......... 15
来源：http://ky.szxytkj.cn

Swift .......... 15
来源：http://ln.yuexingan06.cn

Lua ............ 10
来源：http://mu.panjiajie.cn

Perl ........... 10
来源：http://ln.shxzukj.cn

Scala .......... 10
来源：http://kd.muxihuayi.cn

------------------------------------
来源：http://on.shxzukj.cn

合计 ........... 2106 条
来源：http://ie.haigaiapp.cn

按章节统计：
来源：http://xu.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ot.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cn.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sd.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iq.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iq.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zm.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ie.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xs.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gh.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fy.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pt.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ft.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zq.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jo.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://za.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mq.lnxyls.cn

Q SQL 专题                              90
来源：http://hs.521024.cn

R Bash 专题                             80
来源：http://ed.panjiajie.cn

S C / C++ 专题                          60
来源：http://yc.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://jp.muxihuayi.cn

U 高频实用片段                         120
来源：http://hz.bookmarksfly.cn

------------------------------------
来源：http://pj.panjiajie.cn

合计                                  2106 条
来源：http://ee.newstarts.cn

--------------------------------------------------------------------------------
来源：http://jr.bookmarksfly.cn

使用提醒
来源：http://ss.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://ii.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ih.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bl.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eh.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://it.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://da.yuntaijiaju.cn

—— 文件结束 ——
来源：http://zz.wgjwhj.cn

================================================================================
来源：http://dz.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://nx.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://dq.huanxung.cn

================================================================================
来源：http://ga.bjjhwx.cn

【收录内容】
来源：http://vy.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mp.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sn.huixiangedu.cn

SQL · Bash · C · C++
来源：http://yz.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://st.huixinmuqiang.cn

【使用说明】
来源：http://nr.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cw.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oy.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mu.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ky.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tx.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wu.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ki.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kv.521024.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bq.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xy.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gs.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kz.szxytkj.cn

【文件统计】
来源：http://rp.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bx.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://fk.shxzskj.cn

目  录
来源：http://bu.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://eu.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rk.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cv.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://py.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fm.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vy.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://af.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mj.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ot.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eo.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gh.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rd.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nm.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://na.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cj.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ld.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fj.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tv.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ck.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pi.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yj.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lc.jctech888.com.cn

================================================================================
来源：http://lm.hahajie.cn

A. 基础语法与类型
来源：http://nd.colortex.cn

================================================================================
来源：http://pp.bookmarksfly.cn

[A01] Hello World
来源：http://eo.nicolike.cn

Py:   print("Hello, World!")
来源：http://de.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://ed.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://yt.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yn.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://kb.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://uq.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://nb.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qs.shxzukj.cn

[A02] 变量声明与赋值
来源：http://sy.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oi.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://st.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ya.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ak.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://vy.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://gm.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://gy.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://es.gzmigu.cn

[A03] 常量定义
来源：http://oe.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cv.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://uk.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://gh.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://ty.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://vc.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://mz.9csxet.cn

Ruby: PI = 3.14159
来源：http://ms.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://wa.huanxung.cn

[A04] 判断变量类型
来源：http://qv.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qv.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qa.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pn.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://re.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ys.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ik.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ew.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://xu.panjiajie.cn

[A05] 整数除法与取模
来源：http://cd.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pd.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vg.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ei.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ie.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://xn.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://os.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://db.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://dd.shxzskj.cn

[A06] 字符串转数字
来源：http://rr.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://nq.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rh.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xx.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pr.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://el.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lg.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rg.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sm.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://ff.wgjwhj.cn

Py:   str(42)
来源：http://dt.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://ue.colortex.cn

JS:   String(42); (42).toString()
来源：http://fj.szxytkj.cn

TS:   String(42)
来源：http://ro.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ic.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://dr.shxzukj.cn

Ruby: 42.to_s
来源：http://hl.szsharing.cn

C#:   42.ToString()
来源：http://fh.szsharing.cn

[A08] 取整与四舍五入
来源：http://fn.chemitech.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lu.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nx.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lj.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ki.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kj.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ut.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ma.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hy.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://sj.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lq.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://od.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gb.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://em.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://um.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oj.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iv.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mz.chemitech.net.cn

[A10] 生成随机数
来源：http://tb.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://fc.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://ba.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ij.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mr.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://ih.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fr.gzmigu.cn

Ruby: rand(1..100)
来源：http://gg.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://kk.newstarts.cn

[A11] 条件表达式（三元）
来源：http://au.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://gy.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sq.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uk.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rg.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://mr.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://la.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bq.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jv.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://wf.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pa.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ye.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://pc.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://la.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://si.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xl.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://mi.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://mg.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zb.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://bp.521024.cn

PHP:  "第一行\n第二行"
来源：http://mg.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://sp.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://qw.gzmigu.cn

Java: "第一行\n第二行"
来源：http://zz.huanxung.cn

Go:   "第一行\n第二行"
来源：http://iy.asd995.cn

Ruby: "第一行\n第二行"
来源：http://oj.nicolike.cn

C#:   "第一行\n第二行"
来源：http://dl.nicolike.cn

[A14] 注释写法
来源：http://gx.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vh.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lw.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://xp.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://ae.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ei.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://uc.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dn.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://of.gzmigu.cn

[A15] 空值判断与默认值
来源：http://kp.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://pf.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://lt.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://mp.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://mn.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xm.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://mq.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://wf.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://zx.huixiangedu.cn

[A16] 真假值判断规则
来源：http://dr.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dn.newstarts.cn


<!-- 参考信息 -->