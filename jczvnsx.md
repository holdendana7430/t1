代发 wailian999

[U89] JS：数组去重
来源：http://od.hahajie.cn

[...new Set(arr)]
来源：http://hi.newstarts.cn

[U90] JS：数字数组排序
来源：http://vj.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://ef.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://iz.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ds.huanxung.cn

[U92] JS：深拷贝
来源：http://lb.bookmarksfly.cn

structuredClone(obj)
来源：http://dn.hahajie.cn

[U93] JS：模板字符串
来源：http://ir.shxzskj.cn

`共 ${n} 条`
来源：http://fd.nszjky.cn

[U94] JS：箭头函数
来源：http://sm.huixinmuqiang.cn

const double = x => x * 2;
来源：http://na.huanxung.cn

[U95] JS：Promise 包装
来源：http://jh.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://hc.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://uz.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ud.wgjwhj.cn

[U97] JS：并发请求
来源：http://qg.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://am.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://mb.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://an.huixiangedu.cn

[U99] JS：事件监听
来源：http://qc.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://al.huanxung.cn

[U100] JS：DOM 查询
来源：http://ib.yuntaijiaju.cn

document.querySelector(".item")
来源：http://pf.shxzskj.cn

[U101] JS：classList 操作
来源：http://zh.wgjwhj.cn

el.classList.toggle("active")
来源：http://ot.haigaiapp.cn

[U102] JS：本地存储
来源：http://ug.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ag.wgjwhj.cn

[U103] JS：定时器
来源：http://oi.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pa.yuexingan06.cn

[U104] JS：防抖
来源：http://ro.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xj.shtwfgs.cn

[U105] JS：节流
来源：http://po.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wy.huanxung.cn

[U106] JS：日期格式化
来源：http://ot.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uy.muxihuayi.cn

[U107] JS：数字千分位
来源：http://qw.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eb.hahajie.cn

[U108] JS：随机整数
来源：http://qw.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ha.bjjhwx.cn

[U109] JS：数组分组
来源：http://ih.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://av.bookmarksfly.cn

[U110] JS：数组分块
来源：http://td.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oi.nicolike.cn

[U111] JS：对象转 Map
来源：http://qz.szxytkj.cn

new Map(Object.entries(obj))
来源：http://sh.jctech888.com.cn

[U112] JS：字符串补位
来源：http://af.muxihuayi.cn

"7".padStart(3, "0")
来源：http://tb.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://md.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://zu.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://wc.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xg.nicolike.cn

[U115] JS：生成 UUID
来源：http://ug.chemitech.net.cn

crypto.randomUUID()
来源：http://ib.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://bx.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://nl.bookmarksfly.cn

[U117] JS：单元测试
来源：http://yu.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://iu.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://pd.hahajie.cn

npm i -D vite;  npx vite
来源：http://ei.chemitech.net.cn

[U119] JS：生产构建
来源：http://kt.huixiangedu.cn

npx vite build
来源：http://tt.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://gv.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://wo.shxzskj.cn

================================================================================
来源：http://ne.szxytkj.cn

统计汇总
来源：http://fc.huanxung.cn

================================================================================
来源：http://uh.asd995.cn

按语言统计（条）：
来源：http://bp.chemitech.net.cn

Python ......... 252
来源：http://hi.lnxyls.cn

PHP ............ 252
来源：http://uz.yuexingan06.cn

JavaScript ..... 252
来源：http://ih.lnxyls.cn

TypeScript ..... 212
来源：http://cp.colortex.cn

Java ........... 212
来源：http://lf.shxzskj.cn

Go ............. 212
来源：http://sq.szsharing.cn

Ruby ........... 212
来源：http://qd.jctech888.com.cn

C# ............. 212
来源：http://ke.9csxet.cn

C .............. 30
来源：http://ed.hnjuh.cn

C++ ............ 30
来源：http://pf.gzmigu.cn

SQL ............ 90
来源：http://um.asd995.cn

Bash ........... 80
来源：http://ge.shtwfgs.cn

Kotlin ......... 15
来源：http://py.huanxung.cn

Swift .......... 15
来源：http://fc.muxihuayi.cn

Lua ............ 10
来源：http://sq.yuexingan06.cn

Perl ........... 10
来源：http://yr.shxzukj.cn

Scala .......... 10
来源：http://eu.jctech888.com.cn

------------------------------------
来源：http://we.haigaiapp.cn

合计 ........... 2106 条
来源：http://og.newstarts.cn

按章节统计：
来源：http://uh.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ux.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xm.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yo.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hn.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://th.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gp.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dg.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://av.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fm.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eu.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dq.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ko.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uf.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://av.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dn.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qj.huanxung.cn

Q SQL 专题                              90
来源：http://cb.hahajie.cn

R Bash 专题                             80
来源：http://wg.haigaiapp.cn

S C / C++ 专题                          60
来源：http://ez.colortex.cn

T 其他语言补充                          60
来源：http://yp.bjjhwx.cn

U 高频实用片段                         120
来源：http://jr.jianghongdianzi.cn

------------------------------------
来源：http://ye.jctech888.com.cn

合计                                  2106 条
来源：http://wi.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://bg.huanxung.cn

使用提醒
来源：http://uz.colortex.cn

--------------------------------------------------------------------------------
来源：http://sg.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wc.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ex.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ei.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://te.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qk.wgjwhj.cn

—— 文件结束 ——
来源：http://ss.jctech888.com.cn

================================================================================
来源：http://rp.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://ce.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://yi.nicolike.cn

================================================================================
来源：http://gw.huanxung.cn

【收录内容】
来源：http://tv.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yz.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hf.newstarts.cn

SQL · Bash · C · C++
来源：http://nf.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yr.huanxung.cn

【使用说明】
来源：http://hf.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://en.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sn.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rc.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gi.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nz.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://it.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sp.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://se.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yb.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jz.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ch.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mf.yuexingan06.cn

【文件统计】
来源：http://pe.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ol.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://zy.lnxyls.cn

目  录
来源：http://bq.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://xp.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bi.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cq.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jw.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gq.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://db.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wx.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aj.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://at.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sd.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hj.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hq.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xv.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dr.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ex.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hc.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ne.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rf.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ln.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dx.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mb.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jt.haigaiapp.cn

================================================================================
来源：http://ed.9csxet.cn

A. 基础语法与类型
来源：http://le.chemitech.net.cn

================================================================================
来源：http://fp.lnxyls.cn

[A01] Hello World
来源：http://sn.gzmigu.cn

Py:   print("Hello, World!")
来源：http://ay.colortex.cn

PHP:  echo "Hello, World!";
来源：http://gl.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://bg.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sv.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://to.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://ny.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://no.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zf.asd995.cn

[A02] 变量声明与赋值
来源：http://od.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uz.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hg.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mu.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dp.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://to.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://bc.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://bv.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yw.asd995.cn

[A03] 常量定义
来源：http://wr.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://at.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://hx.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://wm.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://ur.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://ph.asd995.cn

Go:   const PI = 3.14159
来源：http://av.shxzskj.cn

Ruby: PI = 3.14159
来源：http://sw.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://kz.haigaiapp.cn

[A04] 判断变量类型
来源：http://it.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ko.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yf.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zi.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://eo.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://by.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xf.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ok.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://zj.hnjuh.cn

[A05] 整数除法与取模
来源：http://bb.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jx.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rh.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rg.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ga.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://my.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://of.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://pa.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://gz.hahajie.cn

[A06] 字符串转数字
来源：http://yg.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://dz.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://by.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gg.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hx.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dc.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pb.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vt.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zh.lnxyls.cn

[A07] 数字转字符串
来源：http://kk.szxytkj.cn

Py:   str(42)
来源：http://km.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://cx.asd995.cn

JS:   String(42); (42).toString()
来源：http://po.nicolike.cn

TS:   String(42)
来源：http://wt.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nu.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://hp.asd995.cn

Ruby: 42.to_s
来源：http://nm.yuntaijiaju.cn

C#:   42.ToString()
来源：http://yf.gzmigu.cn

[A08] 取整与四舍五入
来源：http://hk.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ur.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jq.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://el.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hd.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xy.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qc.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mr.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ve.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://ze.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cu.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nn.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://il.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qs.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://js.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zl.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yf.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sd.gzmigu.cn

[A10] 生成随机数
来源：http://kp.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://lx.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://vr.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cz.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kk.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://ao.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ou.shtwfgs.cn

Ruby: rand(1..100)
来源：http://ts.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://gw.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://vc.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://ag.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wu.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zo.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kb.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://zb.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fi.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fb.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zr.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://gg.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jq.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gj.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://uf.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://hm.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://qi.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ws.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://hx.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://dg.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nf.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://yy.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://jd.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://lf.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://gv.gzmigu.cn

Java: "第一行\n第二行"
来源：http://dc.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://qm.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://jp.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://hz.huanxung.cn

[A14] 注释写法
来源：http://lc.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://om.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rf.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://mb.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://sk.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dp.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://mr.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dy.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://fv.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://wq.nszjky.cn

Py:   value = data or "默认值"
来源：http://qw.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://zt.szxytkj.cn


<!-- 参考信息 -->