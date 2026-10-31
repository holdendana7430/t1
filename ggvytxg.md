代发 wailian999

[U97] JS：并发请求
来源：http://by.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vl.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://ap.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ew.huanxung.cn

[U99] JS：事件监听
来源：http://us.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://mj.9csxet.cn

[U100] JS：DOM 查询
来源：http://mh.szxytkj.cn

document.querySelector(".item")
来源：http://ay.szxytkj.cn

[U101] JS：classList 操作
来源：http://vr.lnxyls.cn

el.classList.toggle("active")
来源：http://dk.yuexingan06.cn

[U102] JS：本地存储
来源：http://kw.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sx.jianghongdianzi.cn

[U103] JS：定时器
来源：http://rq.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qk.wgjwhj.cn

[U104] JS：防抖
来源：http://bs.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hd.gzmigu.cn

[U105] JS：节流
来源：http://nb.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gh.wgjwhj.cn

[U106] JS：日期格式化
来源：http://mv.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://on.9csxet.cn

[U107] JS：数字千分位
来源：http://rq.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bt.521024.cn

[U108] JS：随机整数
来源：http://fy.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xi.huanxung.cn

[U109] JS：数组分组
来源：http://xp.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://wm.shtwfgs.cn

[U110] JS：数组分块
来源：http://tz.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zq.lnxyls.cn

[U111] JS：对象转 Map
来源：http://au.hnjuh.cn

new Map(Object.entries(obj))
来源：http://le.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://wl.asd995.cn

"7".padStart(3, "0")
来源：http://nn.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://hb.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://rq.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://sl.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yt.asd995.cn

[U115] JS：生成 UUID
来源：http://ab.jianghongdianzi.cn

crypto.randomUUID()
来源：http://sn.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://gl.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://xl.chemitech.net.cn

[U117] JS：单元测试
来源：http://ki.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://wk.szxytkj.cn

[U118] JS：开发服务器
来源：http://db.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://gc.9csxet.cn

[U119] JS：生产构建
来源：http://lz.huixinmuqiang.cn

npx vite build
来源：http://mi.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://na.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://tg.yuexingan06.cn

================================================================================
来源：http://gc.asd995.cn

统计汇总
来源：http://mi.huixiangedu.cn

================================================================================
来源：http://gu.asd995.cn

按语言统计（条）：
来源：http://fu.yuexingan06.cn

Python ......... 252
来源：http://bm.colortex.cn

PHP ............ 252
来源：http://dk.wgjwhj.cn

JavaScript ..... 252
来源：http://zl.huixiangedu.cn

TypeScript ..... 212
来源：http://sq.gzmigu.cn

Java ........... 212
来源：http://hk.newstarts.cn

Go ............. 212
来源：http://tz.gzmigu.cn

Ruby ........... 212
来源：http://pg.yuexingan06.cn

C# ............. 212
来源：http://kq.hnjuh.cn

C .............. 30
来源：http://jz.panjiajie.cn

C++ ............ 30
来源：http://ij.szxytkj.cn

SQL ............ 90
来源：http://lp.muxihuayi.cn

Bash ........... 80
来源：http://jz.huixiangedu.cn

Kotlin ......... 15
来源：http://vx.gzmigu.cn

Swift .......... 15
来源：http://ij.shxzskj.cn

Lua ............ 10
来源：http://ud.wgjwhj.cn

Perl ........... 10
来源：http://is.bjjhwx.cn

Scala .......... 10
来源：http://eu.nicolike.cn

------------------------------------
来源：http://ae.panjiajie.cn

合计 ........... 2106 条
来源：http://bt.shtwfgs.cn

按章节统计：
来源：http://ds.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://je.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gs.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aq.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zv.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ic.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://it.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ut.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ig.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xf.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bq.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xs.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qy.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://il.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gp.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://es.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jk.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://vc.newstarts.cn

R Bash 专题                             80
来源：http://nr.shxzukj.cn

S C / C++ 专题                          60
来源：http://ok.bookmarksfly.cn

T 其他语言补充                          60
来源：http://ij.jctech888.com.cn

U 高频实用片段                         120
来源：http://ts.haigaiapp.cn

------------------------------------
来源：http://pp.huanxung.cn

合计                                  2106 条
来源：http://gc.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://uy.shtwfgs.cn

使用提醒
来源：http://qp.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://bt.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aa.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yc.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ij.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zv.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zf.huixinmuqiang.cn

—— 文件结束 ——
来源：http://ay.bjjhwx.cn

================================================================================
来源：http://uf.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://ca.newstarts.cn

Common Programming Examples Cheat Book
来源：http://tr.muxihuayi.cn

================================================================================
来源：http://wu.wgjwhj.cn

【收录内容】
来源：http://ke.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gm.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ql.asd995.cn

SQL · Bash · C · C++
来源：http://bk.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qd.huixiangedu.cn

【使用说明】
来源：http://vm.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bo.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vm.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nk.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qv.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ch.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jy.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qy.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://av.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fu.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ir.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gf.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ih.muxihuayi.cn

【文件统计】
来源：http://yu.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xk.colortex.cn

--------------------------------------------------------------------------------
来源：http://zv.hnjuh.cn

目  录
来源：http://au.nicolike.cn

--------------------------------------------------------------------------------
来源：http://yn.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uj.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xf.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://et.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vf.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sk.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://es.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rv.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zh.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ca.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://al.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gf.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xu.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://td.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ie.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ja.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mb.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ks.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://up.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jl.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://se.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pj.521024.cn

================================================================================
来源：http://st.asd995.cn

A. 基础语法与类型
来源：http://yb.jianghongdianzi.cn

================================================================================
来源：http://mb.gzmigu.cn

[A01] Hello World
来源：http://ae.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ta.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://nd.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://sa.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cr.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://ij.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://cw.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://wl.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yd.521024.cn

[A02] 变量声明与赋值
来源：http://kn.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zw.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oj.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vc.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ik.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://vw.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://ko.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://yu.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nw.wgjwhj.cn

[A03] 常量定义
来源：http://dx.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sp.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://oc.hahajie.cn

JS:   const PI = 3.14159;
来源：http://kp.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://pb.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://ei.panjiajie.cn

Go:   const PI = 3.14159
来源：http://zg.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://dt.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://un.shxzskj.cn

[A04] 判断变量类型
来源：http://zu.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nn.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uu.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hy.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://lg.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pu.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mv.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wz.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://al.shxzukj.cn

[A05] 整数除法与取模
来源：http://qw.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ci.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ix.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lc.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ay.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://fb.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://cm.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://tz.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://su.lnxyls.cn

[A06] 字符串转数字
来源：http://ck.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://sm.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kz.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dn.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vz.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://or.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zn.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ai.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wi.chemitech.net.cn

[A07] 数字转字符串
来源：http://du.jctech888.com.cn

Py:   str(42)
来源：http://mn.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://lt.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://sj.panjiajie.cn

TS:   String(42)
来源：http://qu.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nc.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://ci.hahajie.cn

Ruby: 42.to_s
来源：http://yc.jctech888.com.cn

C#:   42.ToString()
来源：http://qo.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://vr.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ql.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cv.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qo.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sb.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://up.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bl.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gh.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ao.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://ak.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fa.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xk.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nn.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yj.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://om.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fs.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xh.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pn.jctech888.com.cn

[A10] 生成随机数
来源：http://cp.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://he.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://pj.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zr.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ba.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://pp.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://br.newstarts.cn

Ruby: rand(1..100)
来源：http://vg.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://yg.hahajie.cn

[A11] 条件表达式（三元）
来源：http://qk.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://oq.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://di.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yv.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fm.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://zf.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://to.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ao.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nx.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://sv.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gh.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ps.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://ve.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://ki.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://ae.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dv.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://rp.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://or.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fl.hahajie.cn

Py:   "第一行\n第二行"
来源：http://cf.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://lm.nszjky.cn

JS:   "第一行\n第二行"
来源：http://eb.nicolike.cn

TS:   "第一行\n第二行"
来源：http://zb.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://gt.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://wj.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://ea.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://ox.shtwfgs.cn

[A14] 注释写法
来源：http://et.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fa.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yl.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://dp.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://ep.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ji.521024.cn

Go:   // 单行；/* 多行 */
来源：http://es.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vt.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://nf.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://oc.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://up.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://wj.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://io.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://xc.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ry.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://xc.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://kl.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://vl.lnxyls.cn

[A16] 真假值判断规则
来源：http://uc.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pz.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xr.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hn.panjiajie.cn

TS:   if (!x) {}
来源：http://xl.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ut.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dw.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lc.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qk.haigaiapp.cn

[A17] 位运算
来源：http://zw.jianghongdianzi.cn


<!-- 参考信息 -->