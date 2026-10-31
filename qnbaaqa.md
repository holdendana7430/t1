代发 wailian999

[U77] PHP：模板渲染
来源：http://bv.huixiangedu.cn

composer require twig/twig
来源：http://ke.jctech888.com.cn

[U78] PHP：单元测试
来源：http://wv.521024.cn

composer require --dev phpunit/phpunit
来源：http://zh.huixiangedu.cn

[U79] PHP：静态分析
来源：http://cd.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://wj.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://hz.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jh.yuexingan06.cn

[U81] JS：初始化项目
来源：http://cu.9csxet.cn

npm init -y;  npm i express
来源：http://rc.nszjky.cn

[U82] JS：package.json 脚本
来源：http://my.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ca.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://gt.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pq.521024.cn

[U84] JS：CommonJS 写法
来源：http://zn.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qj.bjjhwx.cn

[U85] JS：可选链
来源：http://te.muxihuayi.cn

a?.b?.c
来源：http://bq.jctech888.com.cn

[U86] JS：空值合并
来源：http://kx.huixiangedu.cn

a ?? b
来源：http://wa.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ki.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://af.colortex.cn

[U88] JS：对象展开合并
来源：http://hf.hahajie.cn

{ ...a, ...b }
来源：http://ak.huixiangedu.cn

[U89] JS：数组去重
来源：http://py.newstarts.cn

[...new Set(arr)]
来源：http://wj.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ca.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://dl.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://ko.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wj.newstarts.cn

[U92] JS：深拷贝
来源：http://ct.yuntaijiaju.cn

structuredClone(obj)
来源：http://id.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://av.muxihuayi.cn

`共 ${n} 条`
来源：http://iz.bjjhwx.cn

[U94] JS：箭头函数
来源：http://hm.lnxyls.cn

const double = x => x * 2;
来源：http://ho.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://ov.asd995.cn

new Promise((resolve, reject) => {})
来源：http://mi.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://dk.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sr.9csxet.cn

[U97] JS：并发请求
来源：http://dd.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mj.521024.cn

[U98] JS：fetch 带 JSON
来源：http://mj.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ff.chemitech.net.cn

[U99] JS：事件监听
来源：http://gv.newstarts.cn

el.addEventListener("click", e => {})
来源：http://uz.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://yi.muxihuayi.cn

document.querySelector(".item")
来源：http://mt.chemitech.net.cn

[U101] JS：classList 操作
来源：http://ct.9csxet.cn

el.classList.toggle("active")
来源：http://qu.hnjuh.cn

[U102] JS：本地存储
来源：http://di.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ds.shxzskj.cn

[U103] JS：定时器
来源：http://ec.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pc.shtwfgs.cn

[U104] JS：防抖
来源：http://hd.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fn.jctech888.com.cn

[U105] JS：节流
来源：http://xm.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ls.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://ui.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ua.asd995.cn

[U107] JS：数字千分位
来源：http://jy.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ld.shxzskj.cn

[U108] JS：随机整数
来源：http://lp.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://et.asd995.cn

[U109] JS：数组分组
来源：http://fx.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://sc.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://fc.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pu.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://wn.nszjky.cn

new Map(Object.entries(obj))
来源：http://sb.muxihuayi.cn

[U112] JS：字符串补位
来源：http://hd.panjiajie.cn

"7".padStart(3, "0")
来源：http://un.lnxyls.cn

[U113] JS：正则替换全部
来源：http://je.hahajie.cn

s.replaceAll("a", "b")
来源：http://vg.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://lm.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vn.newstarts.cn

[U115] JS：生成 UUID
来源：http://jx.gzmigu.cn

crypto.randomUUID()
来源：http://fl.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://bb.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://uq.nicolike.cn

[U117] JS：单元测试
来源：http://oa.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://ce.hahajie.cn

[U118] JS：开发服务器
来源：http://nq.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://xf.asd995.cn

[U119] JS：生产构建
来源：http://uz.wgjwhj.cn

npx vite build
来源：http://rk.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://ry.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://qw.yuexingan06.cn

================================================================================
来源：http://nw.bjjhwx.cn

统计汇总
来源：http://ff.szsharing.cn

================================================================================
来源：http://jo.colortex.cn

按语言统计（条）：
来源：http://zn.shxzskj.cn

Python ......... 252
来源：http://eb.wgjwhj.cn

PHP ............ 252
来源：http://xh.asd995.cn

JavaScript ..... 252
来源：http://ld.chemitech.net.cn

TypeScript ..... 212
来源：http://dw.szsharing.cn

Java ........... 212
来源：http://go.hahajie.cn

Go ............. 212
来源：http://fq.newstarts.cn

Ruby ........... 212
来源：http://kh.lnxyls.cn

C# ............. 212
来源：http://wc.yuntaijiaju.cn

C .............. 30
来源：http://ts.haigaiapp.cn

C++ ............ 30
来源：http://jc.huanxung.cn

SQL ............ 90
来源：http://bg.shtwfgs.cn

Bash ........... 80
来源：http://rc.panjiajie.cn

Kotlin ......... 15
来源：http://qx.shtwfgs.cn

Swift .......... 15
来源：http://qe.haigaiapp.cn

Lua ............ 10
来源：http://jh.huanxung.cn

Perl ........... 10
来源：http://ux.huixiangedu.cn

Scala .......... 10
来源：http://mn.newstarts.cn

------------------------------------
来源：http://te.asd995.cn

合计 ........... 2106 条
来源：http://ft.colortex.cn

按章节统计：
来源：http://ge.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://by.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kc.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://an.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pz.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eu.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://up.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dq.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pl.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dn.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gf.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bo.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nk.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qq.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gf.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ei.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qx.colortex.cn

Q SQL 专题                              90
来源：http://ib.9csxet.cn

R Bash 专题                             80
来源：http://wf.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://yy.521024.cn

T 其他语言补充                          60
来源：http://am.hahajie.cn

U 高频实用片段                         120
来源：http://sr.shxzukj.cn

------------------------------------
来源：http://mh.szxytkj.cn

合计                                  2106 条
来源：http://is.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://zy.lnxyls.cn

使用提醒
来源：http://xf.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://kf.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mi.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oa.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tn.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rv.newstarts.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tm.521024.cn

—— 文件结束 ——
来源：http://mo.huixiangedu.cn

================================================================================
来源：http://ky.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://tw.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://wk.bjjhwx.cn

================================================================================
来源：http://mi.hnjuh.cn

【收录内容】
来源：http://wg.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cb.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yc.huanxung.cn

SQL · Bash · C · C++
来源：http://fi.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xb.colortex.cn

【使用说明】
来源：http://xd.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rg.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bh.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qt.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yv.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bz.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rc.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mb.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hk.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wd.gzmigu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pk.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wv.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ei.huanxung.cn

【文件统计】
来源：http://oz.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rv.nszjky.cn

--------------------------------------------------------------------------------
来源：http://vv.jctech888.com.cn

目  录
来源：http://xb.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ul.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mz.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bq.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://be.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yy.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vu.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gf.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://no.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ew.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zt.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yo.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hf.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wo.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ps.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://br.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vj.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xf.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ii.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ol.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aw.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lm.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hb.lnxyls.cn

================================================================================
来源：http://nu.jctech888.com.cn

A. 基础语法与类型
来源：http://yv.jianghongdianzi.cn

================================================================================
来源：http://vd.asd995.cn

[A01] Hello World
来源：http://cc.newstarts.cn

Py:   print("Hello, World!")
来源：http://ln.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://qj.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://yf.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://za.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://wz.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://wt.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://te.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uv.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://wy.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ew.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ge.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vu.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eb.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://ye.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://sw.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://wu.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jm.wgjwhj.cn

[A03] 常量定义
来源：http://mh.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tx.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://lz.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://xj.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://fh.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://sj.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://uh.szxytkj.cn

Ruby: PI = 3.14159
来源：http://ev.521024.cn

C#:   const double PI = 3.14159;
来源：http://lv.gzmigu.cn

[A04] 判断变量类型
来源：http://ng.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gr.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fb.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wz.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://ty.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iu.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ub.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rm.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://bi.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://fc.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ry.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://it.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xj.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eu.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://io.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://im.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://ps.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://qi.chemitech.net.cn

[A06] 字符串转数字
来源：http://td.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://ar.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gr.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ih.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lu.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nk.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xm.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hs.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rn.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://ri.yuexingan06.cn

Py:   str(42)
来源：http://mz.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://fa.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://gq.hahajie.cn

TS:   String(42)
来源：http://ud.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pj.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://qf.panjiajie.cn

Ruby: 42.to_s
来源：http://yo.nszjky.cn

C#:   42.ToString()
来源：http://tu.521024.cn

[A08] 取整与四舍五入
来源：http://ol.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dl.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xd.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qx.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dz.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ni.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://av.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sk.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kd.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://tm.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lw.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qa.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cm.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zt.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oo.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qb.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ba.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pe.nicolike.cn

[A10] 生成随机数
来源：http://py.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://sw.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://xw.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ni.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ju.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://xu.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nl.haigaiapp.cn

Ruby: rand(1..100)
来源：http://dr.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://lt.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://le.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://qg.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fd.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pa.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hv.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ru.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dn.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ro.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bu.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://pa.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bh.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://am.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://vf.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://lz.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://ec.huixiangedu.cn


<!-- 参考信息 -->