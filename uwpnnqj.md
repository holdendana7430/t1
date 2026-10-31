代发 wailian999

[U71] PHP：抛出异常
来源：http://tf.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://ih.shxzukj.cn

[U72] PHP：写错误日志
来源：http://au.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://wn.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://ga.521024.cn

parse_ini_file("config.ini", true)
来源：http://ur.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://tt.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://yi.nszjky.cn

[U75] PHP：依赖注入
来源：http://rc.shtwfgs.cn

composer require psr/container
来源：http://ht.asd995.cn

[U76] PHP：简单路由
来源：http://nj.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ys.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://pv.521024.cn

composer require twig/twig
来源：http://co.yuexingan06.cn

[U78] PHP：单元测试
来源：http://sb.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://zi.asd995.cn

[U79] PHP：静态分析
来源：http://oe.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://kz.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://zp.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kx.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://no.szxytkj.cn

npm init -y;  npm i express
来源：http://hr.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://el.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ed.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://cp.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bf.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://op.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jf.huixiangedu.cn

[U85] JS：可选链
来源：http://vu.yuntaijiaju.cn

a?.b?.c
来源：http://ja.521024.cn

[U86] JS：空值合并
来源：http://xy.yuexingan06.cn

a ?? b
来源：http://eu.shxzukj.cn

[U87] JS：解构默认值
来源：http://oc.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://kz.hahajie.cn

[U88] JS：对象展开合并
来源：http://pj.shxzukj.cn

{ ...a, ...b }
来源：http://hu.haigaiapp.cn

[U89] JS：数组去重
来源：http://uh.bookmarksfly.cn

[...new Set(arr)]
来源：http://mc.hahajie.cn

[U90] JS：数字数组排序
来源：http://cg.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://ut.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://yg.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ti.huanxung.cn

[U92] JS：深拷贝
来源：http://dv.colortex.cn

structuredClone(obj)
来源：http://he.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://nm.hahajie.cn

`共 ${n} 条`
来源：http://ju.szsharing.cn

[U94] JS：箭头函数
来源：http://qf.chemitech.net.cn

const double = x => x * 2;
来源：http://mi.nszjky.cn

[U95] JS：Promise 包装
来源：http://en.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://ly.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://je.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ar.szxytkj.cn

[U97] JS：并发请求
来源：http://pa.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uu.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://re.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rw.nicolike.cn

[U99] JS：事件监听
来源：http://vd.newstarts.cn

el.addEventListener("click", e => {})
来源：http://pf.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://pb.colortex.cn

document.querySelector(".item")
来源：http://gw.gzmigu.cn

[U101] JS：classList 操作
来源：http://mt.szsharing.cn

el.classList.toggle("active")
来源：http://kd.jctech888.com.cn

[U102] JS：本地存储
来源：http://vn.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ay.jianghongdianzi.cn

[U103] JS：定时器
来源：http://ca.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ta.chemitech.net.cn

[U104] JS：防抖
来源：http://te.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://my.gzmigu.cn

[U105] JS：节流
来源：http://bf.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tc.hahajie.cn

[U106] JS：日期格式化
来源：http://ra.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yv.colortex.cn

[U107] JS：数字千分位
来源：http://ki.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bm.shxzukj.cn

[U108] JS：随机整数
来源：http://fs.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zk.huanxung.cn

[U109] JS：数组分组
来源：http://ou.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://xl.hahajie.cn

[U110] JS：数组分块
来源：http://hn.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rz.asd995.cn

[U111] JS：对象转 Map
来源：http://it.9csxet.cn

new Map(Object.entries(obj))
来源：http://rm.shxzukj.cn

[U112] JS：字符串补位
来源：http://ui.chemitech.net.cn

"7".padStart(3, "0")
来源：http://yq.szsharing.cn

[U113] JS：正则替换全部
来源：http://eu.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://iu.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://ly.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gy.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://ne.nicolike.cn

crypto.randomUUID()
来源：http://js.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://ej.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://bq.nszjky.cn

[U117] JS：单元测试
来源：http://uu.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://pl.szsharing.cn

[U118] JS：开发服务器
来源：http://hy.colortex.cn

npm i -D vite;  npx vite
来源：http://ro.gzmigu.cn

[U119] JS：生产构建
来源：http://rn.asd995.cn

npx vite build
来源：http://gd.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://dq.521024.cn

import.meta.env.VITE_API_URL
来源：http://ck.gzmigu.cn

================================================================================
来源：http://jz.szsharing.cn

统计汇总
来源：http://aq.shxzskj.cn

================================================================================
来源：http://mt.shxzskj.cn

按语言统计（条）：
来源：http://ew.asd995.cn

Python ......... 252
来源：http://qm.hnjuh.cn

PHP ............ 252
来源：http://hc.gzmigu.cn

JavaScript ..... 252
来源：http://ct.bjjhwx.cn

TypeScript ..... 212
来源：http://da.szsharing.cn

Java ........... 212
来源：http://ky.521024.cn

Go ............. 212
来源：http://oi.newstarts.cn

Ruby ........... 212
来源：http://cb.asd995.cn

C# ............. 212
来源：http://gq.gzmigu.cn

C .............. 30
来源：http://dl.huixiangedu.cn

C++ ............ 30
来源：http://xy.szsharing.cn

SQL ............ 90
来源：http://zt.muxihuayi.cn

Bash ........... 80
来源：http://uj.yuexingan06.cn

Kotlin ......... 15
来源：http://xn.jianghongdianzi.cn

Swift .......... 15
来源：http://kd.gzmigu.cn

Lua ............ 10
来源：http://hq.hnjuh.cn

Perl ........... 10
来源：http://er.colortex.cn

Scala .......... 10
来源：http://mt.shxzskj.cn

------------------------------------
来源：http://rs.jctech888.com.cn

合计 ........... 2106 条
来源：http://rx.asd995.cn

按章节统计：
来源：http://un.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zg.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pl.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ly.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pc.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aw.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zy.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jq.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gu.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yd.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://at.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dv.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://br.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cm.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://se.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mw.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xf.colortex.cn

Q SQL 专题                              90
来源：http://ce.yuexingan06.cn

R Bash 专题                             80
来源：http://sz.colortex.cn

S C / C++ 专题                          60
来源：http://wu.nszjky.cn

T 其他语言补充                          60
来源：http://ah.hahajie.cn

U 高频实用片段                         120
来源：http://al.asd995.cn

------------------------------------
来源：http://xc.9csxet.cn

合计                                  2106 条
来源：http://ov.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://yw.colortex.cn

使用提醒
来源：http://ac.asd995.cn

--------------------------------------------------------------------------------
来源：http://ij.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eu.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wg.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hp.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lk.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://su.nicolike.cn

—— 文件结束 ——
来源：http://os.nicolike.cn

================================================================================
来源：http://en.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://hy.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://nu.nszjky.cn

================================================================================
来源：http://be.huixinmuqiang.cn

【收录内容】
来源：http://zk.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ra.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yq.9csxet.cn

SQL · Bash · C · C++
来源：http://oi.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rw.muxihuayi.cn

【使用说明】
来源：http://ud.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://id.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://me.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nr.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pz.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xt.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jo.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mw.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qr.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rx.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kg.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ic.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eu.szsharing.cn

【文件统计】
来源：http://uv.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yf.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://wp.nszjky.cn

目  录
来源：http://ud.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://he.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jg.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tx.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://me.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ln.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pv.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://td.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://am.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xf.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wh.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zi.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oh.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gn.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zs.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ei.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bj.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rp.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tl.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nd.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oi.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yb.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wn.jianghongdianzi.cn

================================================================================
来源：http://bs.bookmarksfly.cn

A. 基础语法与类型
来源：http://se.asd995.cn

================================================================================
来源：http://ci.bookmarksfly.cn

[A01] Hello World
来源：http://on.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://ou.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://og.colortex.cn

JS:   console.log("Hello, World!");
来源：http://di.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hi.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://zu.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://fj.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://tw.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mn.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://fm.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://th.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ql.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bp.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://si.wgjwhj.cn

Java: String name = "Alex"; int age = 20;
来源：http://wf.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://ef.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://bi.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://je.colortex.cn

[A03] 常量定义
来源：http://rg.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fy.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://ge.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://vw.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://ei.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://kt.asd995.cn

Go:   const PI = 3.14159
来源：http://wy.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://je.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://eq.colortex.cn

[A04] 判断变量类型
来源：http://eb.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fb.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hx.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aj.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://ys.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lz.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nh.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xs.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://wu.chemitech.net.cn

[A05] 整数除法与取模
来源：http://zg.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yu.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vn.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yk.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ex.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://kr.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://vz.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://xc.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://cg.nicolike.cn

[A06] 字符串转数字
来源：http://ht.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://rv.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jw.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ci.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://he.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ar.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jt.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jx.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dn.wgjwhj.cn

[A07] 数字转字符串
来源：http://tf.jctech888.com.cn

Py:   str(42)
来源：http://sb.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://fn.9csxet.cn

JS:   String(42); (42).toString()
来源：http://gp.huixinmuqiang.cn

TS:   String(42)
来源：http://ji.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ot.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://tc.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://nw.shxzukj.cn

C#:   42.ToString()
来源：http://qi.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://hk.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ug.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gn.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bq.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wq.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wq.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kw.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://za.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ne.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://rv.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zv.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gc.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bg.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dm.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yo.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vm.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cn.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hr.huixiangedu.cn

[A10] 生成随机数
来源：http://lp.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://kz.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://vz.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kw.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wt.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://kk.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ui.huanxung.cn

Ruby: rand(1..100)
来源：http://tr.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://sx.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://dp.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://ig.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bn.haigaiapp.cn


<!-- 参考信息 -->