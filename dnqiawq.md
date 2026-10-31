代发 wailian999

[U79] PHP：静态分析
来源：http://sj.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://yv.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://ux.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lh.szxytkj.cn

[U81] JS：初始化项目
来源：http://bn.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://vr.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://zi.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ay.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://pj.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bf.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://jm.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fe.9csxet.cn

[U85] JS：可选链
来源：http://bk.hahajie.cn

a?.b?.c
来源：http://hp.shxzskj.cn

[U86] JS：空值合并
来源：http://di.huixiangedu.cn

a ?? b
来源：http://ax.bjjhwx.cn

[U87] JS：解构默认值
来源：http://lg.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://tm.lnxyls.cn

[U88] JS：对象展开合并
来源：http://tw.hnjuh.cn

{ ...a, ...b }
来源：http://bo.muxihuayi.cn

[U89] JS：数组去重
来源：http://yy.521024.cn

[...new Set(arr)]
来源：http://dg.lnxyls.cn

[U90] JS：数字数组排序
来源：http://zx.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://dw.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://go.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mo.newstarts.cn

[U92] JS：深拷贝
来源：http://nh.haigaiapp.cn

structuredClone(obj)
来源：http://js.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://cx.szxytkj.cn

`共 ${n} 条`
来源：http://oq.521024.cn

[U94] JS：箭头函数
来源：http://kb.jianghongdianzi.cn

const double = x => x * 2;
来源：http://st.nszjky.cn

[U95] JS：Promise 包装
来源：http://xa.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://wj.newstarts.cn

[U96] JS：async/await 与异常
来源：http://de.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fl.nszjky.cn

[U97] JS：并发请求
来源：http://nz.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://py.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://xc.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ec.yuexingan06.cn

[U99] JS：事件监听
来源：http://wa.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://sw.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://mr.hnjuh.cn

document.querySelector(".item")
来源：http://xe.szsharing.cn

[U101] JS：classList 操作
来源：http://xw.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://cv.huanxung.cn

[U102] JS：本地存储
来源：http://mp.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qt.asd995.cn

[U103] JS：定时器
来源：http://gp.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xn.panjiajie.cn

[U104] JS：防抖
来源：http://if.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nv.panjiajie.cn

[U105] JS：节流
来源：http://xw.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vp.huixiangedu.cn

[U106] JS：日期格式化
来源：http://vy.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://em.szxytkj.cn

[U107] JS：数字千分位
来源：http://jl.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rs.gzmigu.cn

[U108] JS：随机整数
来源：http://ka.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tw.colortex.cn

[U109] JS：数组分组
来源：http://co.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://mw.shtwfgs.cn

[U110] JS：数组分块
来源：http://jl.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ny.colortex.cn

[U111] JS：对象转 Map
来源：http://sf.hahajie.cn

new Map(Object.entries(obj))
来源：http://jm.521024.cn

[U112] JS：字符串补位
来源：http://sb.panjiajie.cn

"7".padStart(3, "0")
来源：http://ut.nszjky.cn

[U113] JS：正则替换全部
来源：http://np.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://cb.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://zh.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://og.panjiajie.cn

[U115] JS：生成 UUID
来源：http://oo.huixiangedu.cn

crypto.randomUUID()
来源：http://an.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://gb.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://fz.521024.cn

[U117] JS：单元测试
来源：http://az.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://ow.9csxet.cn

[U118] JS：开发服务器
来源：http://wl.shxzukj.cn

npm i -D vite;  npx vite
来源：http://vn.huanxung.cn

[U119] JS：生产构建
来源：http://yz.chemitech.net.cn

npx vite build
来源：http://vo.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://of.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://rh.bookmarksfly.cn

================================================================================
来源：http://bh.colortex.cn

统计汇总
来源：http://ka.hnjuh.cn

================================================================================
来源：http://xf.bookmarksfly.cn

按语言统计（条）：
来源：http://xq.hnjuh.cn

Python ......... 252
来源：http://lb.gzmigu.cn

PHP ............ 252
来源：http://eb.9csxet.cn

JavaScript ..... 252
来源：http://jm.bjjhwx.cn

TypeScript ..... 212
来源：http://ou.wgjwhj.cn

Java ........... 212
来源：http://kd.huixiangedu.cn

Go ............. 212
来源：http://zr.asd995.cn

Ruby ........... 212
来源：http://hd.colortex.cn

C# ............. 212
来源：http://yn.shxzukj.cn

C .............. 30
来源：http://mk.shxzskj.cn

C++ ............ 30
来源：http://ic.bookmarksfly.cn

SQL ............ 90
来源：http://by.9csxet.cn

Bash ........... 80
来源：http://pv.shxzukj.cn

Kotlin ......... 15
来源：http://jh.jianghongdianzi.cn

Swift .......... 15
来源：http://mj.huixiangedu.cn

Lua ............ 10
来源：http://bm.jianghongdianzi.cn

Perl ........... 10
来源：http://ws.yuexingan06.cn

Scala .......... 10
来源：http://vf.shxzskj.cn

------------------------------------
来源：http://yi.gzmigu.cn

合计 ........... 2106 条
来源：http://bl.jctech888.com.cn

按章节统计：
来源：http://tc.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://na.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ai.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vw.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kb.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sa.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nb.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wj.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pk.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://io.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cx.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yw.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fz.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zx.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wp.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rp.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jj.shxzukj.cn

Q SQL 专题                              90
来源：http://hd.panjiajie.cn

R Bash 专题                             80
来源：http://rd.panjiajie.cn

S C / C++ 专题                          60
来源：http://ny.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://ej.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://ap.hahajie.cn

------------------------------------
来源：http://ph.nszjky.cn

合计                                  2106 条
来源：http://fs.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://xg.colortex.cn

使用提醒
来源：http://eb.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://dk.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dv.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vx.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://di.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lb.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cs.hnjuh.cn

—— 文件结束 ——
来源：http://lg.9csxet.cn

================================================================================
来源：http://hb.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://ew.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://qp.shxzukj.cn

================================================================================
来源：http://sz.jctech888.com.cn

【收录内容】
来源：http://fx.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vk.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ca.nicolike.cn

SQL · Bash · C · C++
来源：http://fe.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pp.shxzskj.cn

【使用说明】
来源：http://pg.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qi.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://il.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jc.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oc.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yy.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lk.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sp.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uw.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ha.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qe.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lg.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nz.9csxet.cn

【文件统计】
来源：http://ix.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mr.szsharing.cn

--------------------------------------------------------------------------------
来源：http://md.hnjuh.cn

目  录
来源：http://rz.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ip.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kr.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uj.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hw.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qv.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yg.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ru.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hv.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jg.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gv.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hc.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ru.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xh.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ha.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rp.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cj.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rz.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://no.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wi.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ff.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gq.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uk.lnxyls.cn

================================================================================
来源：http://qf.gzmigu.cn

A. 基础语法与类型
来源：http://ws.gzmigu.cn

================================================================================
来源：http://od.huixiangedu.cn

[A01] Hello World
来源：http://zk.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://vr.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://mw.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://xq.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dg.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://cd.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://xj.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://yy.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tj.newstarts.cn

[A02] 变量声明与赋值
来源：http://ya.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ma.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dq.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gb.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vs.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://oz.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://gg.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://qj.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kv.panjiajie.cn

[A03] 常量定义
来源：http://wv.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mm.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://kh.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://jb.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://iz.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://en.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://rk.asd995.cn

Ruby: PI = 3.14159
来源：http://ca.asd995.cn

C#:   const double PI = 3.14159;
来源：http://om.hahajie.cn

[A04] 判断变量类型
来源：http://zk.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kl.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xn.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ro.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://nh.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mg.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tu.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vt.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://aa.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://hb.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mj.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vk.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yz.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jk.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://sc.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://gz.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://cx.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://er.nszjky.cn

[A06] 字符串转数字
来源：http://al.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://cj.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://do.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ip.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jl.yuntaijiaju.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pp.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yn.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lg.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vt.bookmarksfly.cn

[A07] 数字转字符串
来源：http://sz.haigaiapp.cn

Py:   str(42)
来源：http://pe.521024.cn

PHP:  (string) 42; strval(42)
来源：http://mw.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://fu.bjjhwx.cn

TS:   String(42)
来源：http://sc.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eb.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://uh.wgjwhj.cn

Ruby: 42.to_s
来源：http://sk.jianghongdianzi.cn

C#:   42.ToString()
来源：http://la.hnjuh.cn

[A08] 取整与四舍五入
来源：http://xj.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://il.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gr.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mo.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jt.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hs.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pi.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ri.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wy.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://md.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://an.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ix.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tb.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ll.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gv.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vc.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yc.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eb.shxzukj.cn

[A10] 生成随机数
来源：http://yi.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://up.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://ns.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hc.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://de.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://ml.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fv.yuexingan06.cn

Ruby: rand(1..100)
来源：http://ay.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://rq.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://df.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://er.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rf.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bw.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lg.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://zb.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ti.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qr.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ee.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://pa.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lv.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xe.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://eg.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://fz.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://we.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://di.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ai.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://nf.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fv.gzmigu.cn


<!-- 参考信息 -->