代发 wailian999

[U75] PHP：依赖注入
来源：http://yz.huanxung.cn

composer require psr/container
来源：http://lu.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://hl.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wj.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://ar.colortex.cn

composer require twig/twig
来源：http://mf.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://zy.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://fz.gzmigu.cn

[U79] PHP：静态分析
来源：http://tb.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://gs.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://zh.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://to.nicolike.cn

[U81] JS：初始化项目
来源：http://tc.wgjwhj.cn

npm init -y;  npm i express
来源：http://nd.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://gk.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ns.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://lr.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eq.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://li.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wx.jctech888.com.cn

[U85] JS：可选链
来源：http://ns.lnxyls.cn

a?.b?.c
来源：http://hw.hnjuh.cn

[U86] JS：空值合并
来源：http://ir.shxzukj.cn

a ?? b
来源：http://zr.lnxyls.cn

[U87] JS：解构默认值
来源：http://ji.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://vr.nicolike.cn

[U88] JS：对象展开合并
来源：http://sg.panjiajie.cn

{ ...a, ...b }
来源：http://ce.shxzskj.cn

[U89] JS：数组去重
来源：http://ev.asd995.cn

[...new Set(arr)]
来源：http://wc.nszjky.cn

[U90] JS：数字数组排序
来源：http://xp.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://oj.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://xi.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lk.chemitech.net.cn

[U92] JS：深拷贝
来源：http://vk.panjiajie.cn

structuredClone(obj)
来源：http://dr.hnjuh.cn

[U93] JS：模板字符串
来源：http://cs.newstarts.cn

`共 ${n} 条`
来源：http://xz.newstarts.cn

[U94] JS：箭头函数
来源：http://ho.9csxet.cn

const double = x => x * 2;
来源：http://kc.nicolike.cn

[U95] JS：Promise 包装
来源：http://yb.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://vf.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://un.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kn.huanxung.cn

[U97] JS：并发请求
来源：http://xm.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hc.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://hb.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nf.panjiajie.cn

[U99] JS：事件监听
来源：http://yp.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://aq.hahajie.cn

[U100] JS：DOM 查询
来源：http://qy.colortex.cn

document.querySelector(".item")
来源：http://cc.hnjuh.cn

[U101] JS：classList 操作
来源：http://tu.wgjwhj.cn

el.classList.toggle("active")
来源：http://xa.muxihuayi.cn

[U102] JS：本地存储
来源：http://wj.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tu.9csxet.cn

[U103] JS：定时器
来源：http://ux.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eb.hahajie.cn

[U104] JS：防抖
来源：http://tv.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://db.huanxung.cn

[U105] JS：节流
来源：http://ez.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zb.nicolike.cn

[U106] JS：日期格式化
来源：http://ih.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dh.shxzukj.cn

[U107] JS：数字千分位
来源：http://ql.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yq.asd995.cn

[U108] JS：随机整数
来源：http://mx.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rd.jctech888.com.cn

[U109] JS：数组分组
来源：http://uq.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://xv.lnxyls.cn

[U110] JS：数组分块
来源：http://xj.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rm.asd995.cn

[U111] JS：对象转 Map
来源：http://qs.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://uv.lnxyls.cn

[U112] JS：字符串补位
来源：http://zj.colortex.cn

"7".padStart(3, "0")
来源：http://xl.szsharing.cn

[U113] JS：正则替换全部
来源：http://dz.panjiajie.cn

s.replaceAll("a", "b")
来源：http://pn.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://dx.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xr.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://ae.muxihuayi.cn

crypto.randomUUID()
来源：http://nt.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ks.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://sm.huixiangedu.cn

[U117] JS：单元测试
来源：http://bl.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://hi.nszjky.cn

[U118] JS：开发服务器
来源：http://ch.nicolike.cn

npm i -D vite;  npx vite
来源：http://qj.colortex.cn

[U119] JS：生产构建
来源：http://wa.521024.cn

npx vite build
来源：http://vj.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://cx.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://um.szxytkj.cn

================================================================================
来源：http://yi.lnxyls.cn

统计汇总
来源：http://dy.szxytkj.cn

================================================================================
来源：http://ir.yuexingan06.cn

按语言统计（条）：
来源：http://pl.asd995.cn

Python ......... 252
来源：http://yf.asd995.cn

PHP ............ 252
来源：http://qw.hnjuh.cn

JavaScript ..... 252
来源：http://xl.shxzskj.cn

TypeScript ..... 212
来源：http://hw.muxihuayi.cn

Java ........... 212
来源：http://ny.jctech888.com.cn

Go ............. 212
来源：http://ai.521024.cn

Ruby ........... 212
来源：http://mg.yuntaijiaju.cn

C# ............. 212
来源：http://yd.nicolike.cn

C .............. 30
来源：http://nu.bjjhwx.cn

C++ ............ 30
来源：http://sa.szxytkj.cn

SQL ............ 90
来源：http://ew.9csxet.cn

Bash ........... 80
来源：http://ua.szxytkj.cn

Kotlin ......... 15
来源：http://tg.huixiangedu.cn

Swift .......... 15
来源：http://nz.yuntaijiaju.cn

Lua ............ 10
来源：http://xv.nszjky.cn

Perl ........... 10
来源：http://sr.shxzukj.cn

Scala .......... 10
来源：http://oi.hnjuh.cn

------------------------------------
来源：http://zg.asd995.cn

合计 ........... 2106 条
来源：http://vn.szxytkj.cn

按章节统计：
来源：http://qz.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gx.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hx.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jx.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ji.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fg.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xe.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tz.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ox.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kz.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ro.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eu.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ko.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iv.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yo.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cz.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zh.jctech888.com.cn

Q SQL 专题                              90
来源：http://rn.jctech888.com.cn

R Bash 专题                             80
来源：http://rc.wgjwhj.cn

S C / C++ 专题                          60
来源：http://iq.colortex.cn

T 其他语言补充                          60
来源：http://fu.yuexingan06.cn

U 高频实用片段                         120
来源：http://lb.asd995.cn

------------------------------------
来源：http://fg.huixinmuqiang.cn

合计                                  2106 条
来源：http://ag.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ac.bookmarksfly.cn

使用提醒
来源：http://fz.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://aj.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jr.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mx.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lw.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qs.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nf.shtwfgs.cn

—— 文件结束 ——
来源：http://yb.yuexingan06.cn

================================================================================
来源：http://ta.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://br.huanxung.cn

Common Programming Examples Cheat Book
来源：http://tz.chemitech.net.cn

================================================================================
来源：http://vd.newstarts.cn

【收录内容】
来源：http://pn.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dv.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bq.yuexingan06.cn

SQL · Bash · C · C++
来源：http://tn.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://db.shxzskj.cn

【使用说明】
来源：http://bu.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vk.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tb.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zc.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ah.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bv.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zk.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uf.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yx.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ey.szxytkj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gd.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ol.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qs.nicolike.cn

【文件统计】
来源：http://xs.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sl.nicolike.cn

--------------------------------------------------------------------------------
来源：http://nd.bookmarksfly.cn

目  录
来源：http://ez.szsharing.cn

--------------------------------------------------------------------------------
来源：http://kb.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://al.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://za.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hj.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gf.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kz.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iv.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rt.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sq.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dv.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iy.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qj.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://of.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dk.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kp.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kv.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tf.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sq.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lg.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hh.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bj.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://or.chemitech.net.cn

================================================================================
来源：http://re.szxytkj.cn

A. 基础语法与类型
来源：http://xs.gzmigu.cn

================================================================================
来源：http://ju.chemitech.net.cn

[A01] Hello World
来源：http://uf.gzmigu.cn

Py:   print("Hello, World!")
来源：http://nv.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://uq.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://fs.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hq.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://xq.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://tj.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://qg.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vs.shxzskj.cn

[A02] 变量声明与赋值
来源：http://wt.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tm.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bz.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ou.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pa.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://oa.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://mx.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://ei.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kq.jianghongdianzi.cn

[A03] 常量定义
来源：http://de.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://iu.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://im.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://cw.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://ye.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://gx.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://wn.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://gt.shxzskj.cn

[A04] 判断变量类型
来源：http://mz.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qq.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ez.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fl.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://rn.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dh.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rw.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://um.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://pc.chemitech.net.cn

[A05] 整数除法与取模
来源：http://uj.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ww.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cj.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kw.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qo.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://lw.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://ay.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://qo.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://hl.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://dh.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://yf.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cx.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pf.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wn.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ei.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yw.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ib.shtwfgs.cn

[A07] 数字转字符串
来源：http://we.panjiajie.cn

Py:   str(42)
来源：http://eu.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://nf.9csxet.cn

JS:   String(42); (42).toString()
来源：http://ih.panjiajie.cn

TS:   String(42)
来源：http://oq.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xw.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://cl.huixiangedu.cn

Ruby: 42.to_s
来源：http://ro.haigaiapp.cn

C#:   42.ToString()
来源：http://ah.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://sy.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kd.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nx.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ut.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nv.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qd.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qh.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://et.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hv.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://vz.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dt.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fp.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hp.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mz.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zx.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nq.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vg.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ak.wgjwhj.cn

[A10] 生成随机数
来源：http://rz.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://li.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://sc.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uq.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://to.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://nv.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ft.huanxung.cn

Ruby: rand(1..100)
来源：http://to.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://ky.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://ot.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://uc.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cd.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ye.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rm.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://rw.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hi.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fs.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rh.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://xj.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cn.nicolike.cn


<!-- 参考信息 -->