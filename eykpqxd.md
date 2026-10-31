代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://cl.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gf.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://bf.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vy.huixinmuqiang.cn

[U85] JS：可选链
来源：http://sm.nicolike.cn

a?.b?.c
来源：http://sh.muxihuayi.cn

[U86] JS：空值合并
来源：http://pi.panjiajie.cn

a ?? b
来源：http://pg.jctech888.com.cn

[U87] JS：解构默认值
来源：http://gi.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://gi.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://uo.lnxyls.cn

{ ...a, ...b }
来源：http://qh.panjiajie.cn

[U89] JS：数组去重
来源：http://yc.chemitech.net.cn

[...new Set(arr)]
来源：http://hk.shxzskj.cn

[U90] JS：数字数组排序
来源：http://nn.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://se.szsharing.cn

[U91] JS：对象键值遍历
来源：http://ad.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ek.yuexingan06.cn

[U92] JS：深拷贝
来源：http://pk.yuexingan06.cn

structuredClone(obj)
来源：http://jc.asd995.cn

[U93] JS：模板字符串
来源：http://zc.panjiajie.cn

`共 ${n} 条`
来源：http://vz.huixiangedu.cn

[U94] JS：箭头函数
来源：http://tf.9csxet.cn

const double = x => x * 2;
来源：http://cy.newstarts.cn

[U95] JS：Promise 包装
来源：http://il.521024.cn

new Promise((resolve, reject) => {})
来源：http://uo.9csxet.cn

[U96] JS：async/await 与异常
来源：http://ik.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vy.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://ow.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sr.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://hh.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gv.bjjhwx.cn

[U99] JS：事件监听
来源：http://wv.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://bf.nicolike.cn

[U100] JS：DOM 查询
来源：http://ge.wgjwhj.cn

document.querySelector(".item")
来源：http://dh.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://ni.gzmigu.cn

el.classList.toggle("active")
来源：http://vy.shxzskj.cn

[U102] JS：本地存储
来源：http://hd.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gv.huixiangedu.cn

[U103] JS：定时器
来源：http://jb.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nx.yuntaijiaju.cn

[U104] JS：防抖
来源：http://gp.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xb.gzmigu.cn

[U105] JS：节流
来源：http://ou.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dp.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://lo.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ty.panjiajie.cn

[U107] JS：数字千分位
来源：http://dc.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rj.wgjwhj.cn

[U108] JS：随机整数
来源：http://jp.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://og.nicolike.cn

[U109] JS：数组分组
来源：http://ev.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://dv.szsharing.cn

[U110] JS：数组分块
来源：http://yi.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ex.shxzskj.cn

[U111] JS：对象转 Map
来源：http://rh.asd995.cn

new Map(Object.entries(obj))
来源：http://ad.hnjuh.cn

[U112] JS：字符串补位
来源：http://yy.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://jy.521024.cn

[U113] JS：正则替换全部
来源：http://xy.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://js.newstarts.cn

[U114] JS：JSON 深比较
来源：http://cx.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hs.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://ou.huixiangedu.cn

crypto.randomUUID()
来源：http://sm.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://mf.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://me.asd995.cn

[U117] JS：单元测试
来源：http://qj.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://xk.hnjuh.cn

[U118] JS：开发服务器
来源：http://fy.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://qk.chemitech.net.cn

[U119] JS：生产构建
来源：http://dc.nszjky.cn

npx vite build
来源：http://rw.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://sk.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://tb.jctech888.com.cn

================================================================================
来源：http://ku.szsharing.cn

统计汇总
来源：http://do.shtwfgs.cn

================================================================================
来源：http://cv.wgjwhj.cn

按语言统计（条）：
来源：http://hg.newstarts.cn

Python ......... 252
来源：http://nt.muxihuayi.cn

PHP ............ 252
来源：http://pd.haigaiapp.cn

JavaScript ..... 252
来源：http://ft.wgjwhj.cn

TypeScript ..... 212
来源：http://iz.shxzukj.cn

Java ........... 212
来源：http://ip.muxihuayi.cn

Go ............. 212
来源：http://yg.bjjhwx.cn

Ruby ........... 212
来源：http://zk.huixiangedu.cn

C# ............. 212
来源：http://rn.huixiangedu.cn

C .............. 30
来源：http://uv.newstarts.cn

C++ ............ 30
来源：http://cw.hahajie.cn

SQL ............ 90
来源：http://ah.haigaiapp.cn

Bash ........... 80
来源：http://sb.szsharing.cn

Kotlin ......... 15
来源：http://qc.hahajie.cn

Swift .......... 15
来源：http://me.yuntaijiaju.cn

Lua ............ 10
来源：http://fi.haigaiapp.cn

Perl ........... 10
来源：http://sv.gzmigu.cn

Scala .......... 10
来源：http://lo.chemitech.net.cn

------------------------------------
来源：http://ns.bjjhwx.cn

合计 ........... 2106 条
来源：http://fv.521024.cn

按章节统计：
来源：http://hy.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qr.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cf.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fl.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ax.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ff.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bk.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xa.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rh.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jg.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dv.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wa.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ae.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bw.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iy.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rv.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qt.nicolike.cn

Q SQL 专题                              90
来源：http://bl.chemitech.net.cn

R Bash 专题                             80
来源：http://gh.gzmigu.cn

S C / C++ 专题                          60
来源：http://sh.bjjhwx.cn

T 其他语言补充                          60
来源：http://qs.shtwfgs.cn

U 高频实用片段                         120
来源：http://fq.wgjwhj.cn

------------------------------------
来源：http://rj.yuntaijiaju.cn

合计                                  2106 条
来源：http://uf.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://sq.hnjuh.cn

使用提醒
来源：http://gg.huanxung.cn

--------------------------------------------------------------------------------
来源：http://oa.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pw.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bu.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wm.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cj.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vo.521024.cn

—— 文件结束 ——
来源：http://iv.yuexingan06.cn

================================================================================
来源：http://ib.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://br.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://hf.huixinmuqiang.cn

================================================================================
来源：http://yh.yuntaijiaju.cn

【收录内容】
来源：http://bo.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ok.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qx.szxytkj.cn

SQL · Bash · C · C++
来源：http://xx.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xv.asd995.cn

【使用说明】
来源：http://jr.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cw.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kq.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sh.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xt.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ss.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jx.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://od.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qt.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ff.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cq.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qq.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://in.muxihuayi.cn

【文件统计】
来源：http://ar.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gm.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://vn.gzmigu.cn

目  录
来源：http://al.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://uq.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jo.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vt.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hn.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://la.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lu.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fw.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rd.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xt.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ej.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gf.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vb.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ww.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wt.huixiangedu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xw.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rk.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ev.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://do.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ro.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pn.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jf.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://io.521024.cn

================================================================================
来源：http://bx.shxzskj.cn

A. 基础语法与类型
来源：http://qh.wgjwhj.cn

================================================================================
来源：http://wa.9csxet.cn

[A01] Hello World
来源：http://ly.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://qz.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://hv.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://wg.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ut.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://gv.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://of.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://yx.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dv.shxzskj.cn

[A02] 变量声明与赋值
来源：http://ug.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hh.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oa.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rq.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://su.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://jy.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://ff.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://pb.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oo.jianghongdianzi.cn

[A03] 常量定义
来源：http://cy.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lo.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://ut.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://hm.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://zm.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://qc.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://ep.szsharing.cn

Ruby: PI = 3.14159
来源：http://by.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://dy.bjjhwx.cn

[A04] 判断变量类型
来源：http://zp.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vy.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hg.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dr.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://jp.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lg.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oy.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wq.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://so.colortex.cn

[A05] 整数除法与取模
来源：http://ym.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gt.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sw.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vv.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dj.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://qc.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://aj.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://jk.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://wq.szsharing.cn

[A06] 字符串转数字
来源：http://lp.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://ih.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sb.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ss.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kh.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qn.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gd.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://um.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wf.hnjuh.cn

[A07] 数字转字符串
来源：http://mt.muxihuayi.cn

Py:   str(42)
来源：http://ds.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://im.asd995.cn

JS:   String(42); (42).toString()
来源：http://rd.jianghongdianzi.cn

TS:   String(42)
来源：http://co.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yu.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://xj.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://mt.jctech888.com.cn

C#:   42.ToString()
来源：http://zd.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://mr.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zo.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hu.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ty.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oc.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ry.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wm.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nh.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zw.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://dp.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ro.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oh.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nq.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yu.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pf.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xd.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qa.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ku.521024.cn

[A10] 生成随机数
来源：http://vp.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://vj.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://kd.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ag.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://el.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://ri.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://is.huixiangedu.cn

Ruby: rand(1..100)
来源：http://nf.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://cm.521024.cn

[A11] 条件表达式（三元）
来源：http://ya.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://rn.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nz.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pb.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yi.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://xh.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fj.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ab.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kc.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://op.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ez.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pk.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://ck.asd995.cn

TS:   `Hello, ${name}!`
来源：http://ub.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://tl.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ee.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://cn.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://rc.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lt.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://aq.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://di.asd995.cn

JS:   "第一行\n第二行"
来源：http://ek.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://rj.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://zx.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://ky.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://ax.newstarts.cn

C#:   "第一行\n第二行"
来源：http://ss.nicolike.cn


<!-- 参考信息 -->