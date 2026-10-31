代发 wailian999

[U99] JS：事件监听
来源：http://pb.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://tq.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://nn.yuntaijiaju.cn

document.querySelector(".item")
来源：http://iz.asd995.cn

[U101] JS：classList 操作
来源：http://va.szxytkj.cn

el.classList.toggle("active")
来源：http://zy.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://ah.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://is.chemitech.net.cn

[U103] JS：定时器
来源：http://bo.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ni.gzmigu.cn

[U104] JS：防抖
来源：http://rn.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jw.szsharing.cn

[U105] JS：节流
来源：http://wb.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ox.yuexingan06.cn

[U106] JS：日期格式化
来源：http://jx.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nn.chemitech.net.cn

[U107] JS：数字千分位
来源：http://bi.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ik.bookmarksfly.cn

[U108] JS：随机整数
来源：http://qx.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xd.wgjwhj.cn

[U109] JS：数组分组
来源：http://xw.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://ue.yuexingan06.cn

[U110] JS：数组分块
来源：http://kr.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ut.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://fg.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://zb.hahajie.cn

[U112] JS：字符串补位
来源：http://no.shtwfgs.cn

"7".padStart(3, "0")
来源：http://sf.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://eo.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://lt.nszjky.cn

[U114] JS：JSON 深比较
来源：http://mr.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oh.gzmigu.cn

[U115] JS：生成 UUID
来源：http://lq.nszjky.cn

crypto.randomUUID()
来源：http://pn.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://dk.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://ju.nicolike.cn

[U117] JS：单元测试
来源：http://fi.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://wv.bjjhwx.cn

[U118] JS：开发服务器
来源：http://cp.9csxet.cn

npm i -D vite;  npx vite
来源：http://cd.asd995.cn

[U119] JS：生产构建
来源：http://dw.huanxung.cn

npx vite build
来源：http://pz.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://sw.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://nw.colortex.cn

================================================================================
来源：http://ij.asd995.cn

统计汇总
来源：http://dm.hnjuh.cn

================================================================================
来源：http://bq.hnjuh.cn

按语言统计（条）：
来源：http://et.shxzskj.cn

Python ......... 252
来源：http://iw.muxihuayi.cn

PHP ............ 252
来源：http://sy.panjiajie.cn

JavaScript ..... 252
来源：http://gn.hnjuh.cn

TypeScript ..... 212
来源：http://xd.huanxung.cn

Java ........... 212
来源：http://vl.asd995.cn

Go ............. 212
来源：http://xc.jianghongdianzi.cn

Ruby ........... 212
来源：http://bk.hahajie.cn

C# ............. 212
来源：http://qv.newstarts.cn

C .............. 30
来源：http://sw.shtwfgs.cn

C++ ............ 30
来源：http://ar.nicolike.cn

SQL ............ 90
来源：http://ro.huixinmuqiang.cn

Bash ........... 80
来源：http://hh.bookmarksfly.cn

Kotlin ......... 15
来源：http://ia.huixinmuqiang.cn

Swift .......... 15
来源：http://qy.hnjuh.cn

Lua ............ 10
来源：http://ef.shxzukj.cn

Perl ........... 10
来源：http://zt.chemitech.net.cn

Scala .......... 10
来源：http://jz.asd995.cn

------------------------------------
来源：http://bh.521024.cn

合计 ........... 2106 条
来源：http://zo.bookmarksfly.cn

按章节统计：
来源：http://it.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mg.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bi.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pe.bookmarksfly.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ax.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jf.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fh.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://op.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://na.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dk.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bh.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hw.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xg.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sw.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yu.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jw.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dc.huixiangedu.cn

Q SQL 专题                              90
来源：http://bp.muxihuayi.cn

R Bash 专题                             80
来源：http://ol.szxytkj.cn

S C / C++ 专题                          60
来源：http://ea.szxytkj.cn

T 其他语言补充                          60
来源：http://gh.wgjwhj.cn

U 高频实用片段                         120
来源：http://us.panjiajie.cn

------------------------------------
来源：http://iu.szsharing.cn

合计                                  2106 条
来源：http://uw.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://et.huixiangedu.cn

使用提醒
来源：http://gc.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ep.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ai.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lr.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fy.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pb.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://in.newstarts.cn

—— 文件结束 ——
来源：http://yq.jianghongdianzi.cn

================================================================================
来源：http://ab.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://bl.9csxet.cn

Common Programming Examples Cheat Book
来源：http://ua.szsharing.cn

================================================================================
来源：http://ya.huanxung.cn

【收录内容】
来源：http://ko.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vk.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mr.colortex.cn

SQL · Bash · C · C++
来源：http://xa.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hc.gzmigu.cn

【使用说明】
来源：http://ro.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://od.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jj.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pw.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pf.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://du.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kc.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ao.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sq.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://od.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://co.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mu.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uo.hahajie.cn

【文件统计】
来源：http://bc.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uf.colortex.cn

--------------------------------------------------------------------------------
来源：http://vc.wgjwhj.cn

目  录
来源：http://yi.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://en.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nr.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bu.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zj.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mo.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://am.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://im.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uq.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dl.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://my.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jm.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iq.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ws.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xy.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dq.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://np.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yx.nicolike.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://le.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://px.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://om.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ju.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wp.nszjky.cn

================================================================================
来源：http://nf.jctech888.com.cn

A. 基础语法与类型
来源：http://yr.wgjwhj.cn

================================================================================
来源：http://xq.shxzukj.cn

[A01] Hello World
来源：http://xq.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://di.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://ac.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://hx.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bs.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://au.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://uc.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://bk.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hm.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://js.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uk.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ie.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qr.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dx.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://te.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://yt.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://gq.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ew.haigaiapp.cn

[A03] 常量定义
来源：http://sd.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tp.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://yn.asd995.cn

JS:   const PI = 3.14159;
来源：http://hc.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://tt.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://uf.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://cu.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://wk.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://ao.shxzskj.cn

[A04] 判断变量类型
来源：http://yh.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tc.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xq.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wp.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://av.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hw.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tk.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ud.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://fy.colortex.cn

[A05] 整数除法与取模
来源：http://am.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ym.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fo.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cz.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sp.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://ye.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://wm.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://jv.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://aa.521024.cn

[A06] 字符串转数字
来源：http://ge.asd995.cn

Py:   int("42"); float("3.14")
来源：http://pq.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oi.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ij.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ch.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tn.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wm.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zk.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jv.9csxet.cn

[A07] 数字转字符串
来源：http://ei.yuntaijiaju.cn

Py:   str(42)
来源：http://st.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://fp.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://pv.huixiangedu.cn

TS:   String(42)
来源：http://up.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://go.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://xd.shtwfgs.cn

Ruby: 42.to_s
来源：http://ij.szsharing.cn

C#:   42.ToString()
来源：http://xk.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://di.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vn.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xg.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vs.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pq.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://im.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wv.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ee.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://am.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ie.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qi.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ro.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ar.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rj.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://op.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ut.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gv.huixiangedu.cn

[A10] 生成随机数
来源：http://xf.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://bl.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://dl.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wb.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jh.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://bx.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gn.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://rl.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://tt.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://fb.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://oq.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yy.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zu.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gt.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://tk.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://km.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dt.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ea.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://fk.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jb.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://db.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://hz.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://cw.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://ul.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lh.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://ij.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://mv.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fm.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://wp.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://xg.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://aj.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://yq.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://dn.newstarts.cn

Go:   "第一行\n第二行"
来源：http://tu.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://ys.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://cm.panjiajie.cn

[A14] 注释写法
来源：http://ww.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cv.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pk.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://gj.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://sr.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fh.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://bp.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fo.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://iz.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://hd.gzmigu.cn

Py:   value = data or "默认值"
来源：http://mp.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://rg.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://gs.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://pt.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xg.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://fe.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://mg.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://cw.chemitech.net.cn

[A16] 真假值判断规则
来源：http://iw.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qd.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sm.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eb.colortex.cn

TS:   if (!x) {}
来源：http://fe.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fj.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ef.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sy.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ds.szxytkj.cn

[A17] 位运算
来源：http://tp.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sd.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lv.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dm.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vu.shxzukj.cn


<!-- 参考信息 -->