代发 wailian999

[U63] PHP：文件读写
来源：http://vv.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hd.newstarts.cn

[U64] PHP：目录遍历
来源：http://wk.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://xo.bjjhwx.cn

[U65] PHP：会话
来源：http://yf.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bl.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://aa.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zi.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://yd.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qd.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://hs.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gm.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://dd.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tx.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://cr.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pl.szxytkj.cn

[U71] PHP：抛出异常
来源：http://yc.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://jq.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://hg.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://zj.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://vr.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://dd.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://yw.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://xw.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://ax.shxzukj.cn

composer require psr/container
来源：http://hx.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://fq.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cd.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://mu.colortex.cn

composer require twig/twig
来源：http://wx.wgjwhj.cn

[U78] PHP：单元测试
来源：http://pn.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://lc.shxzukj.cn

[U79] PHP：静态分析
来源：http://hm.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://mp.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://hu.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zu.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://zu.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://nn.nszjky.cn

[U82] JS：package.json 脚本
来源：http://th.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nn.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://ks.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ct.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://og.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dd.lnxyls.cn

[U85] JS：可选链
来源：http://rr.huixiangedu.cn

a?.b?.c
来源：http://az.muxihuayi.cn

[U86] JS：空值合并
来源：http://lx.huixiangedu.cn

a ?? b
来源：http://iz.jctech888.com.cn

[U87] JS：解构默认值
来源：http://ut.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://xn.shxzukj.cn

[U88] JS：对象展开合并
来源：http://fk.nszjky.cn

{ ...a, ...b }
来源：http://pw.gzmigu.cn

[U89] JS：数组去重
来源：http://fn.chemitech.net.cn

[...new Set(arr)]
来源：http://ri.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://ac.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://fa.nszjky.cn

[U91] JS：对象键值遍历
来源：http://tw.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://au.nszjky.cn

[U92] JS：深拷贝
来源：http://rd.wgjwhj.cn

structuredClone(obj)
来源：http://br.shxzukj.cn

[U93] JS：模板字符串
来源：http://en.szxytkj.cn

`共 ${n} 条`
来源：http://nd.9csxet.cn

[U94] JS：箭头函数
来源：http://rf.asd995.cn

const double = x => x * 2;
来源：http://xv.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://mo.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://jm.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://xl.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bl.shxzskj.cn

[U97] JS：并发请求
来源：http://ul.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dt.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://it.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sk.jctech888.com.cn

[U99] JS：事件监听
来源：http://li.9csxet.cn

el.addEventListener("click", e => {})
来源：http://cs.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://tp.nszjky.cn

document.querySelector(".item")
来源：http://nm.muxihuayi.cn

[U101] JS：classList 操作
来源：http://ct.bjjhwx.cn

el.classList.toggle("active")
来源：http://fv.gzmigu.cn

[U102] JS：本地存储
来源：http://jg.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sg.shxzskj.cn

[U103] JS：定时器
来源：http://vo.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yb.yuexingan06.cn

[U104] JS：防抖
来源：http://no.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ut.huanxung.cn

[U105] JS：节流
来源：http://mo.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rb.shxzukj.cn

[U106] JS：日期格式化
来源：http://hs.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eh.asd995.cn

[U107] JS：数字千分位
来源：http://nr.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mp.newstarts.cn

[U108] JS：随机整数
来源：http://ju.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cl.szsharing.cn

[U109] JS：数组分组
来源：http://sm.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://sc.nicolike.cn

[U110] JS：数组分块
来源：http://ws.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sc.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://dw.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://mp.asd995.cn

[U112] JS：字符串补位
来源：http://zv.asd995.cn

"7".padStart(3, "0")
来源：http://fa.szxytkj.cn

[U113] JS：正则替换全部
来源：http://zf.colortex.cn

s.replaceAll("a", "b")
来源：http://rv.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://qb.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tt.gzmigu.cn

[U115] JS：生成 UUID
来源：http://aq.hahajie.cn

crypto.randomUUID()
来源：http://cj.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://un.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://ej.bjjhwx.cn

[U117] JS：单元测试
来源：http://vl.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://if.newstarts.cn

[U118] JS：开发服务器
来源：http://rg.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://if.colortex.cn

[U119] JS：生产构建
来源：http://rk.lnxyls.cn

npx vite build
来源：http://do.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://wt.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://ke.huixiangedu.cn

================================================================================
来源：http://uz.chemitech.net.cn

统计汇总
来源：http://kp.shxzukj.cn

================================================================================
来源：http://mj.lnxyls.cn

按语言统计（条）：
来源：http://hr.jianghongdianzi.cn

Python ......... 252
来源：http://kp.panjiajie.cn

PHP ............ 252
来源：http://vm.bjjhwx.cn

JavaScript ..... 252
来源：http://ag.521024.cn

TypeScript ..... 212
来源：http://ci.shxzskj.cn

Java ........... 212
来源：http://lp.huixiangedu.cn

Go ............. 212
来源：http://lv.jctech888.com.cn

Ruby ........... 212
来源：http://yl.haigaiapp.cn

C# ............. 212
来源：http://vp.haigaiapp.cn

C .............. 30
来源：http://bb.szsharing.cn

C++ ............ 30
来源：http://yk.chemitech.net.cn

SQL ............ 90
来源：http://bh.yuntaijiaju.cn

Bash ........... 80
来源：http://oo.colortex.cn

Kotlin ......... 15
来源：http://qr.shxzskj.cn

Swift .......... 15
来源：http://gd.newstarts.cn

Lua ............ 10
来源：http://if.9csxet.cn

Perl ........... 10
来源：http://sk.nicolike.cn

Scala .......... 10
来源：http://ro.haigaiapp.cn

------------------------------------
来源：http://ma.haigaiapp.cn

合计 ........... 2106 条
来源：http://dl.nicolike.cn

按章节统计：
来源：http://zy.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zy.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kx.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bu.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uk.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rr.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ac.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kw.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wd.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tp.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zj.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ke.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kz.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uh.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bh.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pc.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ec.huixiangedu.cn

Q SQL 专题                              90
来源：http://yg.asd995.cn

R Bash 专题                             80
来源：http://ab.bjjhwx.cn

S C / C++ 专题                          60
来源：http://tw.huanxung.cn

T 其他语言补充                          60
来源：http://wi.haigaiapp.cn

U 高频实用片段                         120
来源：http://ix.panjiajie.cn

------------------------------------
来源：http://rd.shxzskj.cn

合计                                  2106 条
来源：http://th.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://bz.huixiangedu.cn

使用提醒
来源：http://by.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://vq.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gi.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nr.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rl.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nw.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ft.huixiangedu.cn

—— 文件结束 ——
来源：http://wd.lnxyls.cn

================================================================================
来源：http://dv.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://es.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://zk.jianghongdianzi.cn

================================================================================
来源：http://ko.yuexingan06.cn

【收录内容】
来源：http://uc.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://eb.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nn.szxytkj.cn

SQL · Bash · C · C++
来源：http://qk.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ap.shxzukj.cn

【使用说明】
来源：http://zw.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cu.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ji.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qt.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vn.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ui.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xx.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fd.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://va.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uh.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xj.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ka.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mx.bookmarksfly.cn

【文件统计】
来源：http://ul.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://so.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://fh.nszjky.cn

目  录
来源：http://he.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ye.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qb.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qv.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qn.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ny.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uj.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wo.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mw.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ql.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dx.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ox.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lt.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nx.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ax.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ok.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tj.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ta.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ou.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gs.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qe.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bu.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dx.haigaiapp.cn

================================================================================
来源：http://qv.chemitech.net.cn

A. 基础语法与类型
来源：http://ll.newstarts.cn

================================================================================
来源：http://jy.chemitech.net.cn

[A01] Hello World
来源：http://mp.newstarts.cn

Py:   print("Hello, World!")
来源：http://zk.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://fk.521024.cn

JS:   console.log("Hello, World!");
来源：http://uy.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hy.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://iv.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://bb.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://ss.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ct.newstarts.cn

[A02] 变量声明与赋值
来源：http://nw.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ya.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mt.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dh.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jw.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://pa.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://cc.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://hy.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kj.jctech888.com.cn

[A03] 常量定义
来源：http://vh.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fp.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://iv.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://sp.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://hy.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://dk.colortex.cn

Go:   const PI = 3.14159
来源：http://tf.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://sv.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://ao.yuexingan06.cn

[A04] 判断变量类型
来源：http://bd.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vf.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sa.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mr.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://er.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nx.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pv.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ao.521024.cn

C#:   x.GetType().Name; x is int
来源：http://ox.yuexingan06.cn

[A05] 整数除法与取模
来源：http://tb.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lt.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tn.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jc.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ms.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://iw.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://bg.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://vu.521024.cn

C#:   7 / 2; 7 % 2
来源：http://jf.huanxung.cn

[A06] 字符串转数字
来源：http://hk.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://yu.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yu.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xf.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oq.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ih.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vk.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wt.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eu.shxzskj.cn

[A07] 数字转字符串
来源：http://uo.huixiangedu.cn

Py:   str(42)
来源：http://op.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://lp.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://gu.szsharing.cn

TS:   String(42)
来源：http://nw.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gj.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://sn.shtwfgs.cn

Ruby: 42.to_s
来源：http://tk.huanxung.cn

C#:   42.ToString()
来源：http://ms.hahajie.cn

[A08] 取整与四舍五入
来源：http://cg.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sz.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bo.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qx.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hq.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://an.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ao.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wz.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lf.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://iq.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xk.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tz.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nw.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wa.szsharing.cn


<!-- 参考信息 -->