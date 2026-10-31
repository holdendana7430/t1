代发 wailian999

[U85] JS：可选链
来源：http://sy.muxihuayi.cn

a?.b?.c
来源：http://uj.szxytkj.cn

[U86] JS：空值合并
来源：http://xf.colortex.cn

a ?? b
来源：http://cp.szsharing.cn

[U87] JS：解构默认值
来源：http://hn.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://kg.nszjky.cn

[U88] JS：对象展开合并
来源：http://fa.lnxyls.cn

{ ...a, ...b }
来源：http://go.shxzskj.cn

[U89] JS：数组去重
来源：http://oy.wgjwhj.cn

[...new Set(arr)]
来源：http://ry.521024.cn

[U90] JS：数字数组排序
来源：http://dt.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://xx.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://mi.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bw.lnxyls.cn

[U92] JS：深拷贝
来源：http://pz.521024.cn

structuredClone(obj)
来源：http://zf.chemitech.net.cn

[U93] JS：模板字符串
来源：http://qk.hnjuh.cn

`共 ${n} 条`
来源：http://sn.bjjhwx.cn

[U94] JS：箭头函数
来源：http://mi.huixinmuqiang.cn

const double = x => x * 2;
来源：http://me.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://uw.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://un.szsharing.cn

[U96] JS：async/await 与异常
来源：http://wn.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ra.szsharing.cn

[U97] JS：并发请求
来源：http://ef.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uj.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://id.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zs.lnxyls.cn

[U99] JS：事件监听
来源：http://bg.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://ba.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://ko.chemitech.net.cn

document.querySelector(".item")
来源：http://fm.521024.cn

[U101] JS：classList 操作
来源：http://hi.huanxung.cn

el.classList.toggle("active")
来源：http://st.wgjwhj.cn

[U102] JS：本地存储
来源：http://su.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zj.huixinmuqiang.cn

[U103] JS：定时器
来源：http://op.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ym.nicolike.cn

[U104] JS：防抖
来源：http://qm.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yr.gzmigu.cn

[U105] JS：节流
来源：http://th.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oy.szxytkj.cn

[U106] JS：日期格式化
来源：http://fk.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ya.nszjky.cn

[U107] JS：数字千分位
来源：http://kz.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cw.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://bw.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sz.521024.cn

[U109] JS：数组分组
来源：http://yp.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://lf.9csxet.cn

[U110] JS：数组分块
来源：http://is.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ru.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://vk.szxytkj.cn

new Map(Object.entries(obj))
来源：http://yo.shtwfgs.cn

[U112] JS：字符串补位
来源：http://sy.bjjhwx.cn

"7".padStart(3, "0")
来源：http://nj.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://tt.panjiajie.cn

s.replaceAll("a", "b")
来源：http://cr.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://dx.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xj.hnjuh.cn

[U115] JS：生成 UUID
来源：http://zp.haigaiapp.cn

crypto.randomUUID()
来源：http://wt.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://oj.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://lo.shxzskj.cn

[U117] JS：单元测试
来源：http://qe.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://eq.colortex.cn

[U118] JS：开发服务器
来源：http://mf.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://bl.hahajie.cn

[U119] JS：生产构建
来源：http://xe.bookmarksfly.cn

npx vite build
来源：http://vf.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://vm.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://ds.chemitech.net.cn

================================================================================
来源：http://bf.szsharing.cn

统计汇总
来源：http://te.bjjhwx.cn

================================================================================
来源：http://nv.hahajie.cn

按语言统计（条）：
来源：http://si.yuexingan06.cn

Python ......... 252
来源：http://tb.haigaiapp.cn

PHP ............ 252
来源：http://gp.hnjuh.cn

JavaScript ..... 252
来源：http://ne.yuntaijiaju.cn

TypeScript ..... 212
来源：http://xa.huixinmuqiang.cn

Java ........... 212
来源：http://fn.nicolike.cn

Go ............. 212
来源：http://uj.huixinmuqiang.cn

Ruby ........... 212
来源：http://je.shtwfgs.cn

C# ............. 212
来源：http://tl.jctech888.com.cn

C .............. 30
来源：http://pe.nicolike.cn

C++ ............ 30
来源：http://oo.muxihuayi.cn

SQL ............ 90
来源：http://na.bookmarksfly.cn

Bash ........... 80
来源：http://hc.asd995.cn

Kotlin ......... 15
来源：http://jz.szsharing.cn

Swift .......... 15
来源：http://gp.chemitech.net.cn

Lua ............ 10
来源：http://lj.shxzukj.cn

Perl ........... 10
来源：http://fp.chemitech.net.cn

Scala .......... 10
来源：http://qk.haigaiapp.cn

------------------------------------
来源：http://cq.yuexingan06.cn

合计 ........... 2106 条
来源：http://es.shtwfgs.cn

按章节统计：
来源：http://nx.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://no.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bp.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rg.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dg.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fe.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ot.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ju.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tv.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ha.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ge.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zb.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hd.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ye.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ne.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fb.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://po.huanxung.cn

Q SQL 专题                              90
来源：http://rj.9csxet.cn

R Bash 专题                             80
来源：http://aa.yuexingan06.cn

S C / C++ 专题                          60
来源：http://dt.newstarts.cn

T 其他语言补充                          60
来源：http://xk.haigaiapp.cn

U 高频实用片段                         120
来源：http://ya.9csxet.cn

------------------------------------
来源：http://og.9csxet.cn

合计                                  2106 条
来源：http://ud.colortex.cn

--------------------------------------------------------------------------------
来源：http://ma.shxzskj.cn

使用提醒
来源：http://my.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://nz.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kq.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tb.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vf.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lo.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cy.gzmigu.cn

—— 文件结束 ——
来源：http://px.muxihuayi.cn

================================================================================
来源：http://bu.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://pn.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://jm.nicolike.cn

================================================================================
来源：http://sq.bjjhwx.cn

【收录内容】
来源：http://xt.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bd.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yw.szsharing.cn

SQL · Bash · C · C++
来源：http://oe.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wr.colortex.cn

【使用说明】
来源：http://bo.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pn.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nc.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pf.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gt.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mv.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ao.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nl.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bb.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vi.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xw.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qw.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pw.shxzukj.cn

【文件统计】
来源：http://ns.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lz.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://oy.szsharing.cn

目  录
来源：http://fm.9csxet.cn

--------------------------------------------------------------------------------
来源：http://xg.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vl.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dv.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zf.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qz.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ir.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pl.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iz.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kx.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ff.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lo.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dm.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lg.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jk.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rs.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tf.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sl.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vr.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tt.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mn.yuexingan06.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pi.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lc.shxzukj.cn

================================================================================
来源：http://ve.yuexingan06.cn

A. 基础语法与类型
来源：http://va.asd995.cn

================================================================================
来源：http://zp.bookmarksfly.cn

[A01] Hello World
来源：http://pd.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://tk.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://hz.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://cu.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lk.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://oh.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://bo.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://ae.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cr.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://mq.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kr.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mw.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gr.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://um.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://xf.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://ke.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://fm.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xx.nicolike.cn

[A03] 常量定义
来源：http://fb.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dj.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://ux.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://qm.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://xg.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://ls.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://ya.szxytkj.cn

Ruby: PI = 3.14159
来源：http://lt.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://na.hnjuh.cn

[A04] 判断变量类型
来源：http://do.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wk.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fn.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tn.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://ii.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vl.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yb.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://te.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://xy.bjjhwx.cn

[A05] 整数除法与取模
来源：http://bc.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mj.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dd.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ff.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cf.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://jp.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://nr.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://ld.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://rw.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://bb.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://rg.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qe.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://va.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pj.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jh.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://af.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pf.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aa.bookmarksfly.cn

[A07] 数字转字符串
来源：http://vk.shxzukj.cn

Py:   str(42)
来源：http://kk.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://ng.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://dg.wgjwhj.cn

TS:   String(42)
来源：http://xn.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dn.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://uf.hahajie.cn

Ruby: 42.to_s
来源：http://qb.jctech888.com.cn

C#:   42.ToString()
来源：http://sp.hahajie.cn

[A08] 取整与四舍五入
来源：http://bz.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ph.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qz.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ea.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ye.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gl.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xd.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://im.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fm.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://if.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ke.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oj.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wr.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vy.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xy.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oh.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cn.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ff.newstarts.cn

[A10] 生成随机数
来源：http://za.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://tt.521024.cn

PHP:  random_int(1, 100);
来源：http://xu.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kc.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ts.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ic.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ok.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://xm.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://ch.huanxung.cn

[A11] 条件表达式（三元）
来源：http://tv.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://pg.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://od.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rn.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qg.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://go.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://za.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qb.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ey.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://hd.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kt.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nz.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://eq.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://mo.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://dc.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hr.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://mk.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://so.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kd.huanxung.cn

Py:   "第一行\n第二行"
来源：http://pc.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://wq.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://tp.521024.cn

TS:   "第一行\n第二行"
来源：http://ko.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://ws.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://yq.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://fq.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://mi.haigaiapp.cn

[A14] 注释写法
来源：http://xi.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wv.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fb.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://qp.huixinmuqiang.cn


<!-- 参考信息 -->