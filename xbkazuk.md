代发 wailian999

[U99] JS：事件监听
来源：http://eg.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://xh.9csxet.cn

[U100] JS：DOM 查询
来源：http://fz.asd995.cn

document.querySelector(".item")
来源：http://nn.szxytkj.cn

[U101] JS：classList 操作
来源：http://sf.nicolike.cn

el.classList.toggle("active")
来源：http://te.shtwfgs.cn

[U102] JS：本地存储
来源：http://if.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uo.yuexingan06.cn

[U103] JS：定时器
来源：http://vo.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iy.521024.cn

[U104] JS：防抖
来源：http://sg.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kg.shxzskj.cn

[U105] JS：节流
来源：http://ac.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zp.chemitech.net.cn

[U106] JS：日期格式化
来源：http://ia.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kq.hnjuh.cn

[U107] JS：数字千分位
来源：http://no.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gf.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://nh.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hh.chemitech.net.cn

[U109] JS：数组分组
来源：http://uz.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://yr.9csxet.cn

[U110] JS：数组分块
来源：http://sg.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gt.shxzukj.cn

[U111] JS：对象转 Map
来源：http://ko.colortex.cn

new Map(Object.entries(obj))
来源：http://fd.asd995.cn

[U112] JS：字符串补位
来源：http://ob.haigaiapp.cn

"7".padStart(3, "0")
来源：http://yi.asd995.cn

[U113] JS：正则替换全部
来源：http://hb.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://bc.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://za.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rs.asd995.cn

[U115] JS：生成 UUID
来源：http://ve.wgjwhj.cn

crypto.randomUUID()
来源：http://zp.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://tv.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://rx.muxihuayi.cn

[U117] JS：单元测试
来源：http://ns.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://rd.panjiajie.cn

[U118] JS：开发服务器
来源：http://rl.nicolike.cn

npm i -D vite;  npx vite
来源：http://ro.haigaiapp.cn

[U119] JS：生产构建
来源：http://se.hahajie.cn

npx vite build
来源：http://cd.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://zj.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://lj.bookmarksfly.cn

================================================================================
来源：http://hn.shtwfgs.cn

统计汇总
来源：http://uz.panjiajie.cn

================================================================================
来源：http://de.muxihuayi.cn

按语言统计（条）：
来源：http://li.yuexingan06.cn

Python ......... 252
来源：http://nu.yuntaijiaju.cn

PHP ............ 252
来源：http://hc.nszjky.cn

JavaScript ..... 252
来源：http://qt.panjiajie.cn

TypeScript ..... 212
来源：http://it.huixinmuqiang.cn

Java ........... 212
来源：http://ot.yuexingan06.cn

Go ............. 212
来源：http://eg.nicolike.cn

Ruby ........... 212
来源：http://oo.yuexingan06.cn

C# ............. 212
来源：http://yt.muxihuayi.cn

C .............. 30
来源：http://lh.panjiajie.cn

C++ ............ 30
来源：http://cm.lnxyls.cn

SQL ............ 90
来源：http://oo.yuntaijiaju.cn

Bash ........... 80
来源：http://vf.huixiangedu.cn

Kotlin ......... 15
来源：http://gt.shxzskj.cn

Swift .......... 15
来源：http://nd.shxzukj.cn

Lua ............ 10
来源：http://zr.panjiajie.cn

Perl ........... 10
来源：http://uw.gzmigu.cn

Scala .......... 10
来源：http://fq.shxzskj.cn

------------------------------------
来源：http://hu.9csxet.cn

合计 ........... 2106 条
来源：http://oz.yuntaijiaju.cn

按章节统计：
来源：http://hb.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tz.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zx.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vc.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ie.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jm.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eb.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hu.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vh.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pb.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qf.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://js.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qk.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://op.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xe.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nm.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ya.yuexingan06.cn

Q SQL 专题                              90
来源：http://tf.chemitech.net.cn

R Bash 专题                             80
来源：http://jh.panjiajie.cn

S C / C++ 专题                          60
来源：http://oq.colortex.cn

T 其他语言补充                          60
来源：http://vh.chemitech.net.cn

U 高频实用片段                         120
来源：http://mv.521024.cn

------------------------------------
来源：http://mu.nicolike.cn

合计                                  2106 条
来源：http://lv.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://ds.newstarts.cn

使用提醒
来源：http://at.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://pi.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xp.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ol.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lg.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xw.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ps.colortex.cn

—— 文件结束 ——
来源：http://qc.521024.cn

================================================================================
来源：http://zh.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://tm.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://kt.shxzukj.cn

================================================================================
来源：http://na.huixiangedu.cn

【收录内容】
来源：http://qd.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dz.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qw.hnjuh.cn

SQL · Bash · C · C++
来源：http://zd.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ac.szxytkj.cn

【使用说明】
来源：http://hg.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ad.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bs.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pt.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://au.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tl.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dl.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tw.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gj.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ak.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pm.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kt.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://au.9csxet.cn

【文件统计】
来源：http://gh.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yd.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ur.lnxyls.cn

目  录
来源：http://xm.nszjky.cn

--------------------------------------------------------------------------------
来源：http://wu.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ot.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oe.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zd.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zd.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ye.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kj.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://is.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sa.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ri.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ld.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bs.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dn.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nw.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yw.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ok.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gy.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kf.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gi.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://en.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://im.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://su.jctech888.com.cn

================================================================================
来源：http://ii.wgjwhj.cn

A. 基础语法与类型
来源：http://so.nicolike.cn

================================================================================
来源：http://ko.yuexingan06.cn

[A01] Hello World
来源：http://qd.shxzukj.cn

Py:   print("Hello, World!")
来源：http://ry.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://jj.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://yo.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nk.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://xt.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://xc.shxzskj.cn

Ruby: puts "Hello, World!"
来源：http://rn.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hq.521024.cn

[A02] 变量声明与赋值
来源：http://tv.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hj.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ys.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xm.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wd.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://sk.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://bo.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://an.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ld.szxytkj.cn

[A03] 常量定义
来源：http://tz.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vf.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://ik.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://hd.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://bt.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://rt.521024.cn

Go:   const PI = 3.14159
来源：http://am.muxihuayi.cn

Ruby: PI = 3.14159
来源：http://wk.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://ak.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://oz.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cz.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xr.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mo.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://ah.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sb.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vt.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bf.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://vm.wgjwhj.cn

[A05] 整数除法与取模
来源：http://gd.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xh.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yy.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ch.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kl.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://nt.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://ug.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://ia.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://mt.shtwfgs.cn

[A06] 字符串转数字
来源：http://oo.521024.cn

Py:   int("42"); float("3.14")
来源：http://pe.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://af.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rv.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fu.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oy.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mu.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rn.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tb.lnxyls.cn

[A07] 数字转字符串
来源：http://nx.haigaiapp.cn

Py:   str(42)
来源：http://fw.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://yo.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://wn.lnxyls.cn

TS:   String(42)
来源：http://dn.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gx.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://yd.lnxyls.cn

Ruby: 42.to_s
来源：http://re.hahajie.cn

C#:   42.ToString()
来源：http://ai.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://rd.jianghongdianzi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xh.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gi.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dp.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://su.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ir.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jz.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bc.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cl.colortex.cn

[A09] 绝对值与最大最小值
来源：http://cf.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ru.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hq.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tf.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ld.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gz.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mg.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cx.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ly.huixinmuqiang.cn

[A10] 生成随机数
来源：http://zg.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://re.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://pq.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kr.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ah.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://bo.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tr.huixiangedu.cn

Ruby: rand(1..100)
来源：http://nz.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://xg.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://uq.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ix.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lh.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uk.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qe.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://tm.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ui.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lp.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ea.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://zq.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uw.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jl.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://ea.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://ra.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://si.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yn.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://uq.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://fv.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yd.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://gc.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://ht.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://ai.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://tk.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://zh.szsharing.cn

Go:   "第一行\n第二行"
来源：http://gc.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://al.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://do.hnjuh.cn

[A14] 注释写法
来源：http://yx.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://td.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cr.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://cp.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://au.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yr.521024.cn

Go:   // 单行；/* 多行 */
来源：http://es.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dt.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://lr.szsharing.cn

[A15] 空值判断与默认值
来源：http://qt.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://wn.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://at.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://jr.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://zo.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wy.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://ac.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://sh.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://vu.newstarts.cn

[A16] 真假值判断规则
来源：http://cu.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gu.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xz.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mo.asd995.cn

TS:   if (!x) {}
来源：http://tm.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ay.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kd.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sa.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ih.9csxet.cn

[A17] 位运算
来源：http://ld.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ku.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dm.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kn.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mx.haigaiapp.cn


<!-- 参考信息 -->