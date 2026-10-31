代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://sn.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://xc.asd995.cn

[U74] PHP：读取环境变量
来源：http://ze.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://jq.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://ht.jctech888.com.cn

composer require psr/container
来源：http://qs.muxihuayi.cn

[U76] PHP：简单路由
来源：http://ss.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qs.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://vi.bjjhwx.cn

composer require twig/twig
来源：http://gg.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://bs.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://sy.9csxet.cn

[U79] PHP：静态分析
来源：http://ws.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://lh.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://oq.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ao.newstarts.cn

[U81] JS：初始化项目
来源：http://pb.jctech888.com.cn

npm init -y;  npm i express
来源：http://gk.nszjky.cn

[U82] JS：package.json 脚本
来源：http://rl.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fi.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://al.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yz.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://qr.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zs.colortex.cn

[U85] JS：可选链
来源：http://lp.yuexingan06.cn

a?.b?.c
来源：http://dk.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://vj.panjiajie.cn

a ?? b
来源：http://xf.newstarts.cn

[U87] JS：解构默认值
来源：http://mi.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://hf.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://sq.nszjky.cn

{ ...a, ...b }
来源：http://uc.muxihuayi.cn

[U89] JS：数组去重
来源：http://xc.jctech888.com.cn

[...new Set(arr)]
来源：http://nf.shxzskj.cn

[U90] JS：数字数组排序
来源：http://ve.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://dn.nicolike.cn

[U91] JS：对象键值遍历
来源：http://lc.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pd.nszjky.cn

[U92] JS：深拷贝
来源：http://oz.gzmigu.cn

structuredClone(obj)
来源：http://wr.hnjuh.cn

[U93] JS：模板字符串
来源：http://zc.yuexingan06.cn

`共 ${n} 条`
来源：http://sl.nszjky.cn

[U94] JS：箭头函数
来源：http://kg.yuexingan06.cn

const double = x => x * 2;
来源：http://jo.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://se.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://sa.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://bb.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xk.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://xu.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bz.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://ox.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yk.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://np.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://ly.521024.cn

[U100] JS：DOM 查询
来源：http://hw.panjiajie.cn

document.querySelector(".item")
来源：http://ka.haigaiapp.cn

[U101] JS：classList 操作
来源：http://zg.nszjky.cn

el.classList.toggle("active")
来源：http://rq.wgjwhj.cn

[U102] JS：本地存储
来源：http://rl.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xf.szxytkj.cn

[U103] JS：定时器
来源：http://vj.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yv.chemitech.net.cn

[U104] JS：防抖
来源：http://ow.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pa.yuntaijiaju.cn

[U105] JS：节流
来源：http://mu.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wm.lnxyls.cn

[U106] JS：日期格式化
来源：http://sq.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pc.huanxung.cn

[U107] JS：数字千分位
来源：http://oi.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ys.shxzskj.cn

[U108] JS：随机整数
来源：http://dj.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pm.lnxyls.cn

[U109] JS：数组分组
来源：http://ec.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://lo.nszjky.cn

[U110] JS：数组分块
来源：http://xs.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jy.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://rd.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://hl.wgjwhj.cn

[U112] JS：字符串补位
来源：http://lf.9csxet.cn

"7".padStart(3, "0")
来源：http://ys.nicolike.cn

[U113] JS：正则替换全部
来源：http://lu.lnxyls.cn

s.replaceAll("a", "b")
来源：http://nw.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://fp.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://em.shxzskj.cn

[U115] JS：生成 UUID
来源：http://tj.bjjhwx.cn

crypto.randomUUID()
来源：http://ew.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://si.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://oa.gzmigu.cn

[U117] JS：单元测试
来源：http://pg.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://go.jctech888.com.cn

[U118] JS：开发服务器
来源：http://rj.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://ah.bjjhwx.cn

[U119] JS：生产构建
来源：http://vc.colortex.cn

npx vite build
来源：http://gv.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://vb.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://ia.yuntaijiaju.cn

================================================================================
来源：http://yo.bookmarksfly.cn

统计汇总
来源：http://ft.hnjuh.cn

================================================================================
来源：http://sr.colortex.cn

按语言统计（条）：
来源：http://ys.gzmigu.cn

Python ......... 252
来源：http://fe.shxzukj.cn

PHP ............ 252
来源：http://ct.panjiajie.cn

JavaScript ..... 252
来源：http://wp.panjiajie.cn

TypeScript ..... 212
来源：http://ca.huixiangedu.cn

Java ........... 212
来源：http://qh.newstarts.cn

Go ............. 212
来源：http://pp.jctech888.com.cn

Ruby ........... 212
来源：http://ys.521024.cn

C# ............. 212
来源：http://qf.521024.cn

C .............. 30
来源：http://om.colortex.cn

C++ ............ 30
来源：http://os.nicolike.cn

SQL ............ 90
来源：http://fg.nszjky.cn

Bash ........... 80
来源：http://sc.szsharing.cn

Kotlin ......... 15
来源：http://ug.haigaiapp.cn

Swift .......... 15
来源：http://zs.yuntaijiaju.cn

Lua ............ 10
来源：http://cu.newstarts.cn

Perl ........... 10
来源：http://gw.shxzukj.cn

Scala .......... 10
来源：http://bv.lnxyls.cn

------------------------------------
来源：http://tj.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://jo.9csxet.cn

按章节统计：
来源：http://mo.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yr.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ei.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ny.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cf.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tx.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ea.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nj.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zu.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dr.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kq.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sz.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jq.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jy.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://he.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ug.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ja.haigaiapp.cn

Q SQL 专题                              90
来源：http://ri.bookmarksfly.cn

R Bash 专题                             80
来源：http://zl.nicolike.cn

S C / C++ 专题                          60
来源：http://mn.bjjhwx.cn

T 其他语言补充                          60
来源：http://lw.bjjhwx.cn

U 高频实用片段                         120
来源：http://bs.yuntaijiaju.cn

------------------------------------
来源：http://td.bjjhwx.cn

合计                                  2106 条
来源：http://dk.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://id.yuexingan06.cn

使用提醒
来源：http://gd.521024.cn

--------------------------------------------------------------------------------
来源：http://wl.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yy.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fj.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yk.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wz.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://at.huanxung.cn

—— 文件结束 ——
来源：http://hz.yuntaijiaju.cn

================================================================================
来源：http://et.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://eg.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://rn.asd995.cn

================================================================================
来源：http://cl.nszjky.cn

【收录内容】
来源：http://df.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ek.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ki.muxihuayi.cn

SQL · Bash · C · C++
来源：http://fp.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nz.haigaiapp.cn

【使用说明】
来源：http://ja.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uj.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mz.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nh.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ui.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qi.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ek.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yh.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ro.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fh.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nz.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mf.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eo.521024.cn

【文件统计】
来源：http://aw.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vr.9csxet.cn

--------------------------------------------------------------------------------
来源：http://cm.wgjwhj.cn

目  录
来源：http://eb.nszjky.cn

--------------------------------------------------------------------------------
来源：http://ev.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yv.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sd.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qo.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ww.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://or.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://we.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wo.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fs.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nx.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pg.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gr.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vs.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bc.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mw.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://un.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ts.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sf.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ig.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qu.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ie.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rt.jianghongdianzi.cn

================================================================================
来源：http://hy.asd995.cn

A. 基础语法与类型
来源：http://ns.asd995.cn

================================================================================
来源：http://qe.hahajie.cn

[A01] Hello World
来源：http://uy.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://vt.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://qw.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://ql.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eg.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://fb.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://iy.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://vi.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ie.hnjuh.cn

[A02] 变量声明与赋值
来源：http://xe.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kw.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fx.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://th.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mo.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://dw.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://yp.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://jx.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tz.521024.cn

[A03] 常量定义
来源：http://rd.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ej.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://jd.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://lm.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://au.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://pq.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://qz.huanxung.cn

Ruby: PI = 3.14159
来源：http://wz.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://vj.wgjwhj.cn

[A04] 判断变量类型
来源：http://uf.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uu.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vd.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fs.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://zk.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://od.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://el.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ez.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://vq.asd995.cn

[A05] 整数除法与取模
来源：http://vh.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ik.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wh.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jt.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ri.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://nh.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://ln.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://qo.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://du.haigaiapp.cn

[A06] 字符串转数字
来源：http://dg.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://bl.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zg.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sy.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rt.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gy.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pc.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://il.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bi.hnjuh.cn

[A07] 数字转字符串
来源：http://qe.wgjwhj.cn

Py:   str(42)
来源：http://py.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://pe.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://jg.nszjky.cn

TS:   String(42)
来源：http://rp.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ps.asd995.cn

Go:   strconv.Itoa(42)
来源：http://sm.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://be.panjiajie.cn

C#:   42.ToString()
来源：http://ln.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://zw.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ec.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nz.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wd.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xz.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mx.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rk.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xa.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ol.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://zn.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ah.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://on.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oy.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://up.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nq.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sm.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iq.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tn.9csxet.cn

[A10] 生成随机数
来源：http://on.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://ns.colortex.cn

PHP:  random_int(1, 100);
来源：http://uk.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ra.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vs.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://od.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://is.szxytkj.cn

Ruby: rand(1..100)
来源：http://vl.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://in.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://ky.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://ql.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ws.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ss.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sy.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://pq.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xk.huanxung.cn


<!-- 参考信息 -->