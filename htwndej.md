代发 wailian999

[U81] JS：初始化项目
来源：http://eu.gzmigu.cn

npm init -y;  npm i express
来源：http://pr.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://nj.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vj.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://mz.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oi.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://ki.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hd.muxihuayi.cn

[U85] JS：可选链
来源：http://pk.shtwfgs.cn

a?.b?.c
来源：http://bf.muxihuayi.cn

[U86] JS：空值合并
来源：http://sj.asd995.cn

a ?? b
来源：http://rs.bjjhwx.cn

[U87] JS：解构默认值
来源：http://kf.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://fw.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://us.jianghongdianzi.cn

{ ...a, ...b }
来源：http://pa.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://dd.jianghongdianzi.cn

[...new Set(arr)]
来源：http://rm.9csxet.cn

[U90] JS：数字数组排序
来源：http://de.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://rm.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://wr.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fb.gzmigu.cn

[U92] JS：深拷贝
来源：http://gs.lnxyls.cn

structuredClone(obj)
来源：http://xx.szsharing.cn

[U93] JS：模板字符串
来源：http://ts.bookmarksfly.cn

`共 ${n} 条`
来源：http://yi.haigaiapp.cn

[U94] JS：箭头函数
来源：http://nf.bookmarksfly.cn

const double = x => x * 2;
来源：http://xe.nszjky.cn

[U95] JS：Promise 包装
来源：http://dr.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://av.huanxung.cn

[U96] JS：async/await 与异常
来源：http://ki.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cc.panjiajie.cn

[U97] JS：并发请求
来源：http://bz.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yp.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://di.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ri.chemitech.net.cn

[U99] JS：事件监听
来源：http://vj.asd995.cn

el.addEventListener("click", e => {})
来源：http://fc.szsharing.cn

[U100] JS：DOM 查询
来源：http://rb.hahajie.cn

document.querySelector(".item")
来源：http://yh.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://fd.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://gv.shxzukj.cn

[U102] JS：本地存储
来源：http://fo.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ki.huixinmuqiang.cn

[U103] JS：定时器
来源：http://ep.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rm.chemitech.net.cn

[U104] JS：防抖
来源：http://vn.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vm.yuntaijiaju.cn

[U105] JS：节流
来源：http://iq.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jq.szsharing.cn

[U106] JS：日期格式化
来源：http://bo.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sx.chemitech.net.cn

[U107] JS：数字千分位
来源：http://ln.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://du.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://wt.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qi.chemitech.net.cn

[U109] JS：数组分组
来源：http://xq.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://vb.hahajie.cn

[U110] JS：数组分块
来源：http://vn.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uy.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://uq.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://tx.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://xg.yuexingan06.cn

"7".padStart(3, "0")
来源：http://za.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://va.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://au.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://il.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fu.shxzskj.cn

[U115] JS：生成 UUID
来源：http://sv.huanxung.cn

crypto.randomUUID()
来源：http://wx.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://ff.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://jl.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://lv.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://nh.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://ks.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://mv.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://vv.asd995.cn

npx vite build
来源：http://qb.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://yo.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://zk.szsharing.cn

================================================================================
来源：http://sd.huixinmuqiang.cn

统计汇总
来源：http://ag.yuntaijiaju.cn

================================================================================
来源：http://mi.chemitech.net.cn

按语言统计（条）：
来源：http://ts.nicolike.cn

Python ......... 252
来源：http://ar.huanxung.cn

PHP ............ 252
来源：http://fj.szxytkj.cn

JavaScript ..... 252
来源：http://ez.yuntaijiaju.cn

TypeScript ..... 212
来源：http://dk.huixinmuqiang.cn

Java ........... 212
来源：http://dn.colortex.cn

Go ............. 212
来源：http://xy.asd995.cn

Ruby ........... 212
来源：http://wg.shxzukj.cn

C# ............. 212
来源：http://jc.bjjhwx.cn

C .............. 30
来源：http://gv.shtwfgs.cn

C++ ............ 30
来源：http://uy.huanxung.cn

SQL ............ 90
来源：http://xb.panjiajie.cn

Bash ........... 80
来源：http://wj.muxihuayi.cn

Kotlin ......... 15
来源：http://tk.chemitech.net.cn

Swift .......... 15
来源：http://nm.szxytkj.cn

Lua ............ 10
来源：http://pg.521024.cn

Perl ........... 10
来源：http://tl.muxihuayi.cn

Scala .......... 10
来源：http://aq.haigaiapp.cn

------------------------------------
来源：http://so.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://vk.bookmarksfly.cn

按章节统计：
来源：http://rz.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vt.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://za.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dd.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nn.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cy.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oe.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://on.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yb.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pi.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bg.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vm.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fo.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qo.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pp.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lq.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xv.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://pa.nszjky.cn

R Bash 专题                             80
来源：http://nb.muxihuayi.cn

S C / C++ 专题                          60
来源：http://cs.bjjhwx.cn

T 其他语言补充                          60
来源：http://cd.shxzukj.cn

U 高频实用片段                         120
来源：http://ab.hnjuh.cn

------------------------------------
来源：http://dp.jianghongdianzi.cn

合计                                  2106 条
来源：http://ll.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ov.shtwfgs.cn

使用提醒
来源：http://vm.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://qb.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ar.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fn.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vo.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yt.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kx.bookmarksfly.cn

—— 文件结束 ——
来源：http://wh.newstarts.cn

================================================================================
来源：http://mp.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://dc.nszjky.cn

Common Programming Examples Cheat Book
来源：http://fo.panjiajie.cn

================================================================================
来源：http://dg.chemitech.net.cn

【收录内容】
来源：http://qr.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pi.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xt.haigaiapp.cn

SQL · Bash · C · C++
来源：http://ag.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gi.bookmarksfly.cn

【使用说明】
来源：http://fi.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://se.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hf.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dc.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cy.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zz.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vo.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yr.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jg.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eb.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://be.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eg.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hx.muxihuayi.cn

【文件统计】
来源：http://ah.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mr.9csxet.cn

--------------------------------------------------------------------------------
来源：http://eu.gzmigu.cn

目  录
来源：http://uy.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://im.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rh.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ka.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bi.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://py.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ll.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ll.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mq.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qi.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hp.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gx.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vm.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vr.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xq.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hr.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oo.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kz.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oc.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://st.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dx.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://js.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kt.9csxet.cn

================================================================================
来源：http://gl.panjiajie.cn

A. 基础语法与类型
来源：http://fj.shtwfgs.cn

================================================================================
来源：http://et.jctech888.com.cn

[A01] Hello World
来源：http://gt.nszjky.cn

Py:   print("Hello, World!")
来源：http://nj.colortex.cn

PHP:  echo "Hello, World!";
来源：http://jt.shxzukj.cn

JS:   console.log("Hello, World!");
来源：http://vd.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kc.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://vm.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://mi.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://lj.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yv.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://uz.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jl.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fk.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gg.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jx.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://by.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://nn.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://tq.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://er.chemitech.net.cn

[A03] 常量定义
来源：http://wo.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lb.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://di.nszjky.cn

JS:   const PI = 3.14159;
来源：http://lv.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://ai.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://ik.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://jo.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://aq.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://pg.gzmigu.cn

[A04] 判断变量类型
来源：http://fm.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dl.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uc.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ti.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://zs.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://aj.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dm.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://om.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://zg.lnxyls.cn

[A05] 整数除法与取模
来源：http://mz.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ta.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ed.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://du.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://em.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://qh.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://ih.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://gl.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://lb.nszjky.cn

[A06] 字符串转数字
来源：http://ch.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://xi.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ly.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://av.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qt.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rx.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sl.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vm.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oz.jctech888.com.cn

[A07] 数字转字符串
来源：http://mf.panjiajie.cn

Py:   str(42)
来源：http://ua.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://lq.huanxung.cn

JS:   String(42); (42).toString()
来源：http://od.wgjwhj.cn

TS:   String(42)
来源：http://nq.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cz.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://ze.szsharing.cn

Ruby: 42.to_s
来源：http://lm.szxytkj.cn

C#:   42.ToString()
来源：http://fh.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://vc.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gs.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wq.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://br.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://av.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dt.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mx.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jx.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zk.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://xk.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fk.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ih.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xd.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yh.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nu.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ye.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lh.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ol.hnjuh.cn

[A10] 生成随机数
来源：http://xb.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://cp.asd995.cn

PHP:  random_int(1, 100);
来源：http://wb.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jd.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gq.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://vh.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mz.szsharing.cn

Ruby: rand(1..100)
来源：http://qo.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://tb.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://eo.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://uj.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jr.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gf.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iu.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://ci.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fr.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bu.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ba.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://fm.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bw.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wn.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://lz.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://up.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://rv.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uv.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://gf.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://zu.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zh.nszjky.cn

Py:   "第一行\n第二行"
来源：http://bz.521024.cn

PHP:  "第一行\n第二行"
来源：http://mt.9csxet.cn

JS:   "第一行\n第二行"
来源：http://cn.nszjky.cn

TS:   "第一行\n第二行"
来源：http://tn.muxihuayi.cn


<!-- 参考信息 -->