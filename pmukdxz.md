代发 wailian999

[U93] JS：模板字符串
来源：http://kd.colortex.cn

`共 ${n} 条`
来源：http://ik.asd995.cn

[U94] JS：箭头函数
来源：http://iu.huixinmuqiang.cn

const double = x => x * 2;
来源：http://ej.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://pa.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://ss.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://nq.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qv.panjiajie.cn

[U97] JS：并发请求
来源：http://xj.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jy.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://gq.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nx.shxzskj.cn

[U99] JS：事件监听
来源：http://kx.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://tr.panjiajie.cn

[U100] JS：DOM 查询
来源：http://ev.lnxyls.cn

document.querySelector(".item")
来源：http://ii.bjjhwx.cn

[U101] JS：classList 操作
来源：http://mj.nicolike.cn

el.classList.toggle("active")
来源：http://xb.yuexingan06.cn

[U102] JS：本地存储
来源：http://po.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dc.huixinmuqiang.cn

[U103] JS：定时器
来源：http://gh.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ab.asd995.cn

[U104] JS：防抖
来源：http://yj.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sx.haigaiapp.cn

[U105] JS：节流
来源：http://sq.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ij.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://cc.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lw.gzmigu.cn

[U107] JS：数字千分位
来源：http://br.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rj.gzmigu.cn

[U108] JS：随机整数
来源：http://zm.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tm.szxytkj.cn

[U109] JS：数组分组
来源：http://qv.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://fs.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://rc.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ej.shxzukj.cn

[U111] JS：对象转 Map
来源：http://jc.hnjuh.cn

new Map(Object.entries(obj))
来源：http://cu.nicolike.cn

[U112] JS：字符串补位
来源：http://zy.shxzskj.cn

"7".padStart(3, "0")
来源：http://cp.asd995.cn

[U113] JS：正则替换全部
来源：http://bj.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://mc.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://yp.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ot.shxzskj.cn

[U115] JS：生成 UUID
来源：http://uk.hnjuh.cn

crypto.randomUUID()
来源：http://hy.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://rv.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://bj.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://oz.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://ev.chemitech.net.cn

[U118] JS：开发服务器
来源：http://dg.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://jv.shxzskj.cn

[U119] JS：生产构建
来源：http://ua.shxzukj.cn

npx vite build
来源：http://xv.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://vr.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://cr.shtwfgs.cn

================================================================================
来源：http://zd.lnxyls.cn

统计汇总
来源：http://wh.9csxet.cn

================================================================================
来源：http://mg.gzmigu.cn

按语言统计（条）：
来源：http://xk.newstarts.cn

Python ......... 252
来源：http://ru.colortex.cn

PHP ............ 252
来源：http://jr.panjiajie.cn

JavaScript ..... 252
来源：http://jn.bjjhwx.cn

TypeScript ..... 212
来源：http://ir.shxzukj.cn

Java ........... 212
来源：http://yi.jianghongdianzi.cn

Go ............. 212
来源：http://xe.shxzskj.cn

Ruby ........... 212
来源：http://jb.hahajie.cn

C# ............. 212
来源：http://oc.shtwfgs.cn

C .............. 30
来源：http://bc.huanxung.cn

C++ ............ 30
来源：http://sr.szsharing.cn

SQL ............ 90
来源：http://eb.wgjwhj.cn

Bash ........... 80
来源：http://tq.nicolike.cn

Kotlin ......... 15
来源：http://wz.panjiajie.cn

Swift .......... 15
来源：http://sa.wgjwhj.cn

Lua ............ 10
来源：http://vw.hahajie.cn

Perl ........... 10
来源：http://ru.szxytkj.cn

Scala .......... 10
来源：http://dq.nszjky.cn

------------------------------------
来源：http://vi.huixiangedu.cn

合计 ........... 2106 条
来源：http://bm.bookmarksfly.cn

按章节统计：
来源：http://ux.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://je.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rv.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rk.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://px.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yt.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pi.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wf.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yz.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aa.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ub.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zl.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ie.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kq.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oz.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uu.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yd.bookmarksfly.cn

Q SQL 专题                              90
来源：http://ps.yuexingan06.cn

R Bash 专题                             80
来源：http://sc.gzmigu.cn

S C / C++ 专题                          60
来源：http://rs.nicolike.cn

T 其他语言补充                          60
来源：http://nm.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://pq.newstarts.cn

------------------------------------
来源：http://nk.gzmigu.cn

合计                                  2106 条
来源：http://ab.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://bl.chemitech.net.cn

使用提醒
来源：http://ba.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://jy.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ur.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bp.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zg.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yx.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wt.bookmarksfly.cn

—— 文件结束 ——
来源：http://og.haigaiapp.cn

================================================================================
来源：http://vs.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://fj.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://cs.9csxet.cn

================================================================================
来源：http://zb.yuntaijiaju.cn

【收录内容】
来源：http://kz.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oc.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ap.haigaiapp.cn

SQL · Bash · C · C++
来源：http://iz.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sf.muxihuayi.cn

【使用说明】
来源：http://hh.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gt.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ar.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ch.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bf.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sq.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fm.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fv.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vb.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xz.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aw.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gp.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zy.asd995.cn

【文件统计】
来源：http://mo.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://od.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ec.huanxung.cn

目  录
来源：http://yg.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://pi.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bc.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jz.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zp.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rk.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://my.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ag.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zf.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zw.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yq.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ey.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mk.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zy.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kj.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hy.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nj.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bl.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yo.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ob.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://br.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fg.shxzskj.cn

================================================================================
来源：http://yb.panjiajie.cn

A. 基础语法与类型
来源：http://aa.huixinmuqiang.cn

================================================================================
来源：http://cg.szxytkj.cn

[A01] Hello World
来源：http://xz.huanxung.cn

Py:   print("Hello, World!")
来源：http://ns.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://iv.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://rl.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mg.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://os.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://wi.521024.cn

Ruby: puts "Hello, World!"
来源：http://sh.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://er.gzmigu.cn

[A02] 变量声明与赋值
来源：http://tp.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nx.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://np.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cg.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ui.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://id.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://on.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://nl.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gf.colortex.cn

[A03] 常量定义
来源：http://ou.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pc.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://eu.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://gr.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://uq.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://bx.shxzukj.cn

Go:   const PI = 3.14159
来源：http://uu.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://bt.asd995.cn

C#:   const double PI = 3.14159;
来源：http://od.shxzukj.cn

[A04] 判断变量类型
来源：http://mi.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fs.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yq.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ir.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://ca.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://po.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zv.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ty.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://es.hahajie.cn

[A05] 整数除法与取模
来源：http://xj.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jo.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rn.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mf.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sm.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://mq.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://ev.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://wr.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://dv.jctech888.com.cn

[A06] 字符串转数字
来源：http://uc.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://qr.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cp.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dc.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tm.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dt.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nn.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://en.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ld.bookmarksfly.cn

[A07] 数字转字符串
来源：http://en.shxzskj.cn

Py:   str(42)
来源：http://sd.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://bl.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://un.szsharing.cn

TS:   String(42)
来源：http://pq.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kg.521024.cn

Go:   strconv.Itoa(42)
来源：http://pf.shxzukj.cn

Ruby: 42.to_s
来源：http://pj.9csxet.cn

C#:   42.ToString()
来源：http://vc.hahajie.cn

[A08] 取整与四舍五入
来源：http://cl.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mf.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rn.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ya.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gh.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ax.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iy.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gx.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://of.asd995.cn

[A09] 绝对值与最大最小值
来源：http://cz.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mc.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rd.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rw.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lt.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zx.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wy.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ih.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vi.szsharing.cn

[A10] 生成随机数
来源：http://vx.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://ji.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://jh.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sm.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uj.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://ks.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ph.haigaiapp.cn

Ruby: rand(1..100)
来源：http://rp.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://dk.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://ba.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://iy.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://df.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ml.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kc.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://ih.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pz.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aj.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gq.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://lm.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zi.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xt.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://ui.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://ac.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://yv.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ms.521024.cn

Ruby: "Hello, #{name}!"
来源：http://dv.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://fk.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xk.521024.cn

Py:   "第一行\n第二行"
来源：http://ga.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://qj.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://xr.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://mi.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://tc.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://au.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://ss.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://ve.newstarts.cn

[A14] 注释写法
来源：http://bm.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zv.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ta.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://zd.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://lx.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fb.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://fz.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yq.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://rm.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://ey.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://uf.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://fw.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://il.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://dv.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sd.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://jq.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://du.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://xc.shxzskj.cn

[A16] 真假值判断规则
来源：http://jh.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nw.chemitech.net.cn


<!-- 参考信息 -->