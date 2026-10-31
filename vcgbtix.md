代发 wailian999

[U95] JS：Promise 包装
来源：http://zq.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://yx.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://eo.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zs.szxytkj.cn

[U97] JS：并发请求
来源：http://ci.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ot.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://av.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pf.hahajie.cn

[U99] JS：事件监听
来源：http://mb.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://ia.shxzskj.cn

[U100] JS：DOM 查询
来源：http://cg.newstarts.cn

document.querySelector(".item")
来源：http://rd.wgjwhj.cn

[U101] JS：classList 操作
来源：http://cd.shtwfgs.cn

el.classList.toggle("active")
来源：http://bi.colortex.cn

[U102] JS：本地存储
来源：http://mb.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jp.jianghongdianzi.cn

[U103] JS：定时器
来源：http://we.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vn.newstarts.cn

[U104] JS：防抖
来源：http://bz.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gb.521024.cn

[U105] JS：节流
来源：http://in.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jj.nszjky.cn

[U106] JS：日期格式化
来源：http://ub.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ns.szxytkj.cn

[U107] JS：数字千分位
来源：http://ad.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lq.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://fn.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gg.shxzskj.cn

[U109] JS：数组分组
来源：http://bg.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://eh.newstarts.cn

[U110] JS：数组分块
来源：http://zy.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uw.gzmigu.cn

[U111] JS：对象转 Map
来源：http://ha.hahajie.cn

new Map(Object.entries(obj))
来源：http://az.chemitech.net.cn

[U112] JS：字符串补位
来源：http://nc.chemitech.net.cn

"7".padStart(3, "0")
来源：http://ut.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://dm.nicolike.cn

s.replaceAll("a", "b")
来源：http://xi.9csxet.cn

[U114] JS：JSON 深比较
来源：http://kh.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hp.szsharing.cn

[U115] JS：生成 UUID
来源：http://mr.asd995.cn

crypto.randomUUID()
来源：http://ju.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://lr.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://aj.huanxung.cn

[U117] JS：单元测试
来源：http://wy.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://rb.szxytkj.cn

[U118] JS：开发服务器
来源：http://ls.nicolike.cn

npm i -D vite;  npx vite
来源：http://ho.shxzskj.cn

[U119] JS：生产构建
来源：http://ad.nicolike.cn

npx vite build
来源：http://to.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://bk.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://qs.lnxyls.cn

================================================================================
来源：http://cc.9csxet.cn

统计汇总
来源：http://hi.shtwfgs.cn

================================================================================
来源：http://rs.panjiajie.cn

按语言统计（条）：
来源：http://bb.nicolike.cn

Python ......... 252
来源：http://pc.wgjwhj.cn

PHP ............ 252
来源：http://no.wgjwhj.cn

JavaScript ..... 252
来源：http://ok.huixinmuqiang.cn

TypeScript ..... 212
来源：http://wv.huixiangedu.cn

Java ........... 212
来源：http://nc.newstarts.cn

Go ............. 212
来源：http://bf.muxihuayi.cn

Ruby ........... 212
来源：http://ql.yuntaijiaju.cn

C# ............. 212
来源：http://yq.521024.cn

C .............. 30
来源：http://eh.huixinmuqiang.cn

C++ ............ 30
来源：http://is.panjiajie.cn

SQL ............ 90
来源：http://fy.521024.cn

Bash ........... 80
来源：http://ev.newstarts.cn

Kotlin ......... 15
来源：http://io.bjjhwx.cn

Swift .......... 15
来源：http://qf.9csxet.cn

Lua ............ 10
来源：http://xx.huixinmuqiang.cn

Perl ........... 10
来源：http://fd.huixinmuqiang.cn

Scala .......... 10
来源：http://ff.521024.cn

------------------------------------
来源：http://xn.szxytkj.cn

合计 ........... 2106 条
来源：http://na.shxzukj.cn

按章节统计：
来源：http://sr.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fm.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ou.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rc.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://py.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yy.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ie.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fm.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yt.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yb.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fj.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ll.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ra.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zh.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tw.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yy.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tn.panjiajie.cn

Q SQL 专题                              90
来源：http://en.nicolike.cn

R Bash 专题                             80
来源：http://zi.lnxyls.cn

S C / C++ 专题                          60
来源：http://xk.huanxung.cn

T 其他语言补充                          60
来源：http://jj.szsharing.cn

U 高频实用片段                         120
来源：http://df.muxihuayi.cn

------------------------------------
来源：http://lz.shxzukj.cn

合计                                  2106 条
来源：http://ef.521024.cn

--------------------------------------------------------------------------------
来源：http://ye.jianghongdianzi.cn

使用提醒
来源：http://sx.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://en.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xz.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jp.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rn.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xv.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nt.9csxet.cn

—— 文件结束 ——
来源：http://js.521024.cn

================================================================================
来源：http://dk.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://kz.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://im.9csxet.cn

================================================================================
来源：http://gn.asd995.cn

【收录内容】
来源：http://ba.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pq.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://io.yuexingan06.cn

SQL · Bash · C · C++
来源：http://sz.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uh.chemitech.net.cn

【使用说明】
来源：http://ea.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gy.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sy.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://px.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wv.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kj.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ui.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://db.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://im.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ib.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zt.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://td.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bw.yuntaijiaju.cn

【文件统计】
来源：http://qz.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mv.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://gq.nszjky.cn

目  录
来源：http://wo.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ek.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cy.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iv.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sh.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lz.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://an.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uh.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ya.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zo.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gx.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fz.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://po.shxzskj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qp.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aq.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nk.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qm.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mx.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vq.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mt.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://av.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ja.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vq.521024.cn

================================================================================
来源：http://zg.huixiangedu.cn

A. 基础语法与类型
来源：http://wx.huixinmuqiang.cn

================================================================================
来源：http://hs.panjiajie.cn

[A01] Hello World
来源：http://nl.hahajie.cn

Py:   print("Hello, World!")
来源：http://zn.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://nj.colortex.cn

JS:   console.log("Hello, World!");
来源：http://an.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dr.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://sf.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://ou.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://gg.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://it.hahajie.cn

[A02] 变量声明与赋值
来源：http://hc.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kd.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://li.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ph.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lq.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://zs.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://ry.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://el.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vf.yuntaijiaju.cn

[A03] 常量定义
来源：http://kx.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lw.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://ad.newstarts.cn

JS:   const PI = 3.14159;
来源：http://rw.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://zp.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://cp.hnjuh.cn

Go:   const PI = 3.14159
来源：http://zc.shxzukj.cn

Ruby: PI = 3.14159
来源：http://rz.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://qf.newstarts.cn

[A04] 判断变量类型
来源：http://oo.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ho.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jg.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ur.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://gt.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dm.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gy.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kd.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://oz.hnjuh.cn

[A05] 整数除法与取模
来源：http://aw.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ak.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vj.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wk.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bs.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://uz.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://ak.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://rd.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://lu.panjiajie.cn

[A06] 字符串转数字
来源：http://gg.521024.cn

Py:   int("42"); float("3.14")
来源：http://td.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gh.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fq.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hm.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nl.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cr.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dd.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pn.panjiajie.cn

[A07] 数字转字符串
来源：http://ub.muxihuayi.cn

Py:   str(42)
来源：http://gy.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://tf.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://vl.chemitech.net.cn

TS:   String(42)
来源：http://jw.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ny.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://ld.nicolike.cn

Ruby: 42.to_s
来源：http://bg.yuntaijiaju.cn

C#:   42.ToString()
来源：http://kl.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://lf.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mj.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fi.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ho.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aj.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://aa.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yo.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cb.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://py.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://gn.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yh.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://en.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://op.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nx.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://if.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ga.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jc.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nx.szsharing.cn

[A10] 生成随机数
来源：http://wp.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://gp.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://gm.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sy.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cv.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://jc.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vu.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://ej.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://or.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://if.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://pp.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ih.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nu.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rh.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://oy.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lc.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bj.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pr.521024.cn

[A12] 字符串插值 / 格式化
来源：http://os.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zd.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oh.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://gs.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://os.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://nu.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qx.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://la.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://xe.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xt.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://rz.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://ga.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://nw.9csxet.cn

TS:   "第一行\n第二行"
来源：http://ik.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://sn.asd995.cn

Go:   "第一行\n第二行"
来源：http://sb.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://iv.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://az.nicolike.cn

[A14] 注释写法
来源：http://vb.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tl.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dj.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://bn.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://dm.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kd.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://nm.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wz.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://zy.colortex.cn

[A15] 空值判断与默认值
来源：http://xi.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://xu.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://yq.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://qu.521024.cn

TS:   const value = data ?? "默认值";
来源：http://ch.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ui.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://zj.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://xf.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://ya.szxytkj.cn

[A16] 真假值判断规则
来源：http://if.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hl.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ds.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yw.shxzskj.cn

TS:   if (!x) {}
来源：http://gp.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qs.nszjky.cn


<!-- 参考信息 -->