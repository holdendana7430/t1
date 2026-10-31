代发 wailian999

[U71] PHP：抛出异常
来源：http://ds.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://ni.shxzskj.cn

[U72] PHP：写错误日志
来源：http://wf.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://rg.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://hd.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://ll.szsharing.cn

[U74] PHP：读取环境变量
来源：http://ky.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://lc.newstarts.cn

[U75] PHP：依赖注入
来源：http://fv.huanxung.cn

composer require psr/container
来源：http://xc.lnxyls.cn

[U76] PHP：简单路由
来源：http://ri.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ej.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://oj.szxytkj.cn

composer require twig/twig
来源：http://mm.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://oc.asd995.cn

composer require --dev phpunit/phpunit
来源：http://mt.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://tk.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://pv.9csxet.cn

[U80] PHP：代码规范修复
来源：http://ap.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hk.lnxyls.cn

[U81] JS：初始化项目
来源：http://io.bookmarksfly.cn

npm init -y;  npm i express
来源：http://nv.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://vp.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rs.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://uh.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mh.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://lb.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qv.haigaiapp.cn

[U85] JS：可选链
来源：http://ko.lnxyls.cn

a?.b?.c
来源：http://bb.shxzukj.cn

[U86] JS：空值合并
来源：http://eq.bookmarksfly.cn

a ?? b
来源：http://ko.nicolike.cn

[U87] JS：解构默认值
来源：http://bv.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://lq.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://zi.huixiangedu.cn

{ ...a, ...b }
来源：http://wu.9csxet.cn

[U89] JS：数组去重
来源：http://ct.bookmarksfly.cn

[...new Set(arr)]
来源：http://pv.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://fu.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://bm.newstarts.cn

[U91] JS：对象键值遍历
来源：http://cj.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://es.jctech888.com.cn

[U92] JS：深拷贝
来源：http://fl.huanxung.cn

structuredClone(obj)
来源：http://fj.shxzukj.cn

[U93] JS：模板字符串
来源：http://ge.jctech888.com.cn

`共 ${n} 条`
来源：http://vs.asd995.cn

[U94] JS：箭头函数
来源：http://to.szxytkj.cn

const double = x => x * 2;
来源：http://gm.newstarts.cn

[U95] JS：Promise 包装
来源：http://hn.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://nk.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://da.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vi.shxzskj.cn

[U97] JS：并发请求
来源：http://ex.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ly.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://yj.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tz.shxzukj.cn

[U99] JS：事件监听
来源：http://ch.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://dl.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://am.nicolike.cn

document.querySelector(".item")
来源：http://fg.hahajie.cn

[U101] JS：classList 操作
来源：http://al.bjjhwx.cn

el.classList.toggle("active")
来源：http://ew.chemitech.net.cn

[U102] JS：本地存储
来源：http://fc.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mq.panjiajie.cn

[U103] JS：定时器
来源：http://vt.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://th.chemitech.net.cn

[U104] JS：防抖
来源：http://np.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jg.wgjwhj.cn

[U105] JS：节流
来源：http://eu.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cx.newstarts.cn

[U106] JS：日期格式化
来源：http://wl.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wg.colortex.cn

[U107] JS：数字千分位
来源：http://sg.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vq.nicolike.cn

[U108] JS：随机整数
来源：http://oq.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eb.bjjhwx.cn

[U109] JS：数组分组
来源：http://qa.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://iv.bjjhwx.cn

[U110] JS：数组分块
来源：http://ai.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jh.hnjuh.cn

[U111] JS：对象转 Map
来源：http://wl.nicolike.cn

new Map(Object.entries(obj))
来源：http://gi.9csxet.cn

[U112] JS：字符串补位
来源：http://nh.nicolike.cn

"7".padStart(3, "0")
来源：http://uh.shxzukj.cn

[U113] JS：正则替换全部
来源：http://lh.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://es.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://bn.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bb.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://fs.szsharing.cn

crypto.randomUUID()
来源：http://li.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://pa.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://xz.haigaiapp.cn

[U117] JS：单元测试
来源：http://ld.asd995.cn

npm i -D vitest;  npx vitest
来源：http://ny.hnjuh.cn

[U118] JS：开发服务器
来源：http://ko.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://zo.nszjky.cn

[U119] JS：生产构建
来源：http://fl.nszjky.cn

npx vite build
来源：http://xz.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://mj.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://gt.szsharing.cn

================================================================================
来源：http://sx.jianghongdianzi.cn

统计汇总
来源：http://ky.muxihuayi.cn

================================================================================
来源：http://oc.yuexingan06.cn

按语言统计（条）：
来源：http://fn.colortex.cn

Python ......... 252
来源：http://jr.huixinmuqiang.cn

PHP ............ 252
来源：http://qo.szxytkj.cn

JavaScript ..... 252
来源：http://cl.huanxung.cn

TypeScript ..... 212
来源：http://gr.haigaiapp.cn

Java ........... 212
来源：http://tf.shxzukj.cn

Go ............. 212
来源：http://hk.nicolike.cn

Ruby ........... 212
来源：http://dz.jctech888.com.cn

C# ............. 212
来源：http://xk.haigaiapp.cn

C .............. 30
来源：http://tx.wgjwhj.cn

C++ ............ 30
来源：http://it.haigaiapp.cn

SQL ............ 90
来源：http://hg.huixiangedu.cn

Bash ........... 80
来源：http://dw.lnxyls.cn

Kotlin ......... 15
来源：http://wf.bookmarksfly.cn

Swift .......... 15
来源：http://dk.szxytkj.cn

Lua ............ 10
来源：http://pt.wgjwhj.cn

Perl ........... 10
来源：http://lg.szsharing.cn

Scala .......... 10
来源：http://xf.szxytkj.cn

------------------------------------
来源：http://xx.shtwfgs.cn

合计 ........... 2106 条
来源：http://jm.wgjwhj.cn

按章节统计：
来源：http://kc.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tf.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pu.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://no.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nc.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://es.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cg.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qw.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wc.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ax.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ye.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jq.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rs.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jd.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bj.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qr.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://go.szsharing.cn

Q SQL 专题                              90
来源：http://cj.colortex.cn

R Bash 专题                             80
来源：http://ca.hnjuh.cn

S C / C++ 专题                          60
来源：http://ol.huanxung.cn

T 其他语言补充                          60
来源：http://jc.gzmigu.cn

U 高频实用片段                         120
来源：http://ps.shxzskj.cn

------------------------------------
来源：http://lt.bjjhwx.cn

合计                                  2106 条
来源：http://fo.9csxet.cn

--------------------------------------------------------------------------------
来源：http://iq.shxzskj.cn

使用提醒
来源：http://an.9csxet.cn

--------------------------------------------------------------------------------
来源：http://qv.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lj.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zg.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qi.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fo.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ro.szxytkj.cn

—— 文件结束 ——
来源：http://gf.hnjuh.cn

================================================================================
来源：http://tq.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://ar.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://ey.jianghongdianzi.cn

================================================================================
来源：http://hy.muxihuayi.cn

【收录内容】
来源：http://be.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://op.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ke.shtwfgs.cn

SQL · Bash · C · C++
来源：http://gx.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mq.nszjky.cn

【使用说明】
来源：http://km.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yv.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jt.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bl.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ad.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xl.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ge.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dm.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jg.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lb.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://in.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bj.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wz.szxytkj.cn

【文件统计】
来源：http://nj.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mz.521024.cn

--------------------------------------------------------------------------------
来源：http://mt.haigaiapp.cn

目  录
来源：http://mw.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://xq.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bv.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yx.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tw.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qj.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://re.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dr.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wg.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://om.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ms.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://av.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lg.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yq.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qo.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vj.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mw.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tj.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hp.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lm.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fy.yuexingan06.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zv.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jf.haigaiapp.cn

================================================================================
来源：http://th.yuntaijiaju.cn

A. 基础语法与类型
来源：http://pg.newstarts.cn

================================================================================
来源：http://hr.hahajie.cn

[A01] Hello World
来源：http://sj.panjiajie.cn

Py:   print("Hello, World!")
来源：http://ie.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://op.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://iw.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://om.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://jo.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://kl.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://bi.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cv.szsharing.cn

[A02] 变量声明与赋值
来源：http://pj.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://za.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xw.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ak.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sv.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://ob.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://dz.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://ng.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ir.szsharing.cn

[A03] 常量定义
来源：http://vs.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xk.colortex.cn

PHP:  const PI = 3.14159;
来源：http://lq.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://xm.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://ri.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://cd.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://gv.newstarts.cn

Ruby: PI = 3.14159
来源：http://gw.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://am.jctech888.com.cn

[A04] 判断变量类型
来源：http://rd.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dy.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xh.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ty.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://ah.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qw.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ha.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://px.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://eg.muxihuayi.cn

[A05] 整数除法与取模
来源：http://rr.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vm.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ll.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pg.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pw.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://li.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://jx.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://lh.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://so.huixiangedu.cn

[A06] 字符串转数字
来源：http://kz.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://uz.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://me.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rq.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ef.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ux.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tz.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://st.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qw.chemitech.net.cn

[A07] 数字转字符串
来源：http://ez.bookmarksfly.cn

Py:   str(42)
来源：http://xh.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://gs.hahajie.cn

JS:   String(42); (42).toString()
来源：http://kt.lnxyls.cn

TS:   String(42)
来源：http://bc.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ux.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://qr.shxzskj.cn

Ruby: 42.to_s
来源：http://ov.muxihuayi.cn

C#:   42.ToString()
来源：http://gh.asd995.cn

[A08] 取整与四舍五入
来源：http://jj.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://au.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ad.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rn.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hx.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yv.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yo.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lc.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fb.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://cq.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vd.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ng.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fo.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://aq.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nh.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qg.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qq.asd995.cn

[A10] 生成随机数
来源：http://vf.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://mp.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://cq.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ov.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hw.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://qp.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dq.nicolike.cn

Ruby: rand(1..100)
来源：http://ia.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://lp.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://qn.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://yt.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dx.colortex.cn


<!-- 参考信息 -->