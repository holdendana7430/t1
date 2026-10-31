代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://ha.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xm.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://nm.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xd.hnjuh.cn

[U85] JS：可选链
来源：http://ex.nszjky.cn

a?.b?.c
来源：http://xs.shtwfgs.cn

[U86] JS：空值合并
来源：http://rj.newstarts.cn

a ?? b
来源：http://lb.gzmigu.cn

[U87] JS：解构默认值
来源：http://op.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://wb.521024.cn

[U88] JS：对象展开合并
来源：http://ad.lnxyls.cn

{ ...a, ...b }
来源：http://ae.chemitech.net.cn

[U89] JS：数组去重
来源：http://yr.bookmarksfly.cn

[...new Set(arr)]
来源：http://iw.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://hp.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://hy.nszjky.cn

[U91] JS：对象键值遍历
来源：http://bs.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xn.shxzskj.cn

[U92] JS：深拷贝
来源：http://rf.wgjwhj.cn

structuredClone(obj)
来源：http://zc.wgjwhj.cn

[U93] JS：模板字符串
来源：http://ds.newstarts.cn

`共 ${n} 条`
来源：http://zy.haigaiapp.cn

[U94] JS：箭头函数
来源：http://or.colortex.cn

const double = x => x * 2;
来源：http://kr.nszjky.cn

[U95] JS：Promise 包装
来源：http://lf.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://wq.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://me.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zn.newstarts.cn

[U97] JS：并发请求
来源：http://db.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fl.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://rh.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wj.bookmarksfly.cn

[U99] JS：事件监听
来源：http://it.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://hp.9csxet.cn

[U100] JS：DOM 查询
来源：http://zq.gzmigu.cn

document.querySelector(".item")
来源：http://fn.bjjhwx.cn

[U101] JS：classList 操作
来源：http://qx.chemitech.net.cn

el.classList.toggle("active")
来源：http://yw.jctech888.com.cn

[U102] JS：本地存储
来源：http://jq.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lb.521024.cn

[U103] JS：定时器
来源：http://vy.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ly.shxzukj.cn

[U104] JS：防抖
来源：http://ip.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pq.521024.cn

[U105] JS：节流
来源：http://qe.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nh.9csxet.cn

[U106] JS：日期格式化
来源：http://pn.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://en.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://ma.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://li.huixiangedu.cn

[U108] JS：随机整数
来源：http://rs.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nm.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://mu.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://bo.9csxet.cn

[U110] JS：数组分块
来源：http://aa.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zl.asd995.cn

[U111] JS：对象转 Map
来源：http://fm.szsharing.cn

new Map(Object.entries(obj))
来源：http://io.szsharing.cn

[U112] JS：字符串补位
来源：http://zi.haigaiapp.cn

"7".padStart(3, "0")
来源：http://ry.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://ys.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://fn.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://rp.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vg.shxzskj.cn

[U115] JS：生成 UUID
来源：http://um.yuexingan06.cn

crypto.randomUUID()
来源：http://af.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://tq.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://uz.521024.cn

[U117] JS：单元测试
来源：http://fr.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://jm.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://tp.asd995.cn

npm i -D vite;  npx vite
来源：http://uq.9csxet.cn

[U119] JS：生产构建
来源：http://tq.hahajie.cn

npx vite build
来源：http://sm.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://gl.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://ze.newstarts.cn

================================================================================
来源：http://bx.bjjhwx.cn

统计汇总
来源：http://bb.panjiajie.cn

================================================================================
来源：http://qf.shtwfgs.cn

按语言统计（条）：
来源：http://lc.asd995.cn

Python ......... 252
来源：http://za.hahajie.cn

PHP ............ 252
来源：http://ux.yuntaijiaju.cn

JavaScript ..... 252
来源：http://xg.wgjwhj.cn

TypeScript ..... 212
来源：http://hh.colortex.cn

Java ........... 212
来源：http://ml.yuntaijiaju.cn

Go ............. 212
来源：http://oa.panjiajie.cn

Ruby ........... 212
来源：http://dr.panjiajie.cn

C# ............. 212
来源：http://vk.wgjwhj.cn

C .............. 30
来源：http://tq.shtwfgs.cn

C++ ............ 30
来源：http://we.nszjky.cn

SQL ............ 90
来源：http://pp.huanxung.cn

Bash ........... 80
来源：http://iy.szxytkj.cn

Kotlin ......... 15
来源：http://jn.szsharing.cn

Swift .......... 15
来源：http://qp.jctech888.com.cn

Lua ............ 10
来源：http://el.jianghongdianzi.cn

Perl ........... 10
来源：http://js.jctech888.com.cn

Scala .......... 10
来源：http://xp.newstarts.cn

------------------------------------
来源：http://ap.szsharing.cn

合计 ........... 2106 条
来源：http://iy.lnxyls.cn

按章节统计：
来源：http://fc.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kz.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oi.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qp.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zj.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pv.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ry.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hp.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hg.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fs.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ln.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vx.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qg.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nh.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ok.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pz.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lt.lnxyls.cn

Q SQL 专题                              90
来源：http://tx.521024.cn

R Bash 专题                             80
来源：http://cg.jctech888.com.cn

S C / C++ 专题                          60
来源：http://jf.nicolike.cn

T 其他语言补充                          60
来源：http://gy.gzmigu.cn

U 高频实用片段                         120
来源：http://hr.gzmigu.cn

------------------------------------
来源：http://tc.wgjwhj.cn

合计                                  2106 条
来源：http://jx.521024.cn

--------------------------------------------------------------------------------
来源：http://cy.9csxet.cn

使用提醒
来源：http://ll.521024.cn

--------------------------------------------------------------------------------
来源：http://if.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qr.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pi.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ta.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ih.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ox.muxihuayi.cn

—— 文件结束 ——
来源：http://qk.haigaiapp.cn

================================================================================
来源：http://jw.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://af.521024.cn

Common Programming Examples Cheat Book
来源：http://gv.hahajie.cn

================================================================================
来源：http://ls.huixinmuqiang.cn

【收录内容】
来源：http://vb.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tr.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rr.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://vr.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rq.huanxung.cn

【使用说明】
来源：http://ci.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://la.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uz.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pj.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rj.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fd.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://me.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jd.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gw.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aj.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gi.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wm.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gb.newstarts.cn

【文件统计】
来源：http://qx.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ap.asd995.cn

--------------------------------------------------------------------------------
来源：http://xi.hahajie.cn

目  录
来源：http://qn.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://hc.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ax.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://od.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iq.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ei.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://na.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ue.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://il.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wc.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mf.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qf.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fy.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qj.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wl.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fo.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://st.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ie.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fo.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cs.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://di.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eq.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://es.haigaiapp.cn

================================================================================
来源：http://dp.shxzukj.cn

A. 基础语法与类型
来源：http://py.jctech888.com.cn

================================================================================
来源：http://dy.colortex.cn

[A01] Hello World
来源：http://oo.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://hn.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://hp.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://df.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ac.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://fr.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://cw.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://sw.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qk.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://hh.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cz.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gb.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vw.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vs.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://ss.521024.cn

Go:   name := "Alex"; age := 20
来源：http://um.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://kt.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wd.jianghongdianzi.cn

[A03] 常量定义
来源：http://fv.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rn.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://kj.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://qj.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://at.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://ou.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://fa.9csxet.cn

Ruby: PI = 3.14159
来源：http://jk.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://ar.lnxyls.cn

[A04] 判断变量类型
来源：http://cc.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ep.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sf.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cs.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://ur.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qr.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cz.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vp.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://ox.chemitech.net.cn

[A05] 整数除法与取模
来源：http://rr.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kj.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qf.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pa.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yz.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://dx.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://zt.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://oe.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://as.chemitech.net.cn

[A06] 字符串转数字
来源：http://ur.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://uc.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zw.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nu.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ln.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cq.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mw.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wr.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://al.haigaiapp.cn

[A07] 数字转字符串
来源：http://jo.jctech888.com.cn

Py:   str(42)
来源：http://mq.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://pq.hahajie.cn

JS:   String(42); (42).toString()
来源：http://kc.colortex.cn

TS:   String(42)
来源：http://ik.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://is.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://wt.nicolike.cn

Ruby: 42.to_s
来源：http://ph.asd995.cn

C#:   42.ToString()
来源：http://rt.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://yp.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://im.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uv.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tv.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sr.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pr.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ke.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tn.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ny.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://zq.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gl.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fd.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://km.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://le.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nx.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mt.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ry.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kx.9csxet.cn

[A10] 生成随机数
来源：http://de.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://qv.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://ft.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oc.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://np.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://ja.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ds.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://pz.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://yc.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://tm.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://qn.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pj.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gd.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vn.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://vy.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cq.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sc.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hh.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://sj.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bh.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sw.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://ht.colortex.cn

TS:   `Hello, ${name}!`
来源：http://ve.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://uv.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fx.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://an.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://yu.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kz.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://em.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://dl.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://ln.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://qg.szxytkj.cn

Java: "第一行\n第二行"
来源：http://wz.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://co.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://rf.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://pe.jctech888.com.cn


<!-- 参考信息 -->