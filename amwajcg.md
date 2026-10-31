代发 wailian999

[U95] JS：Promise 包装
来源：http://hl.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://sg.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://dw.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ka.wgjwhj.cn

[U97] JS：并发请求
来源：http://fd.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xn.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://yt.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ib.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://rf.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://gw.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://jb.shxzskj.cn

document.querySelector(".item")
来源：http://jv.hahajie.cn

[U101] JS：classList 操作
来源：http://fx.panjiajie.cn

el.classList.toggle("active")
来源：http://gp.muxihuayi.cn

[U102] JS：本地存储
来源：http://lo.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ra.asd995.cn

[U103] JS：定时器
来源：http://gt.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ss.asd995.cn

[U104] JS：防抖
来源：http://bn.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://if.lnxyls.cn

[U105] JS：节流
来源：http://wi.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ar.wgjwhj.cn

[U106] JS：日期格式化
来源：http://is.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qe.asd995.cn

[U107] JS：数字千分位
来源：http://er.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wq.wgjwhj.cn

[U108] JS：随机整数
来源：http://qs.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fr.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://ic.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://rz.wgjwhj.cn

[U110] JS：数组分块
来源：http://xl.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dx.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://mw.hahajie.cn

new Map(Object.entries(obj))
来源：http://up.shxzskj.cn

[U112] JS：字符串补位
来源：http://lp.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://he.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://js.9csxet.cn

s.replaceAll("a", "b")
来源：http://sx.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://ww.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ug.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://pu.bjjhwx.cn

crypto.randomUUID()
来源：http://so.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://bm.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://mb.szsharing.cn

[U117] JS：单元测试
来源：http://ki.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://rz.szsharing.cn

[U118] JS：开发服务器
来源：http://eu.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://jf.shxzukj.cn

[U119] JS：生产构建
来源：http://jo.muxihuayi.cn

npx vite build
来源：http://fq.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://ne.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://io.shxzukj.cn

================================================================================
来源：http://kf.hahajie.cn

统计汇总
来源：http://pi.shtwfgs.cn

================================================================================
来源：http://eu.lnxyls.cn

按语言统计（条）：
来源：http://ya.panjiajie.cn

Python ......... 252
来源：http://bm.muxihuayi.cn

PHP ............ 252
来源：http://dn.newstarts.cn

JavaScript ..... 252
来源：http://qz.huixiangedu.cn

TypeScript ..... 212
来源：http://ll.shxzukj.cn

Java ........... 212
来源：http://lc.yuntaijiaju.cn

Go ............. 212
来源：http://es.gzmigu.cn

Ruby ........... 212
来源：http://tr.lnxyls.cn

C# ............. 212
来源：http://ck.lnxyls.cn

C .............. 30
来源：http://ek.huixiangedu.cn

C++ ............ 30
来源：http://xp.jianghongdianzi.cn

SQL ............ 90
来源：http://hs.haigaiapp.cn

Bash ........... 80
来源：http://mk.shtwfgs.cn

Kotlin ......... 15
来源：http://lr.panjiajie.cn

Swift .......... 15
来源：http://jy.shxzskj.cn

Lua ............ 10
来源：http://vq.wgjwhj.cn

Perl ........... 10
来源：http://vs.lnxyls.cn

Scala .......... 10
来源：http://sj.huixinmuqiang.cn

------------------------------------
来源：http://mb.521024.cn

合计 ........... 2106 条
来源：http://ck.panjiajie.cn

按章节统计：
来源：http://jh.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pc.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bk.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lh.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iq.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zw.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cq.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xm.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fk.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xl.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zn.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lc.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pu.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jz.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dp.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zz.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tp.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://nt.newstarts.cn

R Bash 专题                             80
来源：http://qo.szxytkj.cn

S C / C++ 专题                          60
来源：http://qe.asd995.cn

T 其他语言补充                          60
来源：http://vg.muxihuayi.cn

U 高频实用片段                         120
来源：http://ak.bjjhwx.cn

------------------------------------
来源：http://cb.yuexingan06.cn

合计                                  2106 条
来源：http://hg.huanxung.cn

--------------------------------------------------------------------------------
来源：http://bm.muxihuayi.cn

使用提醒
来源：http://vp.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ih.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hl.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ub.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pn.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zg.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ma.hnjuh.cn

—— 文件结束 ——
来源：http://rq.9csxet.cn

================================================================================
来源：http://im.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://ue.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://zk.hnjuh.cn

================================================================================
来源：http://ug.szxytkj.cn

【收录内容】
来源：http://rk.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wc.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mw.9csxet.cn

SQL · Bash · C · C++
来源：http://oe.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ah.lnxyls.cn

【使用说明】
来源：http://ms.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zv.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ap.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://db.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ea.yuntaijiaju.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fk.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hw.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yo.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ax.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aq.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vu.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bd.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ah.chemitech.net.cn

【文件统计】
来源：http://qa.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jf.szsharing.cn

--------------------------------------------------------------------------------
来源：http://jz.haigaiapp.cn

目  录
来源：http://lu.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://hh.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cu.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wj.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jw.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://go.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pf.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://er.shxzukj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sv.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tn.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sk.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ed.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pv.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zq.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ao.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wz.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gw.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ea.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xg.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yz.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ct.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xr.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ug.hnjuh.cn

================================================================================
来源：http://yp.jctech888.com.cn

A. 基础语法与类型
来源：http://st.521024.cn

================================================================================
来源：http://uw.yuntaijiaju.cn

[A01] Hello World
来源：http://on.hahajie.cn

Py:   print("Hello, World!")
来源：http://cf.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://th.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://mf.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jp.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://mi.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://mc.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://hb.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sj.colortex.cn

[A02] 变量声明与赋值
来源：http://jc.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://il.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://no.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yn.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ye.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://fa.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://rr.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://qd.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://th.jctech888.com.cn

[A03] 常量定义
来源：http://sf.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gd.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://fs.asd995.cn

JS:   const PI = 3.14159;
来源：http://wh.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://ex.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://in.hahajie.cn

Go:   const PI = 3.14159
来源：http://ss.huanxung.cn

Ruby: PI = 3.14159
来源：http://nl.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://tv.colortex.cn

[A04] 判断变量类型
来源：http://ux.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ml.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xi.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xe.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://dg.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ch.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ft.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wf.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://xf.9csxet.cn

[A05] 整数除法与取模
来源：http://sb.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vr.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vg.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ut.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dz.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://fy.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://ty.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://jk.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://qe.colortex.cn

[A06] 字符串转数字
来源：http://kh.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://gy.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zv.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cg.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ir.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oa.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yc.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hw.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pd.panjiajie.cn

[A07] 数字转字符串
来源：http://ev.jctech888.com.cn

Py:   str(42)
来源：http://ns.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://xf.huanxung.cn

JS:   String(42); (42).toString()
来源：http://zp.panjiajie.cn

TS:   String(42)
来源：http://xn.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ru.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://hv.muxihuayi.cn

Ruby: 42.to_s
来源：http://yd.asd995.cn

C#:   42.ToString()
来源：http://jv.gzmigu.cn

[A08] 取整与四舍五入
来源：http://sn.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pp.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xu.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ce.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kh.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fs.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zc.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lh.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gf.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://nl.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lx.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qu.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kh.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nu.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ne.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pq.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rp.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wl.muxihuayi.cn

[A10] 生成随机数
来源：http://hj.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://kl.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://pm.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://np.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uz.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://oq.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gi.hnjuh.cn

Ruby: rand(1..100)
来源：http://fk.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://mm.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://tw.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ix.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vc.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sh.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pk.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://nn.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pt.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://js.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ke.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://cz.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mf.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ir.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://zq.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://oq.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://op.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sn.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://gk.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://zd.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fu.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://ge.colortex.cn

PHP:  "第一行\n第二行"
来源：http://tg.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://bq.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://uh.szsharing.cn

Java: "第一行\n第二行"
来源：http://fq.nicolike.cn

Go:   "第一行\n第二行"
来源：http://vr.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://gw.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://qf.chemitech.net.cn

[A14] 注释写法
来源：http://zn.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yq.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ob.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://yd.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://ah.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yr.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://eh.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mm.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://bs.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://mr.asd995.cn

Py:   value = data or "默认值"
来源：http://qy.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://ov.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://lj.521024.cn

TS:   const value = data ?? "默认值";
来源：http://yb.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fw.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://or.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://is.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://lo.hahajie.cn

[A16] 真假值判断规则
来源：http://hh.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tu.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://um.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://us.jctech888.com.cn

TS:   if (!x) {}
来源：http://fs.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://du.szsharing.cn


<!-- 参考信息 -->