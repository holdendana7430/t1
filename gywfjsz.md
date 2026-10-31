代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://cp.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://vj.huanxung.cn

[U74] PHP：读取环境变量
来源：http://rf.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://ua.panjiajie.cn

[U75] PHP：依赖注入
来源：http://oi.muxihuayi.cn

composer require psr/container
来源：http://cf.szsharing.cn

[U76] PHP：简单路由
来源：http://im.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zw.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://jl.szsharing.cn

composer require twig/twig
来源：http://kg.hahajie.cn

[U78] PHP：单元测试
来源：http://mw.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://ju.szxytkj.cn

[U79] PHP：静态分析
来源：http://yv.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://hl.nszjky.cn

[U80] PHP：代码规范修复
来源：http://rt.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ac.panjiajie.cn

[U81] JS：初始化项目
来源：http://eo.szxytkj.cn

npm init -y;  npm i express
来源：http://xa.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://qb.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qy.521024.cn

[U83] JS：ES Module 导入导出
来源：http://xk.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://is.521024.cn

[U84] JS：CommonJS 写法
来源：http://ey.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ms.szsharing.cn

[U85] JS：可选链
来源：http://lr.shtwfgs.cn

a?.b?.c
来源：http://we.shtwfgs.cn

[U86] JS：空值合并
来源：http://mr.huanxung.cn

a ?? b
来源：http://zv.gzmigu.cn

[U87] JS：解构默认值
来源：http://lb.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://qh.lnxyls.cn

[U88] JS：对象展开合并
来源：http://zc.yuexingan06.cn

{ ...a, ...b }
来源：http://br.521024.cn

[U89] JS：数组去重
来源：http://at.chemitech.net.cn

[...new Set(arr)]
来源：http://tm.shxzskj.cn

[U90] JS：数字数组排序
来源：http://yt.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://et.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://tk.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qj.lnxyls.cn

[U92] JS：深拷贝
来源：http://dl.9csxet.cn

structuredClone(obj)
来源：http://dd.chemitech.net.cn

[U93] JS：模板字符串
来源：http://za.shxzukj.cn

`共 ${n} 条`
来源：http://jj.haigaiapp.cn

[U94] JS：箭头函数
来源：http://ew.panjiajie.cn

const double = x => x * 2;
来源：http://le.shxzskj.cn

[U95] JS：Promise 包装
来源：http://zm.521024.cn

new Promise((resolve, reject) => {})
来源：http://ls.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://jl.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nq.9csxet.cn

[U97] JS：并发请求
来源：http://ow.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cj.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://ia.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ct.haigaiapp.cn

[U99] JS：事件监听
来源：http://me.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://bf.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://us.jctech888.com.cn

document.querySelector(".item")
来源：http://tf.9csxet.cn

[U101] JS：classList 操作
来源：http://zj.colortex.cn

el.classList.toggle("active")
来源：http://eo.newstarts.cn

[U102] JS：本地存储
来源：http://jp.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jx.jianghongdianzi.cn

[U103] JS：定时器
来源：http://fv.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://to.bjjhwx.cn

[U104] JS：防抖
来源：http://zo.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yd.huixinmuqiang.cn

[U105] JS：节流
来源：http://sc.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qx.521024.cn

[U106] JS：日期格式化
来源：http://zo.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://md.asd995.cn

[U107] JS：数字千分位
来源：http://yb.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dh.yuexingan06.cn

[U108] JS：随机整数
来源：http://oq.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vo.haigaiapp.cn

[U109] JS：数组分组
来源：http://oc.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://iw.panjiajie.cn

[U110] JS：数组分块
来源：http://so.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vh.nszjky.cn

[U111] JS：对象转 Map
来源：http://rq.hnjuh.cn

new Map(Object.entries(obj))
来源：http://yg.jctech888.com.cn

[U112] JS：字符串补位
来源：http://fi.panjiajie.cn

"7".padStart(3, "0")
来源：http://ur.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://mb.lnxyls.cn

s.replaceAll("a", "b")
来源：http://bx.hahajie.cn

[U114] JS：JSON 深比较
来源：http://qv.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ms.521024.cn

[U115] JS：生成 UUID
来源：http://hk.szsharing.cn

crypto.randomUUID()
来源：http://br.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://rh.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://nl.nszjky.cn

[U117] JS：单元测试
来源：http://ei.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://zg.szxytkj.cn

[U118] JS：开发服务器
来源：http://qw.hahajie.cn

npm i -D vite;  npx vite
来源：http://zk.hahajie.cn

[U119] JS：生产构建
来源：http://vl.szsharing.cn

npx vite build
来源：http://hv.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://jj.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://pd.jctech888.com.cn

================================================================================
来源：http://mb.shtwfgs.cn

统计汇总
来源：http://by.hahajie.cn

================================================================================
来源：http://xj.jctech888.com.cn

按语言统计（条）：
来源：http://qx.shxzskj.cn

Python ......... 252
来源：http://rj.jctech888.com.cn

PHP ............ 252
来源：http://yg.szsharing.cn

JavaScript ..... 252
来源：http://fj.lnxyls.cn

TypeScript ..... 212
来源：http://ir.521024.cn

Java ........... 212
来源：http://rb.yuexingan06.cn

Go ............. 212
来源：http://gn.nszjky.cn

Ruby ........... 212
来源：http://gf.haigaiapp.cn

C# ............. 212
来源：http://ij.jianghongdianzi.cn

C .............. 30
来源：http://xb.haigaiapp.cn

C++ ............ 30
来源：http://qn.nicolike.cn

SQL ............ 90
来源：http://pc.szsharing.cn

Bash ........... 80
来源：http://pj.yuntaijiaju.cn

Kotlin ......... 15
来源：http://ar.szxytkj.cn

Swift .......... 15
来源：http://sk.bookmarksfly.cn

Lua ............ 10
来源：http://ei.huixiangedu.cn

Perl ........... 10
来源：http://fa.hnjuh.cn

Scala .......... 10
来源：http://by.jctech888.com.cn

------------------------------------
来源：http://qr.hnjuh.cn

合计 ........... 2106 条
来源：http://ii.bookmarksfly.cn

按章节统计：
来源：http://xn.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mr.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ep.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lk.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ya.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fv.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sy.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ir.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://we.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vx.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sf.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ns.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vz.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ih.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xm.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xm.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nq.huixiangedu.cn

Q SQL 专题                              90
来源：http://pb.panjiajie.cn

R Bash 专题                             80
来源：http://hj.521024.cn

S C / C++ 专题                          60
来源：http://je.lnxyls.cn

T 其他语言补充                          60
来源：http://qs.yuexingan06.cn

U 高频实用片段                         120
来源：http://en.asd995.cn

------------------------------------
来源：http://ew.hahajie.cn

合计                                  2106 条
来源：http://of.nszjky.cn

--------------------------------------------------------------------------------
来源：http://we.asd995.cn

使用提醒
来源：http://ph.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://up.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tr.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xw.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gp.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://en.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xv.yuexingan06.cn

—— 文件结束 ——
来源：http://hn.chemitech.net.cn

================================================================================
来源：http://wb.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://mi.hahajie.cn

Common Programming Examples Cheat Book
来源：http://ah.yuexingan06.cn

================================================================================
来源：http://xh.newstarts.cn

【收录内容】
来源：http://gx.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qv.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rz.shtwfgs.cn

SQL · Bash · C · C++
来源：http://hi.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hv.huixinmuqiang.cn

【使用说明】
来源：http://fk.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fp.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uk.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kb.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fd.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bp.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xy.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rq.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://un.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ht.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fs.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ob.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qn.gzmigu.cn

【文件统计】
来源：http://bx.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://of.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ts.jianghongdianzi.cn

目  录
来源：http://vy.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://cl.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kx.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jd.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://io.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jp.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://he.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jy.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fn.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://td.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iu.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lh.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ad.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ju.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cg.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vd.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hc.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://od.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iy.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://br.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mo.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uk.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nq.huanxung.cn

================================================================================
来源：http://pj.bookmarksfly.cn

A. 基础语法与类型
来源：http://il.panjiajie.cn

================================================================================
来源：http://kg.panjiajie.cn

[A01] Hello World
来源：http://ff.szxytkj.cn

Py:   print("Hello, World!")
来源：http://lj.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://uw.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://ft.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ye.521024.cn

Java: System.out.println("Hello, World!");
来源：http://nl.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://aq.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://ln.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pg.9csxet.cn

[A02] 变量声明与赋值
来源：http://ra.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pi.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tc.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lm.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://op.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://ly.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://cr.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://dd.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ij.lnxyls.cn

[A03] 常量定义
来源：http://ih.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ml.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://ta.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://hd.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://cz.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://av.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://ao.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://zz.colortex.cn

C#:   const double PI = 3.14159;
来源：http://hj.gzmigu.cn

[A04] 判断变量类型
来源：http://za.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ys.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ea.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fk.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://kq.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yw.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nr.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bp.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://mf.chemitech.net.cn

[A05] 整数除法与取模
来源：http://wv.nszjky.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hw.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zy.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sy.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oo.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://wp.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://sd.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://cp.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://mn.hahajie.cn

[A06] 字符串转数字
来源：http://rp.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://td.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ue.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rp.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://df.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lx.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yv.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://di.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vz.nszjky.cn

[A07] 数字转字符串
来源：http://jz.wgjwhj.cn

Py:   str(42)
来源：http://vh.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://vp.newstarts.cn

JS:   String(42); (42).toString()
来源：http://pq.yuexingan06.cn

TS:   String(42)
来源：http://uo.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://al.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://jo.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://gq.lnxyls.cn

C#:   42.ToString()
来源：http://qg.asd995.cn

[A08] 取整与四舍五入
来源：http://bx.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qc.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mn.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://td.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nw.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ki.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xv.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tx.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ks.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://yl.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pi.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://si.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://si.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zz.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nj.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ku.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xo.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ge.colortex.cn

[A10] 生成随机数
来源：http://lp.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://na.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://le.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pl.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nx.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://je.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uq.hahajie.cn

Ruby: rand(1..100)
来源：http://kg.521024.cn

C#:   new Random().Next(1, 101)
来源：http://bh.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://hg.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://xn.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vd.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rv.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ol.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://zy.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nb.haigaiapp.cn


<!-- 参考信息 -->