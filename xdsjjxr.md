代发 wailian999

[U65] PHP：会话
来源：http://pt.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wr.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://qn.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ol.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://mv.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ej.asd995.cn

[U68] PHP：PDO 连接
来源：http://dq.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://av.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://op.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yv.hahajie.cn

[U70] PHP：PDO 事务
来源：http://un.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hr.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://kg.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://sg.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://hb.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://am.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://jq.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://pd.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://ci.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://qu.asd995.cn

[U75] PHP：依赖注入
来源：http://az.szsharing.cn

composer require psr/container
来源：http://re.shtwfgs.cn

[U76] PHP：简单路由
来源：http://ka.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rg.lnxyls.cn

[U77] PHP：模板渲染
来源：http://xb.shxzskj.cn

composer require twig/twig
来源：http://dj.colortex.cn

[U78] PHP：单元测试
来源：http://rv.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://gu.wgjwhj.cn

[U79] PHP：静态分析
来源：http://ol.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://zf.colortex.cn

[U80] PHP：代码规范修复
来源：http://sh.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kt.nszjky.cn

[U81] JS：初始化项目
来源：http://ob.muxihuayi.cn

npm init -y;  npm i express
来源：http://ip.huanxung.cn

[U82] JS：package.json 脚本
来源：http://hk.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ru.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://jp.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jy.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://zf.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kd.yuexingan06.cn

[U85] JS：可选链
来源：http://mt.panjiajie.cn

a?.b?.c
来源：http://pw.9csxet.cn

[U86] JS：空值合并
来源：http://nc.nszjky.cn

a ?? b
来源：http://gc.haigaiapp.cn

[U87] JS：解构默认值
来源：http://sf.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://kb.newstarts.cn

[U88] JS：对象展开合并
来源：http://vd.huixinmuqiang.cn

{ ...a, ...b }
来源：http://sh.521024.cn

[U89] JS：数组去重
来源：http://hl.chemitech.net.cn

[...new Set(arr)]
来源：http://ve.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://ji.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://th.asd995.cn

[U91] JS：对象键值遍历
来源：http://qe.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://op.chemitech.net.cn

[U92] JS：深拷贝
来源：http://ml.szxytkj.cn

structuredClone(obj)
来源：http://uh.huanxung.cn

[U93] JS：模板字符串
来源：http://sh.hahajie.cn

`共 ${n} 条`
来源：http://fe.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://ar.huixinmuqiang.cn

const double = x => x * 2;
来源：http://xb.colortex.cn

[U95] JS：Promise 包装
来源：http://xe.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://nv.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://tj.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hq.haigaiapp.cn

[U97] JS：并发请求
来源：http://jf.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fw.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://zb.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ru.chemitech.net.cn

[U99] JS：事件监听
来源：http://hm.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://rz.newstarts.cn

[U100] JS：DOM 查询
来源：http://pz.nszjky.cn

document.querySelector(".item")
来源：http://lr.shxzskj.cn

[U101] JS：classList 操作
来源：http://hj.hnjuh.cn

el.classList.toggle("active")
来源：http://tz.shxzukj.cn

[U102] JS：本地存储
来源：http://es.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qv.colortex.cn

[U103] JS：定时器
来源：http://vk.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cs.szsharing.cn

[U104] JS：防抖
来源：http://xv.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mu.nszjky.cn

[U105] JS：节流
来源：http://yj.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rh.muxihuayi.cn

[U106] JS：日期格式化
来源：http://mc.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wp.yuexingan06.cn

[U107] JS：数字千分位
来源：http://hy.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eh.wgjwhj.cn

[U108] JS：随机整数
来源：http://iq.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oh.szxytkj.cn

[U109] JS：数组分组
来源：http://uw.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://ab.nicolike.cn

[U110] JS：数组分块
来源：http://jm.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sr.gzmigu.cn

[U111] JS：对象转 Map
来源：http://lw.nszjky.cn

new Map(Object.entries(obj))
来源：http://kz.huanxung.cn

[U112] JS：字符串补位
来源：http://yw.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://jw.9csxet.cn

[U113] JS：正则替换全部
来源：http://bl.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://py.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://sp.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kh.lnxyls.cn

[U115] JS：生成 UUID
来源：http://jg.jctech888.com.cn

crypto.randomUUID()
来源：http://vp.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://oi.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://hp.chemitech.net.cn

[U117] JS：单元测试
来源：http://jo.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://to.gzmigu.cn

[U118] JS：开发服务器
来源：http://tv.shxzukj.cn

npm i -D vite;  npx vite
来源：http://ml.asd995.cn

[U119] JS：生产构建
来源：http://bk.jianghongdianzi.cn

npx vite build
来源：http://an.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://dx.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://fj.szsharing.cn

================================================================================
来源：http://jm.huixiangedu.cn

统计汇总
来源：http://zn.hahajie.cn

================================================================================
来源：http://ol.yuexingan06.cn

按语言统计（条）：
来源：http://ar.jctech888.com.cn

Python ......... 252
来源：http://sk.panjiajie.cn

PHP ............ 252
来源：http://xw.szsharing.cn

JavaScript ..... 252
来源：http://ib.huixiangedu.cn

TypeScript ..... 212
来源：http://kv.szxytkj.cn

Java ........... 212
来源：http://kv.hahajie.cn

Go ............. 212
来源：http://sk.nszjky.cn

Ruby ........... 212
来源：http://ed.szxytkj.cn

C# ............. 212
来源：http://qp.lnxyls.cn

C .............. 30
来源：http://lf.gzmigu.cn

C++ ............ 30
来源：http://ug.asd995.cn

SQL ............ 90
来源：http://sq.shxzukj.cn

Bash ........... 80
来源：http://hi.shxzskj.cn

Kotlin ......... 15
来源：http://vg.huixiangedu.cn

Swift .......... 15
来源：http://zx.muxihuayi.cn

Lua ............ 10
来源：http://sc.chemitech.net.cn

Perl ........... 10
来源：http://lc.521024.cn

Scala .......... 10
来源：http://lh.newstarts.cn

------------------------------------
来源：http://eu.hnjuh.cn

合计 ........... 2106 条
来源：http://cf.shxzskj.cn

按章节统计：
来源：http://mh.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jf.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xh.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zp.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ve.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kf.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ho.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bz.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xy.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sq.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bt.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yv.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rf.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ww.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gz.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jm.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cr.bjjhwx.cn

Q SQL 专题                              90
来源：http://zr.asd995.cn

R Bash 专题                             80
来源：http://nf.newstarts.cn

S C / C++ 专题                          60
来源：http://ye.newstarts.cn

T 其他语言补充                          60
来源：http://wv.jctech888.com.cn

U 高频实用片段                         120
来源：http://xm.nicolike.cn

------------------------------------
来源：http://xu.panjiajie.cn

合计                                  2106 条
来源：http://ks.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://wa.muxihuayi.cn

使用提醒
来源：http://tx.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://eh.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dy.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jq.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://au.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yt.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xl.bookmarksfly.cn

—— 文件结束 ——
来源：http://jh.colortex.cn

================================================================================
来源：http://wx.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://yz.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://gz.bookmarksfly.cn

================================================================================
来源：http://lp.huixinmuqiang.cn

【收录内容】
来源：http://rv.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bu.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hy.colortex.cn

SQL · Bash · C · C++
来源：http://cl.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yp.bjjhwx.cn

【使用说明】
来源：http://xv.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pc.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ac.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hk.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tu.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fp.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ir.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ib.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yw.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fa.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nb.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pw.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mv.lnxyls.cn

【文件统计】
来源：http://im.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fl.huanxung.cn

--------------------------------------------------------------------------------
来源：http://hg.panjiajie.cn

目  录
来源：http://ya.nszjky.cn

--------------------------------------------------------------------------------
来源：http://ze.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ed.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hs.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ex.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wb.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sj.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tz.shxzukj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lj.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jk.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zp.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eq.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zf.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://me.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ts.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gw.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://al.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kf.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ne.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yp.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pu.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rv.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rn.gzmigu.cn

================================================================================
来源：http://hy.huanxung.cn

A. 基础语法与类型
来源：http://rj.huanxung.cn

================================================================================
来源：http://ui.nicolike.cn

[A01] Hello World
来源：http://jy.jctech888.com.cn

Py:   print("Hello, World!")
来源：http://hx.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://hd.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://wc.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ez.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://gv.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://px.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://fq.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ys.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://kw.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://as.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wb.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://im.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qb.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://bq.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://wn.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://nh.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cb.huixiangedu.cn

[A03] 常量定义
来源：http://hk.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ne.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://gz.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://ha.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://wu.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://lw.asd995.cn

Go:   const PI = 3.14159
来源：http://sr.shxzukj.cn

Ruby: PI = 3.14159
来源：http://yk.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://ox.huixiangedu.cn

[A04] 判断变量类型
来源：http://fm.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://du.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ls.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vz.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://xy.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hi.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oa.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kj.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://bs.shtwfgs.cn

[A05] 整数除法与取模
来源：http://qs.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://px.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ju.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oy.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yr.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://vn.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://lb.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://mh.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://bl.9csxet.cn

[A06] 字符串转数字
来源：http://jy.colortex.cn

Py:   int("42"); float("3.14")
来源：http://cc.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wq.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xr.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fc.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yd.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oh.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bc.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vc.shxzukj.cn

[A07] 数字转字符串
来源：http://vc.huixinmuqiang.cn

Py:   str(42)
来源：http://nd.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://np.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://zg.huanxung.cn

TS:   String(42)
来源：http://rq.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://co.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://wu.colortex.cn

Ruby: 42.to_s
来源：http://yo.hahajie.cn

C#:   42.ToString()
来源：http://mi.521024.cn

[A08] 取整与四舍五入
来源：http://kr.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nm.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xp.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hk.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tv.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oc.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pc.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ob.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mk.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://eu.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mw.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nq.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tr.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ig.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iv.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vr.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qz.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sq.szsharing.cn


<!-- 参考信息 -->