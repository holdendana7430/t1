代发 wailian999

[U91] JS：对象键值遍历
来源：http://ws.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zr.nicolike.cn

[U92] JS：深拷贝
来源：http://oo.lnxyls.cn

structuredClone(obj)
来源：http://oa.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://jl.szsharing.cn

`共 ${n} 条`
来源：http://jm.newstarts.cn

[U94] JS：箭头函数
来源：http://gx.hnjuh.cn

const double = x => x * 2;
来源：http://qe.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://le.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://gd.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://ap.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dp.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://hk.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ts.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://vh.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nf.bjjhwx.cn

[U99] JS：事件监听
来源：http://kl.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://kb.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://bu.jctech888.com.cn

document.querySelector(".item")
来源：http://yj.yuexingan06.cn

[U101] JS：classList 操作
来源：http://gl.bjjhwx.cn

el.classList.toggle("active")
来源：http://yj.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://yf.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wg.bookmarksfly.cn

[U103] JS：定时器
来源：http://yq.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ll.lnxyls.cn

[U104] JS：防抖
来源：http://ii.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pu.yuntaijiaju.cn

[U105] JS：节流
来源：http://cm.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wn.colortex.cn

[U106] JS：日期格式化
来源：http://tm.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jd.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://hf.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qz.nicolike.cn

[U108] JS：随机整数
来源：http://di.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ro.huanxung.cn

[U109] JS：数组分组
来源：http://oc.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://ud.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://ck.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wn.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://zc.lnxyls.cn

new Map(Object.entries(obj))
来源：http://vg.panjiajie.cn

[U112] JS：字符串补位
来源：http://tb.gzmigu.cn

"7".padStart(3, "0")
来源：http://ho.szxytkj.cn

[U113] JS：正则替换全部
来源：http://zw.nicolike.cn

s.replaceAll("a", "b")
来源：http://uh.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://rz.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pj.newstarts.cn

[U115] JS：生成 UUID
来源：http://oh.asd995.cn

crypto.randomUUID()
来源：http://uo.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ub.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://dd.hnjuh.cn

[U117] JS：单元测试
来源：http://kr.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://at.lnxyls.cn

[U118] JS：开发服务器
来源：http://yw.szxytkj.cn

npm i -D vite;  npx vite
来源：http://rz.huixiangedu.cn

[U119] JS：生产构建
来源：http://sz.521024.cn

npx vite build
来源：http://tb.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://ej.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://mg.521024.cn

================================================================================
来源：http://ug.asd995.cn

统计汇总
来源：http://zj.panjiajie.cn

================================================================================
来源：http://uh.szxytkj.cn

按语言统计（条）：
来源：http://ai.9csxet.cn

Python ......... 252
来源：http://sq.colortex.cn

PHP ............ 252
来源：http://zh.huixinmuqiang.cn

JavaScript ..... 252
来源：http://ev.521024.cn

TypeScript ..... 212
来源：http://qf.panjiajie.cn

Java ........... 212
来源：http://ee.asd995.cn

Go ............. 212
来源：http://qf.jianghongdianzi.cn

Ruby ........... 212
来源：http://yv.huixiangedu.cn

C# ............. 212
来源：http://di.shtwfgs.cn

C .............. 30
来源：http://wf.colortex.cn

C++ ............ 30
来源：http://zl.chemitech.net.cn

SQL ............ 90
来源：http://kd.nicolike.cn

Bash ........... 80
来源：http://mm.szsharing.cn

Kotlin ......... 15
来源：http://zl.szsharing.cn

Swift .......... 15
来源：http://ff.hnjuh.cn

Lua ............ 10
来源：http://sa.newstarts.cn

Perl ........... 10
来源：http://hy.chemitech.net.cn

Scala .......... 10
来源：http://wg.shxzskj.cn

------------------------------------
来源：http://ao.szsharing.cn

合计 ........... 2106 条
来源：http://cc.newstarts.cn

按章节统计：
来源：http://nz.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ye.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rc.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zq.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wp.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ht.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://la.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ek.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bm.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xu.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sd.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bh.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://we.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kd.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://va.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://on.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oo.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://pm.jianghongdianzi.cn

R Bash 专题                             80
来源：http://mx.nicolike.cn

S C / C++ 专题                          60
来源：http://rv.nszjky.cn

T 其他语言补充                          60
来源：http://qz.wgjwhj.cn

U 高频实用片段                         120
来源：http://kq.asd995.cn

------------------------------------
来源：http://wk.newstarts.cn

合计                                  2106 条
来源：http://zy.hahajie.cn

--------------------------------------------------------------------------------
来源：http://kl.yuntaijiaju.cn

使用提醒
来源：http://hb.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://wq.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gg.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://im.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lr.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wh.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pq.shtwfgs.cn

—— 文件结束 ——
来源：http://ts.gzmigu.cn

================================================================================
来源：http://wc.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://xn.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://ih.asd995.cn

================================================================================
来源：http://eg.panjiajie.cn

【收录内容】
来源：http://ef.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ym.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tf.lnxyls.cn

SQL · Bash · C · C++
来源：http://rk.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yo.shxzskj.cn

【使用说明】
来源：http://fe.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ik.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://db.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gc.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tw.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gu.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gr.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uo.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ev.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bq.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ov.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oh.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bb.521024.cn

【文件统计】
来源：http://ez.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lj.szsharing.cn

--------------------------------------------------------------------------------
来源：http://df.bjjhwx.cn

目  录
来源：http://vn.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://co.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tb.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ji.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://on.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dq.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cp.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dz.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hp.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://os.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gx.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ku.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aw.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nj.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vt.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://on.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://de.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ax.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zd.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ae.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pr.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bd.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ih.muxihuayi.cn

================================================================================
来源：http://px.huixinmuqiang.cn

A. 基础语法与类型
来源：http://at.colortex.cn

================================================================================
来源：http://ms.colortex.cn

[A01] Hello World
来源：http://bo.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://ed.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://sf.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://ha.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cm.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://hh.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://gp.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://wd.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hi.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://kx.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kz.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vt.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ta.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ax.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://rf.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://vq.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://vq.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gz.szxytkj.cn

[A03] 常量定义
来源：http://fb.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sy.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://tq.nszjky.cn

JS:   const PI = 3.14159;
来源：http://sp.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://mm.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://bg.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://uw.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://ep.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://me.wgjwhj.cn

[A04] 判断变量类型
来源：http://gn.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aa.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nt.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ux.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://sk.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jg.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gr.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tq.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://pa.bjjhwx.cn

[A05] 整数除法与取模
来源：http://sc.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://er.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://na.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yd.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://db.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://my.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://he.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://ga.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://be.shxzskj.cn

[A06] 字符串转数字
来源：http://pu.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://mj.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xc.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sm.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xr.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://li.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dw.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jp.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dw.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://ho.huixiangedu.cn

Py:   str(42)
来源：http://nu.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://sd.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://yg.yuntaijiaju.cn

TS:   String(42)
来源：http://mn.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xu.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://xb.panjiajie.cn

Ruby: 42.to_s
来源：http://mh.huixinmuqiang.cn

C#:   42.ToString()
来源：http://wf.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://qi.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://of.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gm.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wr.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ib.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rj.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bh.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ht.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ie.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://cy.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dl.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ww.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gb.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://on.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jl.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dt.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ex.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cu.hahajie.cn

[A10] 生成随机数
来源：http://xw.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://qu.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://qc.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zh.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://at.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://vt.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xo.jctech888.com.cn

Ruby: rand(1..100)
来源：http://wr.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://je.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://iq.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://uw.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tl.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ga.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://en.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://mg.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cv.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://db.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zq.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://ke.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bp.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bd.asd995.cn

JS:   `Hello, ${name}!`
来源：http://ns.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://uy.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://er.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yy.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://ey.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://rn.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xd.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://zn.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://cl.szsharing.cn

JS:   "第一行\n第二行"
来源：http://ht.newstarts.cn

TS:   "第一行\n第二行"
来源：http://xn.gzmigu.cn

Java: "第一行\n第二行"
来源：http://rl.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://su.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://po.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://uv.9csxet.cn

[A14] 注释写法
来源：http://my.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vo.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bl.521024.cn

JS:   // 单行；/* 多行 */
来源：http://ll.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://oj.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lx.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://fw.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xw.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://jh.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://rq.nszjky.cn

Py:   value = data or "默认值"
来源：http://vz.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://iw.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://rq.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://tj.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pi.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://ej.asd995.cn


<!-- 参考信息 -->