代发 wailian999

[U69] PHP：PDO 预处理
来源：http://kd.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mb.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://lq.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nx.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://hf.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://sj.521024.cn

[U72] PHP：写错误日志
来源：http://dc.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://zr.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://sb.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://cm.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://mx.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://zw.shxzskj.cn

[U75] PHP：依赖注入
来源：http://tc.hahajie.cn

composer require psr/container
来源：http://ii.hnjuh.cn

[U76] PHP：简单路由
来源：http://bv.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ix.szsharing.cn

[U77] PHP：模板渲染
来源：http://sj.hnjuh.cn

composer require twig/twig
来源：http://rm.shxzukj.cn

[U78] PHP：单元测试
来源：http://bb.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://gj.shtwfgs.cn

[U79] PHP：静态分析
来源：http://ux.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://pu.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://dw.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://th.szxytkj.cn

[U81] JS：初始化项目
来源：http://se.panjiajie.cn

npm init -y;  npm i express
来源：http://er.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://xy.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fr.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://cb.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vx.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://ps.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ns.haigaiapp.cn

[U85] JS：可选链
来源：http://vf.yuexingan06.cn

a?.b?.c
来源：http://ol.huixiangedu.cn

[U86] JS：空值合并
来源：http://bg.9csxet.cn

a ?? b
来源：http://ye.panjiajie.cn

[U87] JS：解构默认值
来源：http://nx.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://kq.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://qm.bookmarksfly.cn

{ ...a, ...b }
来源：http://xc.bookmarksfly.cn

[U89] JS：数组去重
来源：http://xd.huanxung.cn

[...new Set(arr)]
来源：http://lx.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://nj.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://ma.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://vp.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ea.nicolike.cn

[U92] JS：深拷贝
来源：http://bi.szxytkj.cn

structuredClone(obj)
来源：http://cg.hnjuh.cn

[U93] JS：模板字符串
来源：http://tm.bookmarksfly.cn

`共 ${n} 条`
来源：http://qe.hnjuh.cn

[U94] JS：箭头函数
来源：http://cs.jctech888.com.cn

const double = x => x * 2;
来源：http://jx.newstarts.cn

[U95] JS：Promise 包装
来源：http://vn.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://pf.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://ij.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lr.9csxet.cn

[U97] JS：并发请求
来源：http://sv.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zk.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://hh.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cs.521024.cn

[U99] JS：事件监听
来源：http://yl.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://ch.newstarts.cn

[U100] JS：DOM 查询
来源：http://qa.gzmigu.cn

document.querySelector(".item")
来源：http://jt.newstarts.cn

[U101] JS：classList 操作
来源：http://mm.szxytkj.cn

el.classList.toggle("active")
来源：http://wt.haigaiapp.cn

[U102] JS：本地存储
来源：http://bs.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rl.huixinmuqiang.cn

[U103] JS：定时器
来源：http://vs.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vp.panjiajie.cn

[U104] JS：防抖
来源：http://xq.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cb.huixinmuqiang.cn

[U105] JS：节流
来源：http://tj.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ja.haigaiapp.cn

[U106] JS：日期格式化
来源：http://xi.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fh.colortex.cn

[U107] JS：数字千分位
来源：http://kw.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uk.chemitech.net.cn

[U108] JS：随机整数
来源：http://bx.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ki.huixiangedu.cn

[U109] JS：数组分组
来源：http://pv.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://zo.gzmigu.cn

[U110] JS：数组分块
来源：http://hc.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gl.panjiajie.cn

[U111] JS：对象转 Map
来源：http://km.szsharing.cn

new Map(Object.entries(obj))
来源：http://wq.newstarts.cn

[U112] JS：字符串补位
来源：http://qt.nszjky.cn

"7".padStart(3, "0")
来源：http://hq.9csxet.cn

[U113] JS：正则替换全部
来源：http://dj.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://zl.asd995.cn

[U114] JS：JSON 深比较
来源：http://qx.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qc.colortex.cn

[U115] JS：生成 UUID
来源：http://ob.hahajie.cn

crypto.randomUUID()
来源：http://fq.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://mc.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://tc.huixiangedu.cn

[U117] JS：单元测试
来源：http://ia.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://vj.huixiangedu.cn

[U118] JS：开发服务器
来源：http://xq.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://zo.haigaiapp.cn

[U119] JS：生产构建
来源：http://fr.jianghongdianzi.cn

npx vite build
来源：http://hi.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://ly.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://wd.jianghongdianzi.cn

================================================================================
来源：http://ja.panjiajie.cn

统计汇总
来源：http://xb.colortex.cn

================================================================================
来源：http://xs.yuntaijiaju.cn

按语言统计（条）：
来源：http://jc.huixiangedu.cn

Python ......... 252
来源：http://ld.shxzukj.cn

PHP ............ 252
来源：http://xx.nicolike.cn

JavaScript ..... 252
来源：http://sm.jianghongdianzi.cn

TypeScript ..... 212
来源：http://eh.huixiangedu.cn

Java ........... 212
来源：http://ye.haigaiapp.cn

Go ............. 212
来源：http://xa.hnjuh.cn

Ruby ........... 212
来源：http://hc.yuexingan06.cn

C# ............. 212
来源：http://og.chemitech.net.cn

C .............. 30
来源：http://ro.colortex.cn

C++ ............ 30
来源：http://xb.9csxet.cn

SQL ............ 90
来源：http://la.szsharing.cn

Bash ........... 80
来源：http://gt.haigaiapp.cn

Kotlin ......... 15
来源：http://ty.nszjky.cn

Swift .......... 15
来源：http://qz.colortex.cn

Lua ............ 10
来源：http://vu.gzmigu.cn

Perl ........... 10
来源：http://oi.huixiangedu.cn

Scala .......... 10
来源：http://lk.lnxyls.cn

------------------------------------
来源：http://gh.huanxung.cn

合计 ........... 2106 条
来源：http://dx.asd995.cn

按章节统计：
来源：http://qw.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nk.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ww.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sl.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ee.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://no.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://da.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://os.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ou.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wj.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://in.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zn.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ob.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rh.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://go.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dm.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mr.newstarts.cn

Q SQL 专题                              90
来源：http://qz.asd995.cn

R Bash 专题                             80
来源：http://dd.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://sj.haigaiapp.cn

T 其他语言补充                          60
来源：http://cq.haigaiapp.cn

U 高频实用片段                         120
来源：http://te.yuntaijiaju.cn

------------------------------------
来源：http://ou.hnjuh.cn

合计                                  2106 条
来源：http://kp.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://hi.szsharing.cn

使用提醒
来源：http://cj.521024.cn

--------------------------------------------------------------------------------
来源：http://ih.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sl.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ui.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ay.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://di.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wv.wgjwhj.cn

—— 文件结束 ——
来源：http://tx.colortex.cn

================================================================================
来源：http://qd.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://dn.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://wo.haigaiapp.cn

================================================================================
来源：http://gg.hnjuh.cn

【收录内容】
来源：http://tb.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lz.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bi.hahajie.cn

SQL · Bash · C · C++
来源：http://nw.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fg.nszjky.cn

【使用说明】
来源：http://pf.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jd.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xs.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hk.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bj.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nb.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ea.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cf.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fi.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nm.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ow.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ky.huixinmuqiang.cn

【文件统计】
来源：http://ky.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qq.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://vp.huixinmuqiang.cn

目  录
来源：http://zr.newstarts.cn

--------------------------------------------------------------------------------
来源：http://zh.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nk.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pl.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tl.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mb.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lt.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wi.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sc.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sj.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dm.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jh.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gu.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vb.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yl.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sb.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zc.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kg.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gv.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gb.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://si.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jq.lnxyls.cn

================================================================================
来源：http://ra.asd995.cn

A. 基础语法与类型
来源：http://db.muxihuayi.cn

================================================================================
来源：http://dy.shtwfgs.cn

[A01] Hello World
来源：http://bo.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://jo.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://xg.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://oe.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jx.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://jh.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://pl.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://jo.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fr.panjiajie.cn

[A02] 变量声明与赋值
来源：http://nf.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ko.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dz.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ft.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ji.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://uh.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://pp.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://rd.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ep.newstarts.cn

[A03] 常量定义
来源：http://bi.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ws.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://wy.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://zf.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://kv.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://zt.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://np.szsharing.cn

Ruby: PI = 3.14159
来源：http://hj.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://sw.nszjky.cn

[A04] 判断变量类型
来源：http://sd.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yu.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://od.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rf.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://wn.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dd.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://so.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gn.521024.cn

C#:   x.GetType().Name; x is int
来源：http://lx.haigaiapp.cn

[A05] 整数除法与取模
来源：http://ab.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oq.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jq.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bv.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kz.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://ec.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://yt.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://of.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://of.nicolike.cn

[A06] 字符串转数字
来源：http://en.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://pd.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://th.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tt.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://es.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dy.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oj.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gk.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cg.yuexingan06.cn

[A07] 数字转字符串
来源：http://cq.newstarts.cn

Py:   str(42)
来源：http://yh.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://jl.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://hg.bookmarksfly.cn

TS:   String(42)
来源：http://ll.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yr.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://gm.jctech888.com.cn

Ruby: 42.to_s
来源：http://pj.nicolike.cn

C#:   42.ToString()
来源：http://tb.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://xv.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vq.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://it.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ve.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://om.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pt.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://os.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zc.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tv.asd995.cn

[A09] 绝对值与最大最小值
来源：http://li.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vk.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://at.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cz.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lc.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yu.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fk.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gn.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ot.newstarts.cn

[A10] 生成随机数
来源：http://lp.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://mw.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://ib.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zi.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yy.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://bm.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uc.asd995.cn

Ruby: rand(1..100)
来源：http://he.bookmarksfly.cn


<!-- 参考信息 -->