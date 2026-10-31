代发 wailian999

[U93] JS：模板字符串
来源：http://yb.colortex.cn

`共 ${n} 条`
来源：http://cj.panjiajie.cn

[U94] JS：箭头函数
来源：http://sa.huanxung.cn

const double = x => x * 2;
来源：http://sq.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://iq.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://dr.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://je.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mj.colortex.cn

[U97] JS：并发请求
来源：http://eb.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fh.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://ih.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zj.nszjky.cn

[U99] JS：事件监听
来源：http://hn.huanxung.cn

el.addEventListener("click", e => {})
来源：http://sd.nszjky.cn

[U100] JS：DOM 查询
来源：http://if.jctech888.com.cn

document.querySelector(".item")
来源：http://vr.newstarts.cn

[U101] JS：classList 操作
来源：http://ai.colortex.cn

el.classList.toggle("active")
来源：http://of.shxzukj.cn

[U102] JS：本地存储
来源：http://tg.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pl.yuexingan06.cn

[U103] JS：定时器
来源：http://wu.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eq.huixinmuqiang.cn

[U104] JS：防抖
来源：http://tl.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wd.colortex.cn

[U105] JS：节流
来源：http://wc.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gj.hahajie.cn

[U106] JS：日期格式化
来源：http://ms.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ve.huanxung.cn

[U107] JS：数字千分位
来源：http://ns.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ed.szxytkj.cn

[U108] JS：随机整数
来源：http://ng.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ae.szsharing.cn

[U109] JS：数组分组
来源：http://kx.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://dy.shxzskj.cn

[U110] JS：数组分块
来源：http://ce.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://io.newstarts.cn

[U111] JS：对象转 Map
来源：http://ci.9csxet.cn

new Map(Object.entries(obj))
来源：http://fk.panjiajie.cn

[U112] JS：字符串补位
来源：http://zj.yuexingan06.cn

"7".padStart(3, "0")
来源：http://un.huanxung.cn

[U113] JS：正则替换全部
来源：http://yo.panjiajie.cn

s.replaceAll("a", "b")
来源：http://mj.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://ny.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tc.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://uf.chemitech.net.cn

crypto.randomUUID()
来源：http://ba.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://mu.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://tu.szxytkj.cn

[U117] JS：单元测试
来源：http://vf.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://de.szxytkj.cn

[U118] JS：开发服务器
来源：http://te.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://xa.muxihuayi.cn

[U119] JS：生产构建
来源：http://sc.hnjuh.cn

npx vite build
来源：http://mi.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://cw.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://ge.nicolike.cn

================================================================================
来源：http://ru.9csxet.cn

统计汇总
来源：http://sw.newstarts.cn

================================================================================
来源：http://xg.haigaiapp.cn

按语言统计（条）：
来源：http://ow.newstarts.cn

Python ......... 252
来源：http://gr.szsharing.cn

PHP ............ 252
来源：http://dx.hahajie.cn

JavaScript ..... 252
来源：http://ae.haigaiapp.cn

TypeScript ..... 212
来源：http://rx.521024.cn

Java ........... 212
来源：http://pr.panjiajie.cn

Go ............. 212
来源：http://ii.521024.cn

Ruby ........... 212
来源：http://ki.9csxet.cn

C# ............. 212
来源：http://jb.szxytkj.cn

C .............. 30
来源：http://ks.colortex.cn

C++ ............ 30
来源：http://lf.szsharing.cn

SQL ............ 90
来源：http://sv.muxihuayi.cn

Bash ........... 80
来源：http://ji.nszjky.cn

Kotlin ......... 15
来源：http://em.szsharing.cn

Swift .......... 15
来源：http://ne.huixiangedu.cn

Lua ............ 10
来源：http://vc.yuexingan06.cn

Perl ........... 10
来源：http://bl.huixiangedu.cn

Scala .......... 10
来源：http://ea.9csxet.cn

------------------------------------
来源：http://oa.muxihuayi.cn

合计 ........... 2106 条
来源：http://wv.jctech888.com.cn

按章节统计：
来源：http://rx.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nb.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tx.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ig.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ax.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rp.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kr.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vk.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ba.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ro.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vg.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cz.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ya.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mh.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pf.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://to.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dm.newstarts.cn

Q SQL 专题                              90
来源：http://zi.colortex.cn

R Bash 专题                             80
来源：http://hz.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://qs.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://tb.jctech888.com.cn

U 高频实用片段                         120
来源：http://xq.hnjuh.cn

------------------------------------
来源：http://ah.gzmigu.cn

合计                                  2106 条
来源：http://ip.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://uk.huixinmuqiang.cn

使用提醒
来源：http://np.hahajie.cn

--------------------------------------------------------------------------------
来源：http://np.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cz.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zs.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sx.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ad.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uv.hnjuh.cn

—— 文件结束 ——
来源：http://pf.chemitech.net.cn

================================================================================
来源：http://jh.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://yu.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://on.wgjwhj.cn

================================================================================
来源：http://ju.panjiajie.cn

【收录内容】
来源：http://dt.shxzukj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oo.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mo.bjjhwx.cn

SQL · Bash · C · C++
来源：http://ah.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uv.newstarts.cn

【使用说明】
来源：http://wu.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xm.yuntaijiaju.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ke.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://db.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sl.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ek.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rt.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rc.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ed.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tf.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ni.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ge.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ik.szxytkj.cn

【文件统计】
来源：http://rj.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ve.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://us.bjjhwx.cn

目  录
来源：http://wr.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://qt.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cl.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hj.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pk.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fu.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vc.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ux.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://in.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ae.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vr.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ph.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uf.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xz.chemitech.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ou.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cd.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tw.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ed.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://eo.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zm.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qa.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://je.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sp.nicolike.cn

================================================================================
来源：http://tt.szxytkj.cn

A. 基础语法与类型
来源：http://xd.huixiangedu.cn

================================================================================
来源：http://zy.hahajie.cn

[A01] Hello World
来源：http://up.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://qs.asd995.cn

PHP:  echo "Hello, World!";
来源：http://bw.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://gk.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sh.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://wq.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://av.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://hv.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ko.szsharing.cn

[A02] 变量声明与赋值
来源：http://ti.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bt.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oc.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oz.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iz.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://im.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://oi.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://ae.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ef.jctech888.com.cn

[A03] 常量定义
来源：http://ab.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qn.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://dh.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://rb.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://ea.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://ko.asd995.cn

Go:   const PI = 3.14159
来源：http://cz.szsharing.cn

Ruby: PI = 3.14159
来源：http://df.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://gu.bookmarksfly.cn

[A04] 判断变量类型
来源：http://nu.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uk.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kz.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jw.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://jl.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bn.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yg.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ne.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://js.szsharing.cn

[A05] 整数除法与取模
来源：http://ba.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xp.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xh.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ef.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vi.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://bk.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://nd.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://iq.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://bg.nszjky.cn

[A06] 字符串转数字
来源：http://lj.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://ra.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://og.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gt.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ca.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ew.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mz.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ap.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uo.huanxung.cn

[A07] 数字转字符串
来源：http://ex.huixiangedu.cn

Py:   str(42)
来源：http://tx.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://sg.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://xr.huanxung.cn

TS:   String(42)
来源：http://ts.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eu.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://qm.nicolike.cn

Ruby: 42.to_s
来源：http://ht.bjjhwx.cn

C#:   42.ToString()
来源：http://hn.szsharing.cn

[A08] 取整与四舍五入
来源：http://rg.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://go.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ip.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ba.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cx.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://en.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fr.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://iz.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bz.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://qf.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hp.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://av.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vu.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rt.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ev.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nf.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vk.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://re.nszjky.cn

[A10] 生成随机数
来源：http://tb.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://de.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://ne.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ng.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ns.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://ib.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ug.haigaiapp.cn

Ruby: rand(1..100)
来源：http://qx.521024.cn

C#:   new Random().Next(1, 101)
来源：http://ac.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://mv.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://ar.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rd.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tq.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jw.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://yi.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xi.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jh.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://aa.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://si.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://li.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pm.colortex.cn

JS:   `Hello, ${name}!`
来源：http://dn.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://iw.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://io.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sr.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://il.asd995.cn

C#:   $"Hello, {name}!"
来源：http://gb.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lt.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://zk.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://qm.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://zt.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://ry.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://xd.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://yz.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://xz.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://ka.yuntaijiaju.cn

[A14] 注释写法
来源：http://pp.hnjuh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lz.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sr.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://ml.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://na.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wp.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://qd.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uk.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://gv.hahajie.cn

[A15] 空值判断与默认值
来源：http://kl.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://fw.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://go.521024.cn

JS:   const value = data ?? "默认值";
来源：http://zq.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://jy.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ap.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://gf.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://kn.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://ar.huixiangedu.cn

[A16] 真假值判断规则
来源：http://kp.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hu.asd995.cn


<!-- 参考信息 -->