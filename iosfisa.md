代发 wailian999

[U99] JS：事件监听
来源：http://hm.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://hv.szsharing.cn

[U100] JS：DOM 查询
来源：http://pi.szxytkj.cn

document.querySelector(".item")
来源：http://pv.shtwfgs.cn

[U101] JS：classList 操作
来源：http://za.huixiangedu.cn

el.classList.toggle("active")
来源：http://ly.hahajie.cn

[U102] JS：本地存储
来源：http://nm.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ja.nszjky.cn

[U103] JS：定时器
来源：http://bt.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://te.lnxyls.cn

[U104] JS：防抖
来源：http://yk.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lp.hnjuh.cn

[U105] JS：节流
来源：http://uh.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://db.haigaiapp.cn

[U106] JS：日期格式化
来源：http://xx.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kl.szxytkj.cn

[U107] JS：数字千分位
来源：http://sm.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://og.gzmigu.cn

[U108] JS：随机整数
来源：http://pe.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sg.nicolike.cn

[U109] JS：数组分组
来源：http://sg.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://ou.lnxyls.cn

[U110] JS：数组分块
来源：http://jp.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fq.colortex.cn

[U111] JS：对象转 Map
来源：http://qj.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://qe.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://wr.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://pd.szsharing.cn

[U113] JS：正则替换全部
来源：http://vz.nicolike.cn

s.replaceAll("a", "b")
来源：http://ir.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://em.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dn.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://my.shtwfgs.cn

crypto.randomUUID()
来源：http://dx.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://mi.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://wa.wgjwhj.cn

[U117] JS：单元测试
来源：http://bx.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://qe.panjiajie.cn

[U118] JS：开发服务器
来源：http://tt.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://cr.huanxung.cn

[U119] JS：生产构建
来源：http://eu.yuntaijiaju.cn

npx vite build
来源：http://yq.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://pf.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://rf.bookmarksfly.cn

================================================================================
来源：http://ca.szsharing.cn

统计汇总
来源：http://en.newstarts.cn

================================================================================
来源：http://gw.newstarts.cn

按语言统计（条）：
来源：http://if.nicolike.cn

Python ......... 252
来源：http://ml.hahajie.cn

PHP ............ 252
来源：http://ej.jianghongdianzi.cn

JavaScript ..... 252
来源：http://fz.9csxet.cn

TypeScript ..... 212
来源：http://bg.huanxung.cn

Java ........... 212
来源：http://vk.szxytkj.cn

Go ............. 212
来源：http://rd.colortex.cn

Ruby ........... 212
来源：http://oa.gzmigu.cn

C# ............. 212
来源：http://nv.shxzskj.cn

C .............. 30
来源：http://pn.panjiajie.cn

C++ ............ 30
来源：http://vd.bjjhwx.cn

SQL ............ 90
来源：http://ds.jctech888.com.cn

Bash ........... 80
来源：http://ly.nszjky.cn

Kotlin ......... 15
来源：http://as.gzmigu.cn

Swift .......... 15
来源：http://zn.nicolike.cn

Lua ............ 10
来源：http://tf.asd995.cn

Perl ........... 10
来源：http://tx.newstarts.cn

Scala .......... 10
来源：http://mf.nszjky.cn

------------------------------------
来源：http://sl.bookmarksfly.cn

合计 ........... 2106 条
来源：http://wf.521024.cn

按章节统计：
来源：http://tn.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ar.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oi.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yt.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uj.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ap.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://md.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ut.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pt.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nk.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yx.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bw.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cb.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vf.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ss.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sr.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ci.lnxyls.cn

Q SQL 专题                              90
来源：http://sa.huixiangedu.cn

R Bash 专题                             80
来源：http://bi.panjiajie.cn

S C / C++ 专题                          60
来源：http://zr.nicolike.cn

T 其他语言补充                          60
来源：http://zx.hahajie.cn

U 高频实用片段                         120
来源：http://qs.szsharing.cn

------------------------------------
来源：http://bl.shxzukj.cn

合计                                  2106 条
来源：http://ke.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ex.newstarts.cn

使用提醒
来源：http://nu.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://za.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hg.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tg.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uv.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zc.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gm.szxytkj.cn

—— 文件结束 ——
来源：http://kx.gzmigu.cn

================================================================================
来源：http://ss.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://fo.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://ik.newstarts.cn

================================================================================
来源：http://wm.bookmarksfly.cn

【收录内容】
来源：http://ij.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pm.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ms.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://my.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cn.panjiajie.cn

【使用说明】
来源：http://an.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jh.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ep.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fv.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wj.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pj.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yw.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qm.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cy.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qt.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qo.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dq.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://au.hnjuh.cn

【文件统计】
来源：http://wj.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yz.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://hi.bjjhwx.cn

目  录
来源：http://nv.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://dp.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ox.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bk.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zi.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iz.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://al.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://un.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jm.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pa.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wn.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uh.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iv.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vy.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cr.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fv.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ia.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qc.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dt.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://at.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mf.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qc.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hh.szxytkj.cn

================================================================================
来源：http://lu.lnxyls.cn

A. 基础语法与类型
来源：http://ai.bookmarksfly.cn

================================================================================
来源：http://xu.haigaiapp.cn

[A01] Hello World
来源：http://ft.hahajie.cn

Py:   print("Hello, World!")
来源：http://ht.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://xe.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://bv.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pp.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://af.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://dw.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://ru.nszjky.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tw.hahajie.cn

[A02] 变量声明与赋值
来源：http://nt.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://if.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jr.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rj.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bs.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://rf.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://jy.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://px.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xu.yuexingan06.cn

[A03] 常量定义
来源：http://mi.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ya.colortex.cn

PHP:  const PI = 3.14159;
来源：http://nm.szsharing.cn

JS:   const PI = 3.14159;
来源：http://gk.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://av.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://pg.szsharing.cn

Go:   const PI = 3.14159
来源：http://wt.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://zb.521024.cn

C#:   const double PI = 3.14159;
来源：http://fv.bookmarksfly.cn

[A04] 判断变量类型
来源：http://fe.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nz.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nd.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pp.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://lo.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dh.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sw.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kn.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://ax.huanxung.cn

[A05] 整数除法与取模
来源：http://mg.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ii.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pr.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pl.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gn.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://eg.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://be.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://zq.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://wg.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://vg.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://sq.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://he.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fb.huixiangedu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xr.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bk.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://af.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yo.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yv.szxytkj.cn

[A07] 数字转字符串
来源：http://lo.shxzukj.cn

Py:   str(42)
来源：http://dr.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://fq.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://th.yuexingan06.cn

TS:   String(42)
来源：http://hl.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vc.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://ei.asd995.cn

Ruby: 42.to_s
来源：http://kq.521024.cn

C#:   42.ToString()
来源：http://mm.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://jm.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ia.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kf.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nn.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gr.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rz.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zt.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jr.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rl.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://rg.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iw.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gg.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tf.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eo.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vz.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vh.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dn.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pm.muxihuayi.cn

[A10] 生成随机数
来源：http://iv.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://bo.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://pu.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zz.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oz.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://ne.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ai.wgjwhj.cn

Ruby: rand(1..100)
来源：http://is.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://sr.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://ue.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://vm.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cm.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vo.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mh.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://yp.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uy.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://el.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pe.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://pz.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yb.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pu.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://wl.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://fe.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://lw.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ak.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://mw.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://jd.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oy.nszjky.cn

Py:   "第一行\n第二行"
来源：http://hu.521024.cn

PHP:  "第一行\n第二行"
来源：http://gw.nicolike.cn

JS:   "第一行\n第二行"
来源：http://qz.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://rq.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://xf.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://bs.asd995.cn

Ruby: "第一行\n第二行"
来源：http://lo.9csxet.cn

C#:   "第一行\n第二行"
来源：http://lm.jctech888.com.cn

[A14] 注释写法
来源：http://uz.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rd.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tu.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://so.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://gp.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ef.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://xh.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ye.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://ks.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://ti.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://jf.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://ta.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://sh.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://bt.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jh.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://mz.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://nf.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://re.yuexingan06.cn

[A16] 真假值判断规则
来源：http://dy.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nx.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://id.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xh.shxzukj.cn

TS:   if (!x) {}
来源：http://we.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ym.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://el.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oy.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://te.muxihuayi.cn

[A17] 位运算
来源：http://vr.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kq.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cb.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://no.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lr.521024.cn


<!-- 参考信息 -->