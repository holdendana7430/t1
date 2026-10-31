代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://bb.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://kk.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://yu.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://lc.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://lu.bjjhwx.cn

composer require psr/container
来源：http://ie.lnxyls.cn

[U76] PHP：简单路由
来源：http://ln.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nu.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://pz.hahajie.cn

composer require twig/twig
来源：http://jm.hahajie.cn

[U78] PHP：单元测试
来源：http://oz.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://os.huanxung.cn

[U79] PHP：静态分析
来源：http://vu.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://sn.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://kx.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vw.9csxet.cn

[U81] JS：初始化项目
来源：http://ey.shxzukj.cn

npm init -y;  npm i express
来源：http://jq.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://hn.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wn.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://lg.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gi.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://gr.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fs.szsharing.cn

[U85] JS：可选链
来源：http://ga.bookmarksfly.cn

a?.b?.c
来源：http://uh.newstarts.cn

[U86] JS：空值合并
来源：http://zm.shtwfgs.cn

a ?? b
来源：http://od.chemitech.net.cn

[U87] JS：解构默认值
来源：http://kc.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://xr.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://bx.newstarts.cn

{ ...a, ...b }
来源：http://ne.asd995.cn

[U89] JS：数组去重
来源：http://ux.yuntaijiaju.cn

[...new Set(arr)]
来源：http://zf.9csxet.cn

[U90] JS：数字数组排序
来源：http://ll.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://rk.nszjky.cn

[U91] JS：对象键值遍历
来源：http://nn.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://go.jctech888.com.cn

[U92] JS：深拷贝
来源：http://ln.gzmigu.cn

structuredClone(obj)
来源：http://ff.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://fx.hahajie.cn

`共 ${n} 条`
来源：http://wq.muxihuayi.cn

[U94] JS：箭头函数
来源：http://es.colortex.cn

const double = x => x * 2;
来源：http://lo.521024.cn

[U95] JS：Promise 包装
来源：http://sz.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://qt.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://yi.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fi.wgjwhj.cn

[U97] JS：并发请求
来源：http://ah.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ne.521024.cn

[U98] JS：fetch 带 JSON
来源：http://pe.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ww.bookmarksfly.cn

[U99] JS：事件监听
来源：http://cp.nszjky.cn

el.addEventListener("click", e => {})
来源：http://jh.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://pr.shxzskj.cn

document.querySelector(".item")
来源：http://bl.shxzukj.cn

[U101] JS：classList 操作
来源：http://ea.asd995.cn

el.classList.toggle("active")
来源：http://oy.panjiajie.cn

[U102] JS：本地存储
来源：http://qs.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bc.hnjuh.cn

[U103] JS：定时器
来源：http://vk.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uf.huanxung.cn

[U104] JS：防抖
来源：http://bd.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dv.lnxyls.cn

[U105] JS：节流
来源：http://yo.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://el.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://pv.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dk.szxytkj.cn

[U107] JS：数字千分位
来源：http://pw.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pt.colortex.cn

[U108] JS：随机整数
来源：http://rs.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dn.haigaiapp.cn

[U109] JS：数组分组
来源：http://fe.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://ge.newstarts.cn

[U110] JS：数组分块
来源：http://nr.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kd.gzmigu.cn

[U111] JS：对象转 Map
来源：http://fw.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://pb.hnjuh.cn

[U112] JS：字符串补位
来源：http://ji.asd995.cn

"7".padStart(3, "0")
来源：http://im.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://qf.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://kq.521024.cn

[U114] JS：JSON 深比较
来源：http://gx.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://da.szsharing.cn

[U115] JS：生成 UUID
来源：http://bn.huixinmuqiang.cn

crypto.randomUUID()
来源：http://us.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://sw.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://zo.muxihuayi.cn

[U117] JS：单元测试
来源：http://an.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://ez.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://pj.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://ri.panjiajie.cn

[U119] JS：生产构建
来源：http://uh.nicolike.cn

npx vite build
来源：http://zs.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://hl.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://wc.hahajie.cn

================================================================================
来源：http://vc.gzmigu.cn

统计汇总
来源：http://be.nicolike.cn

================================================================================
来源：http://ld.asd995.cn

按语言统计（条）：
来源：http://tf.haigaiapp.cn

Python ......... 252
来源：http://gi.gzmigu.cn

PHP ............ 252
来源：http://qp.bookmarksfly.cn

JavaScript ..... 252
来源：http://li.yuntaijiaju.cn

TypeScript ..... 212
来源：http://oi.szxytkj.cn

Java ........... 212
来源：http://fn.haigaiapp.cn

Go ............. 212
来源：http://fh.shxzukj.cn

Ruby ........... 212
来源：http://xe.shxzukj.cn

C# ............. 212
来源：http://cn.huixinmuqiang.cn

C .............. 30
来源：http://bs.jianghongdianzi.cn

C++ ............ 30
来源：http://yt.chemitech.net.cn

SQL ............ 90
来源：http://ib.muxihuayi.cn

Bash ........... 80
来源：http://ga.nicolike.cn

Kotlin ......... 15
来源：http://cl.shxzskj.cn

Swift .......... 15
来源：http://qx.shxzskj.cn

Lua ............ 10
来源：http://je.yuexingan06.cn

Perl ........... 10
来源：http://mj.yuexingan06.cn

Scala .......... 10
来源：http://qa.muxihuayi.cn

------------------------------------
来源：http://gu.nszjky.cn

合计 ........... 2106 条
来源：http://nh.521024.cn

按章节统计：
来源：http://yn.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hw.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qw.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lw.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://du.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cb.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ht.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ki.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hf.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qs.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ad.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vc.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zi.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ib.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iv.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zh.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dq.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://rz.yuexingan06.cn

R Bash 专题                             80
来源：http://eh.colortex.cn

S C / C++ 专题                          60
来源：http://kb.521024.cn

T 其他语言补充                          60
来源：http://ds.521024.cn

U 高频实用片段                         120
来源：http://wl.shxzukj.cn

------------------------------------
来源：http://ap.haigaiapp.cn

合计                                  2106 条
来源：http://wb.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://xv.hahajie.cn

使用提醒
来源：http://ke.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://jv.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ts.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cy.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hy.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ce.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dd.colortex.cn

—— 文件结束 ——
来源：http://gp.panjiajie.cn

================================================================================
来源：http://in.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://mw.nszjky.cn

Common Programming Examples Cheat Book
来源：http://ta.szxytkj.cn

================================================================================
来源：http://jr.colortex.cn

【收录内容】
来源：http://tw.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://om.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wo.nicolike.cn

SQL · Bash · C · C++
来源：http://ix.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yv.haigaiapp.cn

【使用说明】
来源：http://zz.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vo.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dk.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ii.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ii.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pc.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ts.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ap.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fv.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ns.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ti.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kr.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://td.chemitech.net.cn

【文件统计】
来源：http://oz.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nx.521024.cn

--------------------------------------------------------------------------------
来源：http://wh.chemitech.net.cn

目  录
来源：http://hv.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://un.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vo.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wi.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rz.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fq.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bl.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iy.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zj.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eu.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rn.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ao.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ft.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sj.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jc.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wk.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pp.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jm.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pv.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yl.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qf.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uh.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eo.shxzukj.cn

================================================================================
来源：http://ae.chemitech.net.cn

A. 基础语法与类型
来源：http://vj.huixiangedu.cn

================================================================================
来源：http://ad.hahajie.cn

[A01] Hello World
来源：http://il.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ox.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://qb.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://ib.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qo.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://nk.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://le.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://ux.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cw.shxzskj.cn

[A02] 变量声明与赋值
来源：http://mp.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qh.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rv.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ro.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gx.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://zx.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://xv.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://tp.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fa.9csxet.cn

[A03] 常量定义
来源：http://zw.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gq.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://uj.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://rw.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://ya.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://zk.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://di.colortex.cn

Ruby: PI = 3.14159
来源：http://ko.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://gr.shtwfgs.cn

[A04] 判断变量类型
来源：http://dt.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://we.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fs.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zu.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://fv.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bo.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://br.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ug.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://mm.nicolike.cn

[A05] 整数除法与取模
来源：http://ro.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wj.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dr.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vg.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yz.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://ob.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://pw.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://nd.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://xm.newstarts.cn

[A06] 字符串转数字
来源：http://zg.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://fo.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nl.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ck.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://el.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ni.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tc.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://na.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ud.bookmarksfly.cn

[A07] 数字转字符串
来源：http://da.lnxyls.cn

Py:   str(42)
来源：http://bd.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://uf.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://gb.shtwfgs.cn

TS:   String(42)
来源：http://te.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mu.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://qo.wgjwhj.cn

Ruby: 42.to_s
来源：http://gx.shxzukj.cn

C#:   42.ToString()
来源：http://kw.hnjuh.cn

[A08] 取整与四舍五入
来源：http://gn.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zn.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bc.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rk.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ui.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ah.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ho.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nt.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://el.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://gd.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bu.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gr.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rk.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mn.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gi.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dw.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qv.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zg.shtwfgs.cn

[A10] 生成随机数
来源：http://dw.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://yc.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://co.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cp.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://do.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ua.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mi.lnxyls.cn

Ruby: rand(1..100)
来源：http://om.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://xz.szsharing.cn

[A11] 条件表达式（三元）
来源：http://es.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://mt.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pz.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wp.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://np.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://fq.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://od.muxihuayi.cn


<!-- 参考信息 -->