代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://ix.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nd.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://ws.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mk.gzmigu.cn

[U85] JS：可选链
来源：http://si.gzmigu.cn

a?.b?.c
来源：http://cq.newstarts.cn

[U86] JS：空值合并
来源：http://cj.521024.cn

a ?? b
来源：http://ny.muxihuayi.cn

[U87] JS：解构默认值
来源：http://jd.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://zz.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://om.muxihuayi.cn

{ ...a, ...b }
来源：http://vt.shtwfgs.cn

[U89] JS：数组去重
来源：http://ty.chemitech.net.cn

[...new Set(arr)]
来源：http://bx.hahajie.cn

[U90] JS：数字数组排序
来源：http://jh.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://gj.521024.cn

[U91] JS：对象键值遍历
来源：http://mf.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://na.521024.cn

[U92] JS：深拷贝
来源：http://cw.nicolike.cn

structuredClone(obj)
来源：http://ze.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://rh.szxytkj.cn

`共 ${n} 条`
来源：http://bv.newstarts.cn

[U94] JS：箭头函数
来源：http://it.szsharing.cn

const double = x => x * 2;
来源：http://rc.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://dg.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://tn.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://ft.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vb.shxzskj.cn

[U97] JS：并发请求
来源：http://hj.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cj.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://uw.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tq.panjiajie.cn

[U99] JS：事件监听
来源：http://sp.asd995.cn

el.addEventListener("click", e => {})
来源：http://dq.colortex.cn

[U100] JS：DOM 查询
来源：http://ry.jianghongdianzi.cn

document.querySelector(".item")
来源：http://vr.9csxet.cn

[U101] JS：classList 操作
来源：http://yk.nicolike.cn

el.classList.toggle("active")
来源：http://ls.chemitech.net.cn

[U102] JS：本地存储
来源：http://pg.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cq.lnxyls.cn

[U103] JS：定时器
来源：http://yl.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pq.gzmigu.cn

[U104] JS：防抖
来源：http://kc.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ou.521024.cn

[U105] JS：节流
来源：http://xo.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://os.hahajie.cn

[U106] JS：日期格式化
来源：http://bc.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yu.jctech888.com.cn

[U107] JS：数字千分位
来源：http://mb.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://we.muxihuayi.cn

[U108] JS：随机整数
来源：http://tk.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cu.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://yp.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://ob.hnjuh.cn

[U110] JS：数组分块
来源：http://lf.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cf.shxzskj.cn

[U111] JS：对象转 Map
来源：http://wq.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://ws.gzmigu.cn

[U112] JS：字符串补位
来源：http://tl.jctech888.com.cn

"7".padStart(3, "0")
来源：http://uk.9csxet.cn

[U113] JS：正则替换全部
来源：http://wr.shxzskj.cn

s.replaceAll("a", "b")
来源：http://kt.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://qs.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gd.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://rp.muxihuayi.cn

crypto.randomUUID()
来源：http://hd.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://xf.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://wz.haigaiapp.cn

[U117] JS：单元测试
来源：http://pb.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://ot.nszjky.cn

[U118] JS：开发服务器
来源：http://bb.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://sw.panjiajie.cn

[U119] JS：生产构建
来源：http://wh.bookmarksfly.cn

npx vite build
来源：http://ve.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://nd.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://cc.szxytkj.cn

================================================================================
来源：http://rk.yuexingan06.cn

统计汇总
来源：http://fw.shxzukj.cn

================================================================================
来源：http://ma.shxzskj.cn

按语言统计（条）：
来源：http://dr.panjiajie.cn

Python ......... 252
来源：http://sc.panjiajie.cn

PHP ............ 252
来源：http://sz.newstarts.cn

JavaScript ..... 252
来源：http://jp.hnjuh.cn

TypeScript ..... 212
来源：http://lp.shtwfgs.cn

Java ........... 212
来源：http://hr.szxytkj.cn

Go ............. 212
来源：http://bj.yuexingan06.cn

Ruby ........... 212
来源：http://hi.shtwfgs.cn

C# ............. 212
来源：http://xs.yuntaijiaju.cn

C .............. 30
来源：http://fk.huixinmuqiang.cn

C++ ............ 30
来源：http://bv.shxzukj.cn

SQL ............ 90
来源：http://yo.bookmarksfly.cn

Bash ........... 80
来源：http://es.szxytkj.cn

Kotlin ......... 15
来源：http://kv.haigaiapp.cn

Swift .......... 15
来源：http://lx.shtwfgs.cn

Lua ............ 10
来源：http://eo.bjjhwx.cn

Perl ........... 10
来源：http://np.jctech888.com.cn

Scala .......... 10
来源：http://ff.colortex.cn

------------------------------------
来源：http://zo.shxzskj.cn

合计 ........... 2106 条
来源：http://bh.521024.cn

按章节统计：
来源：http://ou.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mq.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gl.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jm.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sz.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://do.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ur.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lq.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ql.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://il.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ha.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iz.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qt.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://do.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ws.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pj.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zw.lnxyls.cn

Q SQL 专题                              90
来源：http://cb.chemitech.net.cn

R Bash 专题                             80
来源：http://gg.asd995.cn

S C / C++ 专题                          60
来源：http://up.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://ld.lnxyls.cn

U 高频实用片段                         120
来源：http://ga.9csxet.cn

------------------------------------
来源：http://cm.haigaiapp.cn

合计                                  2106 条
来源：http://dn.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://pq.haigaiapp.cn

使用提醒
来源：http://wt.szsharing.cn

--------------------------------------------------------------------------------
来源：http://wh.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zc.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cr.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nd.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kc.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qa.bjjhwx.cn

—— 文件结束 ——
来源：http://gi.jctech888.com.cn

================================================================================
来源：http://ui.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://kj.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://gx.hnjuh.cn

================================================================================
来源：http://uz.521024.cn

【收录内容】
来源：http://zt.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tx.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lt.wgjwhj.cn

SQL · Bash · C · C++
来源：http://oq.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cf.bookmarksfly.cn

【使用说明】
来源：http://qh.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dj.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://os.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://in.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sy.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vi.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://go.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://el.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kf.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gp.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lm.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xt.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mq.panjiajie.cn

【文件统计】
来源：http://kd.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cq.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://yd.panjiajie.cn

目  录
来源：http://iz.asd995.cn

--------------------------------------------------------------------------------
来源：http://oo.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aw.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ax.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ku.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ux.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kb.nicolike.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vs.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xz.nicolike.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ud.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hn.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ee.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wd.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gn.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://od.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pq.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nw.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pu.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cw.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nt.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bm.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ci.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ib.szxytkj.cn

================================================================================
来源：http://yi.panjiajie.cn

A. 基础语法与类型
来源：http://hp.jianghongdianzi.cn

================================================================================
来源：http://ov.szxytkj.cn

[A01] Hello World
来源：http://bu.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://cv.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://zj.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://gz.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://we.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://ha.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://xd.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://ft.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sq.newstarts.cn

[A02] 变量声明与赋值
来源：http://xc.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sx.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kp.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qs.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xe.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://vn.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://lx.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://ay.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yc.lnxyls.cn

[A03] 常量定义
来源：http://kv.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kt.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://fj.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://qc.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://jn.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://na.shxzukj.cn

Go:   const PI = 3.14159
来源：http://nb.gzmigu.cn

Ruby: PI = 3.14159
来源：http://kr.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://gr.haigaiapp.cn

[A04] 判断变量类型
来源：http://pn.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xi.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vi.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ud.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://da.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mj.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oy.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tc.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://mh.shtwfgs.cn

[A05] 整数除法与取模
来源：http://vp.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fx.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rr.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bk.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://si.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://tb.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://mh.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://ve.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://ji.lnxyls.cn

[A06] 字符串转数字
来源：http://ok.521024.cn

Py:   int("42"); float("3.14")
来源：http://dr.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fz.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qw.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ey.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://db.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ve.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fi.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pf.huanxung.cn

[A07] 数字转字符串
来源：http://mo.huixiangedu.cn

Py:   str(42)
来源：http://ij.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://gy.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://jn.chemitech.net.cn

TS:   String(42)
来源：http://ip.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nr.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://gy.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://wy.shxzskj.cn

C#:   42.ToString()
来源：http://iq.521024.cn

[A08] 取整与四舍五入
来源：http://nt.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ve.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bc.yuntaijiaju.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ck.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jm.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fo.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lz.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jd.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cy.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://bd.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oe.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tr.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uf.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rt.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ws.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://et.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qf.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dc.jctech888.com.cn

[A10] 生成随机数
来源：http://gn.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://ib.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://vo.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uu.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nh.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://oc.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zu.hahajie.cn

Ruby: rand(1..100)
来源：http://av.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://hf.hahajie.cn

[A11] 条件表达式（三元）
来源：http://sg.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://wr.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fl.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uu.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ee.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://jr.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nl.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fs.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uv.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://vc.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xr.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mg.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://ux.colortex.cn

TS:   `Hello, ${name}!`
来源：http://zf.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://eq.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ii.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://jo.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://xv.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dc.newstarts.cn

Py:   "第一行\n第二行"
来源：http://li.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://ft.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://mp.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://yy.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://ed.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://ls.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://kd.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://zv.9csxet.cn


<!-- 参考信息 -->