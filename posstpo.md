代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://og.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://kq.huanxung.cn

[U74] PHP：读取环境变量
来源：http://sc.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://zp.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://fs.haigaiapp.cn

composer require psr/container
来源：http://tw.newstarts.cn

[U76] PHP：简单路由
来源：http://kj.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pw.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://pp.shxzskj.cn

composer require twig/twig
来源：http://ms.gzmigu.cn

[U78] PHP：单元测试
来源：http://se.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://hq.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://rz.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://hh.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://vi.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ha.nszjky.cn

[U81] JS：初始化项目
来源：http://zi.szsharing.cn

npm init -y;  npm i express
来源：http://gt.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://kj.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kl.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://gp.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mo.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://is.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xn.jctech888.com.cn

[U85] JS：可选链
来源：http://sk.shtwfgs.cn

a?.b?.c
来源：http://ji.bjjhwx.cn

[U86] JS：空值合并
来源：http://xn.szxytkj.cn

a ?? b
来源：http://bb.lnxyls.cn

[U87] JS：解构默认值
来源：http://tl.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://tg.huanxung.cn

[U88] JS：对象展开合并
来源：http://zx.yuexingan06.cn

{ ...a, ...b }
来源：http://li.shxzskj.cn

[U89] JS：数组去重
来源：http://fz.colortex.cn

[...new Set(arr)]
来源：http://pr.colortex.cn

[U90] JS：数字数组排序
来源：http://pn.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://fe.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://bz.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ma.gzmigu.cn

[U92] JS：深拷贝
来源：http://tr.chemitech.net.cn

structuredClone(obj)
来源：http://ih.asd995.cn

[U93] JS：模板字符串
来源：http://qi.huixiangedu.cn

`共 ${n} 条`
来源：http://db.colortex.cn

[U94] JS：箭头函数
来源：http://sv.shxzskj.cn

const double = x => x * 2;
来源：http://nu.gzmigu.cn

[U95] JS：Promise 包装
来源：http://va.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://pm.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://jb.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nl.nicolike.cn

[U97] JS：并发请求
来源：http://jr.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pq.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://ej.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ye.gzmigu.cn

[U99] JS：事件监听
来源：http://xo.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://gq.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://uf.muxihuayi.cn

document.querySelector(".item")
来源：http://sy.wgjwhj.cn

[U101] JS：classList 操作
来源：http://eh.huixiangedu.cn

el.classList.toggle("active")
来源：http://hz.521024.cn

[U102] JS：本地存储
来源：http://zp.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.haigaiapp.cn

[U103] JS：定时器
来源：http://lq.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bn.jianghongdianzi.cn

[U104] JS：防抖
来源：http://zl.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nj.jctech888.com.cn

[U105] JS：节流
来源：http://mk.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://it.nicolike.cn

[U106] JS：日期格式化
来源：http://bl.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ls.shxzskj.cn

[U107] JS：数字千分位
来源：http://fg.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zb.szsharing.cn

[U108] JS：随机整数
来源：http://gk.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dm.szsharing.cn

[U109] JS：数组分组
来源：http://es.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://bm.muxihuayi.cn

[U110] JS：数组分块
来源：http://ua.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yb.lnxyls.cn

[U111] JS：对象转 Map
来源：http://np.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://yt.jctech888.com.cn

[U112] JS：字符串补位
来源：http://zs.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://tg.szsharing.cn

[U113] JS：正则替换全部
来源：http://to.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://ld.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://rm.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iz.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://fe.yuntaijiaju.cn

crypto.randomUUID()
来源：http://bn.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://sw.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://bc.hahajie.cn

[U117] JS：单元测试
来源：http://ww.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://ln.newstarts.cn

[U118] JS：开发服务器
来源：http://ax.newstarts.cn

npm i -D vite;  npx vite
来源：http://xu.muxihuayi.cn

[U119] JS：生产构建
来源：http://wn.muxihuayi.cn

npx vite build
来源：http://xp.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://qp.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://mg.gzmigu.cn

================================================================================
来源：http://zy.nicolike.cn

统计汇总
来源：http://rg.yuntaijiaju.cn

================================================================================
来源：http://sn.asd995.cn

按语言统计（条）：
来源：http://yq.chemitech.net.cn

Python ......... 252
来源：http://ju.shxzskj.cn

PHP ............ 252
来源：http://fu.bookmarksfly.cn

JavaScript ..... 252
来源：http://yw.bjjhwx.cn

TypeScript ..... 212
来源：http://xi.jianghongdianzi.cn

Java ........... 212
来源：http://dm.bookmarksfly.cn

Go ............. 212
来源：http://no.hnjuh.cn

Ruby ........... 212
来源：http://xc.szsharing.cn

C# ............. 212
来源：http://wd.9csxet.cn

C .............. 30
来源：http://tn.shxzukj.cn

C++ ............ 30
来源：http://te.yuexingan06.cn

SQL ............ 90
来源：http://aj.9csxet.cn

Bash ........... 80
来源：http://jr.lnxyls.cn

Kotlin ......... 15
来源：http://zk.shxzukj.cn

Swift .......... 15
来源：http://dw.shxzskj.cn

Lua ............ 10
来源：http://ac.shxzskj.cn

Perl ........... 10
来源：http://ky.shxzukj.cn

Scala .......... 10
来源：http://xd.huanxung.cn

------------------------------------
来源：http://ih.hnjuh.cn

合计 ........... 2106 条
来源：http://qp.hnjuh.cn

按章节统计：
来源：http://cy.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oh.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pr.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://do.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xi.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jy.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nl.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jn.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kz.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://di.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nx.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://do.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fy.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xd.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pn.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oq.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yh.huixiangedu.cn

Q SQL 专题                              90
来源：http://yj.gzmigu.cn

R Bash 专题                             80
来源：http://wo.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://vs.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://fc.wgjwhj.cn

U 高频实用片段                         120
来源：http://tu.bookmarksfly.cn

------------------------------------
来源：http://ym.szsharing.cn

合计                                  2106 条
来源：http://ad.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://hj.asd995.cn

使用提醒
来源：http://pk.asd995.cn

--------------------------------------------------------------------------------
来源：http://xw.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sd.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zs.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lz.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kv.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sb.shxzskj.cn

—— 文件结束 ——
来源：http://jz.muxihuayi.cn

================================================================================
来源：http://pn.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://it.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://ob.yuexingan06.cn

================================================================================
来源：http://px.huixiangedu.cn

【收录内容】
来源：http://pl.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uh.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tu.lnxyls.cn

SQL · Bash · C · C++
来源：http://qy.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rj.yuntaijiaju.cn

【使用说明】
来源：http://ol.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rm.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ux.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uf.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fl.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://po.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pc.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oj.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oh.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wc.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pw.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wu.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bs.haigaiapp.cn

【文件统计】
来源：http://sp.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fv.521024.cn

--------------------------------------------------------------------------------
来源：http://fd.szxytkj.cn

目  录
来源：http://zx.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://tf.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gq.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qc.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sk.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://om.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sn.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uu.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gw.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nx.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wm.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dw.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pi.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jo.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jq.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yg.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ct.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tx.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sh.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ax.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wc.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cl.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nv.muxihuayi.cn

================================================================================
来源：http://mw.hnjuh.cn

A. 基础语法与类型
来源：http://yu.nszjky.cn

================================================================================
来源：http://us.gzmigu.cn

[A01] Hello World
来源：http://ti.lnxyls.cn

Py:   print("Hello, World!")
来源：http://jo.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://af.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://tc.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pf.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://jt.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://dm.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://bt.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qa.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://dx.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vk.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://si.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gq.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sp.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://gi.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://ga.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://gm.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ap.panjiajie.cn

[A03] 常量定义
来源：http://gw.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://an.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://jf.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://zc.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://ha.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://ds.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://vi.hnjuh.cn

Ruby: PI = 3.14159
来源：http://kh.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://up.hahajie.cn

[A04] 判断变量类型
来源：http://qt.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ae.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rq.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tg.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://dc.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jp.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gf.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ds.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://wv.shxzskj.cn

[A05] 整数除法与取模
来源：http://dz.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wt.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mw.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ol.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qu.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://kl.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://tu.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://ii.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://ht.muxihuayi.cn

[A06] 字符串转数字
来源：http://gf.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://pm.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vb.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ru.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ey.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ze.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://py.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wd.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xk.szsharing.cn

[A07] 数字转字符串
来源：http://br.szxytkj.cn

Py:   str(42)
来源：http://xt.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://fk.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://iy.bjjhwx.cn

TS:   String(42)
来源：http://ry.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://iz.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://dp.szxytkj.cn

Ruby: 42.to_s
来源：http://yw.lnxyls.cn

C#:   42.ToString()
来源：http://ds.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://vp.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xm.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rt.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tu.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rf.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hg.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xl.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jn.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rg.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://dz.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gt.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://af.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gf.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cf.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jt.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wh.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kr.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iy.newstarts.cn

[A10] 生成随机数
来源：http://jb.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://cc.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://ev.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sr.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xs.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://gu.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://go.colortex.cn

Ruby: rand(1..100)
来源：http://hi.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://lr.nicolike.cn

[A11] 条件表达式（三元）
来源：http://fu.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://xf.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xf.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yy.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iq.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://nc.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://im.szxytkj.cn


<!-- 参考信息 -->