代发 wailian999

[U75] PHP：依赖注入
来源：http://ug.huanxung.cn

composer require psr/container
来源：http://pk.shxzskj.cn

[U76] PHP：简单路由
来源：http://wc.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rz.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://mo.shtwfgs.cn

composer require twig/twig
来源：http://iy.chemitech.net.cn

[U78] PHP：单元测试
来源：http://he.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://gf.shtwfgs.cn

[U79] PHP：静态分析
来源：http://sb.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://rm.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://hz.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sj.huanxung.cn

[U81] JS：初始化项目
来源：http://xq.nicolike.cn

npm init -y;  npm i express
来源：http://qf.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://rb.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jx.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://qf.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://db.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://jz.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qm.szsharing.cn

[U85] JS：可选链
来源：http://ox.wgjwhj.cn

a?.b?.c
来源：http://dg.huixiangedu.cn

[U86] JS：空值合并
来源：http://zg.huixiangedu.cn

a ?? b
来源：http://oo.nicolike.cn

[U87] JS：解构默认值
来源：http://xs.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://ui.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://uq.hahajie.cn

{ ...a, ...b }
来源：http://ke.yuexingan06.cn

[U89] JS：数组去重
来源：http://oh.gzmigu.cn

[...new Set(arr)]
来源：http://ry.gzmigu.cn

[U90] JS：数字数组排序
来源：http://ez.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://ik.asd995.cn

[U91] JS：对象键值遍历
来源：http://zo.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rr.yuexingan06.cn

[U92] JS：深拷贝
来源：http://df.shxzskj.cn

structuredClone(obj)
来源：http://xm.haigaiapp.cn

[U93] JS：模板字符串
来源：http://ln.panjiajie.cn

`共 ${n} 条`
来源：http://ex.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://ea.shtwfgs.cn

const double = x => x * 2;
来源：http://oc.nicolike.cn

[U95] JS：Promise 包装
来源：http://sd.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://dt.521024.cn

[U96] JS：async/await 与异常
来源：http://sm.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zu.shtwfgs.cn

[U97] JS：并发请求
来源：http://ny.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ph.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://pm.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tx.hahajie.cn

[U99] JS：事件监听
来源：http://jl.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://at.newstarts.cn

[U100] JS：DOM 查询
来源：http://nq.hnjuh.cn

document.querySelector(".item")
来源：http://yv.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://vn.shxzskj.cn

el.classList.toggle("active")
来源：http://mc.huixiangedu.cn

[U102] JS：本地存储
来源：http://sr.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ux.shxzukj.cn

[U103] JS：定时器
来源：http://bw.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ro.huixiangedu.cn

[U104] JS：防抖
来源：http://qg.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rg.chemitech.net.cn

[U105] JS：节流
来源：http://pd.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xr.9csxet.cn

[U106] JS：日期格式化
来源：http://gg.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uc.nszjky.cn

[U107] JS：数字千分位
来源：http://eu.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aj.chemitech.net.cn

[U108] JS：随机整数
来源：http://nb.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xd.shtwfgs.cn

[U109] JS：数组分组
来源：http://rz.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://oc.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://jy.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://as.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://mf.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://yp.shtwfgs.cn

[U112] JS：字符串补位
来源：http://gc.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://ap.hnjuh.cn

[U113] JS：正则替换全部
来源：http://ee.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://xh.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://xd.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ym.panjiajie.cn

[U115] JS：生成 UUID
来源：http://fj.nicolike.cn

crypto.randomUUID()
来源：http://in.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://gs.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://ex.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://lh.asd995.cn

npm i -D vitest;  npx vitest
来源：http://uz.lnxyls.cn

[U118] JS：开发服务器
来源：http://hp.szxytkj.cn

npm i -D vite;  npx vite
来源：http://ea.nicolike.cn

[U119] JS：生产构建
来源：http://we.bjjhwx.cn

npx vite build
来源：http://rd.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://ay.colortex.cn

import.meta.env.VITE_API_URL
来源：http://zb.yuntaijiaju.cn

================================================================================
来源：http://wy.9csxet.cn

统计汇总
来源：http://qs.yuntaijiaju.cn

================================================================================
来源：http://ec.hnjuh.cn

按语言统计（条）：
来源：http://pe.newstarts.cn

Python ......... 252
来源：http://rb.521024.cn

PHP ............ 252
来源：http://vr.haigaiapp.cn

JavaScript ..... 252
来源：http://gr.szxytkj.cn

TypeScript ..... 212
来源：http://yp.colortex.cn

Java ........... 212
来源：http://fz.chemitech.net.cn

Go ............. 212
来源：http://nt.bookmarksfly.cn

Ruby ........... 212
来源：http://lh.bjjhwx.cn

C# ............. 212
来源：http://gk.huixinmuqiang.cn

C .............. 30
来源：http://vs.yuntaijiaju.cn

C++ ............ 30
来源：http://co.szsharing.cn

SQL ............ 90
来源：http://ro.szxytkj.cn

Bash ........... 80
来源：http://sd.nicolike.cn

Kotlin ......... 15
来源：http://eg.jctech888.com.cn

Swift .......... 15
来源：http://ow.huanxung.cn

Lua ............ 10
来源：http://ai.szxytkj.cn

Perl ........... 10
来源：http://se.yuexingan06.cn

Scala .......... 10
来源：http://sv.huixinmuqiang.cn

------------------------------------
来源：http://rd.yuexingan06.cn

合计 ........... 2106 条
来源：http://yy.hahajie.cn

按章节统计：
来源：http://ga.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rn.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ym.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rf.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aa.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mc.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tc.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iz.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sb.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vk.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yc.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ow.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qb.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://il.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iy.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ua.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tu.bookmarksfly.cn

Q SQL 专题                              90
来源：http://kj.jianghongdianzi.cn

R Bash 专题                             80
来源：http://rw.szsharing.cn

S C / C++ 专题                          60
来源：http://mu.9csxet.cn

T 其他语言补充                          60
来源：http://bi.521024.cn

U 高频实用片段                         120
来源：http://kz.yuexingan06.cn

------------------------------------
来源：http://aa.newstarts.cn

合计                                  2106 条
来源：http://kd.521024.cn

--------------------------------------------------------------------------------
来源：http://ab.hahajie.cn

使用提醒
来源：http://xf.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://pb.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pt.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bj.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pc.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rz.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://md.nicolike.cn

—— 文件结束 ——
来源：http://po.panjiajie.cn

================================================================================
来源：http://wm.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://er.huanxung.cn

Common Programming Examples Cheat Book
来源：http://fe.wgjwhj.cn

================================================================================
来源：http://am.hnjuh.cn

【收录内容】
来源：http://hq.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dg.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://af.muxihuayi.cn

SQL · Bash · C · C++
来源：http://sg.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rb.chemitech.net.cn

【使用说明】
来源：http://hv.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mi.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pu.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kb.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jq.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lg.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ol.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vm.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cd.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lq.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://da.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mb.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pt.521024.cn

【文件统计】
来源：http://iu.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mb.asd995.cn

--------------------------------------------------------------------------------
来源：http://kv.hahajie.cn

目  录
来源：http://iz.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://vy.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wy.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://al.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xu.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bb.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://op.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qu.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fv.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uf.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xy.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ys.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sb.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qr.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://on.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ud.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ui.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ji.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://un.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ah.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ph.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nu.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yb.szxytkj.cn

================================================================================
来源：http://bc.yuntaijiaju.cn

A. 基础语法与类型
来源：http://jk.521024.cn

================================================================================
来源：http://al.shxzskj.cn

[A01] Hello World
来源：http://dw.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://qp.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://kb.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://lx.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hh.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://br.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://hg.asd995.cn

Ruby: puts "Hello, World!"
来源：http://xn.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zu.huanxung.cn

[A02] 变量声明与赋值
来源：http://hr.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rr.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zz.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vd.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gc.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://zt.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://qt.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://ke.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ap.huixiangedu.cn

[A03] 常量定义
来源：http://qi.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qe.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://ym.nicolike.cn

JS:   const PI = 3.14159;
来源：http://nd.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://zk.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://bd.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://oa.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://nc.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://ym.huixiangedu.cn

[A04] 判断变量类型
来源：http://ip.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qg.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bn.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fi.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://it.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zd.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ad.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://di.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://dz.shxzskj.cn

[A05] 整数除法与取模
来源：http://rr.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eo.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://an.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ab.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xb.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://mr.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://jm.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://iv.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://zm.hnjuh.cn

[A06] 字符串转数字
来源：http://nq.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://wg.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ve.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ln.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ad.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fz.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ic.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rg.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sz.nicolike.cn

[A07] 数字转字符串
来源：http://iy.haigaiapp.cn

Py:   str(42)
来源：http://bp.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://rr.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://sb.asd995.cn

TS:   String(42)
来源：http://kp.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pe.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://kp.shxzukj.cn

Ruby: 42.to_s
来源：http://yu.lnxyls.cn

C#:   42.ToString()
来源：http://wp.9csxet.cn

[A08] 取整与四舍五入
来源：http://yo.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ys.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tp.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ol.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bo.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dy.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yx.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zk.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nv.521024.cn

[A09] 绝对值与最大最小值
来源：http://jh.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yy.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dg.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://im.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mm.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wu.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ek.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ef.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tl.shtwfgs.cn

[A10] 生成随机数
来源：http://ev.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://cz.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://fo.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zb.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ss.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://mt.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gq.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://nt.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://ke.hahajie.cn

[A11] 条件表达式（三元）
来源：http://kp.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://sg.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qx.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://se.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ic.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://zc.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vz.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ap.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fj.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://dm.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fv.hahajie.cn


<!-- 参考信息 -->