代发 wailian999

[U95] JS：Promise 包装
来源：http://ha.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://ml.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://ms.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qe.bjjhwx.cn

[U97] JS：并发请求
来源：http://uy.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oi.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://gz.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://se.gzmigu.cn

[U99] JS：事件监听
来源：http://pw.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://uk.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://ug.newstarts.cn

document.querySelector(".item")
来源：http://fz.huanxung.cn

[U101] JS：classList 操作
来源：http://vi.asd995.cn

el.classList.toggle("active")
来源：http://tf.huanxung.cn

[U102] JS：本地存储
来源：http://jp.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jt.haigaiapp.cn

[U103] JS：定时器
来源：http://zf.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://on.haigaiapp.cn

[U104] JS：防抖
来源：http://hv.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wt.szsharing.cn

[U105] JS：节流
来源：http://rp.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ki.hnjuh.cn

[U106] JS：日期格式化
来源：http://uy.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vr.panjiajie.cn

[U107] JS：数字千分位
来源：http://yk.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iy.huixiangedu.cn

[U108] JS：随机整数
来源：http://qo.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sl.gzmigu.cn

[U109] JS：数组分组
来源：http://vf.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://bc.shxzukj.cn

[U110] JS：数组分块
来源：http://fa.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vr.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://yi.szsharing.cn

new Map(Object.entries(obj))
来源：http://cd.shtwfgs.cn

[U112] JS：字符串补位
来源：http://kf.521024.cn

"7".padStart(3, "0")
来源：http://rk.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://aa.hnjuh.cn

s.replaceAll("a", "b")
来源：http://eq.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://ag.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qh.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://jj.newstarts.cn

crypto.randomUUID()
来源：http://ml.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://te.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://ao.shxzskj.cn

[U117] JS：单元测试
来源：http://yw.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://ei.muxihuayi.cn

[U118] JS：开发服务器
来源：http://le.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://ny.huixiangedu.cn

[U119] JS：生产构建
来源：http://kc.asd995.cn

npx vite build
来源：http://gg.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://ps.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://ws.jctech888.com.cn

================================================================================
来源：http://gj.bookmarksfly.cn

统计汇总
来源：http://vn.colortex.cn

================================================================================
来源：http://op.szxytkj.cn

按语言统计（条）：
来源：http://jd.asd995.cn

Python ......... 252
来源：http://vf.muxihuayi.cn

PHP ............ 252
来源：http://ub.wgjwhj.cn

JavaScript ..... 252
来源：http://md.huanxung.cn

TypeScript ..... 212
来源：http://lh.521024.cn

Java ........... 212
来源：http://vw.shxzskj.cn

Go ............. 212
来源：http://uf.colortex.cn

Ruby ........... 212
来源：http://tx.panjiajie.cn

C# ............. 212
来源：http://ii.haigaiapp.cn

C .............. 30
来源：http://qn.colortex.cn

C++ ............ 30
来源：http://vm.hnjuh.cn

SQL ............ 90
来源：http://sy.jianghongdianzi.cn

Bash ........... 80
来源：http://qd.yuntaijiaju.cn

Kotlin ......... 15
来源：http://ti.521024.cn

Swift .......... 15
来源：http://ll.shxzukj.cn

Lua ............ 10
来源：http://ui.gzmigu.cn

Perl ........... 10
来源：http://zj.shtwfgs.cn

Scala .......... 10
来源：http://qk.hnjuh.cn

------------------------------------
来源：http://yk.shxzskj.cn

合计 ........... 2106 条
来源：http://en.muxihuayi.cn

按章节统计：
来源：http://ts.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gl.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bk.hnjuh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fp.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fb.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cf.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yz.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ii.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yb.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rh.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lf.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kh.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://je.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ln.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vl.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://le.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pt.shxzskj.cn

Q SQL 专题                              90
来源：http://xk.shxzskj.cn

R Bash 专题                             80
来源：http://px.muxihuayi.cn

S C / C++ 专题                          60
来源：http://rw.gzmigu.cn

T 其他语言补充                          60
来源：http://lh.521024.cn

U 高频实用片段                         120
来源：http://bc.panjiajie.cn

------------------------------------
来源：http://xj.wgjwhj.cn

合计                                  2106 条
来源：http://jb.asd995.cn

--------------------------------------------------------------------------------
来源：http://xf.chemitech.net.cn

使用提醒
来源：http://fh.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ae.shxzukj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nc.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mo.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fu.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tp.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bd.newstarts.cn

—— 文件结束 ——
来源：http://df.huixinmuqiang.cn

================================================================================
来源：http://ji.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://hb.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://fu.szsharing.cn

================================================================================
来源：http://fn.szsharing.cn

【收录内容】
来源：http://cu.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ig.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hh.gzmigu.cn

SQL · Bash · C · C++
来源：http://gv.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mz.jianghongdianzi.cn

【使用说明】
来源：http://vz.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jk.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yj.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rq.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jm.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ed.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ol.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bh.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vo.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fd.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aj.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dc.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hs.jctech888.com.cn

【文件统计】
来源：http://ym.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://io.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://wp.shtwfgs.cn

目  录
来源：http://ka.hahajie.cn

--------------------------------------------------------------------------------
来源：http://jm.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ny.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cp.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nx.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nj.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wv.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jo.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://id.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bs.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gb.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fl.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jw.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://og.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iq.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zl.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://id.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xv.nicolike.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pz.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qw.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ht.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uk.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://be.nicolike.cn

================================================================================
来源：http://ur.chemitech.net.cn

A. 基础语法与类型
来源：http://kd.huanxung.cn

================================================================================
来源：http://ec.panjiajie.cn

[A01] Hello World
来源：http://fm.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://zy.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://cy.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://zt.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cg.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://in.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://dp.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://uy.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eu.nicolike.cn

[A02] 变量声明与赋值
来源：http://sy.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lg.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://my.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ek.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fp.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://ll.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://dd.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://bj.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ms.hnjuh.cn

[A03] 常量定义
来源：http://za.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mp.521024.cn

PHP:  const PI = 3.14159;
来源：http://ao.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://zk.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://ht.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://ri.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://vh.nicolike.cn

Ruby: PI = 3.14159
来源：http://kg.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://lm.bjjhwx.cn

[A04] 判断变量类型
来源：http://lk.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mq.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mi.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ie.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://na.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://of.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bk.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jt.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://wm.521024.cn

[A05] 整数除法与取模
来源：http://qn.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://db.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nn.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://co.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kh.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://jp.521024.cn

Go:   7 / 2; 7 % 2
来源：http://bt.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://xt.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://mx.wgjwhj.cn

[A06] 字符串转数字
来源：http://yd.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://gh.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iq.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dt.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dt.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fu.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rc.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hl.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hw.panjiajie.cn

[A07] 数字转字符串
来源：http://kx.shtwfgs.cn

Py:   str(42)
来源：http://on.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://nf.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://cm.huanxung.cn

TS:   String(42)
来源：http://rb.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vf.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://jd.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://kt.colortex.cn

C#:   42.ToString()
来源：http://iu.hahajie.cn

[A08] 取整与四舍五入
来源：http://mg.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fv.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zd.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ga.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cd.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xz.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dl.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zx.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ez.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://dx.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ii.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ty.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qi.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wm.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mn.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nq.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rw.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fw.bookmarksfly.cn

[A10] 生成随机数
来源：http://qf.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://xk.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://bu.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dp.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sn.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://hw.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://es.shtwfgs.cn

Ruby: rand(1..100)
来源：http://kz.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://mo.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://av.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://at.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zp.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zj.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rn.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://nb.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://td.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ew.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ab.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://yy.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xt.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pd.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://ur.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://sz.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://xx.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jw.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://jo.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://yd.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mm.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://ig.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://ze.9csxet.cn

JS:   "第一行\n第二行"
来源：http://ak.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://qy.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://zv.nicolike.cn

Go:   "第一行\n第二行"
来源：http://is.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://pw.newstarts.cn

C#:   "第一行\n第二行"
来源：http://yu.521024.cn

[A14] 注释写法
来源：http://wc.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ol.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ly.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://ec.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://pc.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wg.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://dh.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://it.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://cr.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://gk.huanxung.cn

Py:   value = data or "默认值"
来源：http://ho.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://at.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://bj.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://gq.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qj.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://te.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://ux.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://qo.shxzskj.cn

[A16] 真假值判断规则
来源：http://rt.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ft.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://on.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yr.szxytkj.cn

TS:   if (!x) {}
来源：http://rx.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yf.lnxyls.cn


<!-- 参考信息 -->