代发 wailian999

[U61] PHP：正则
来源：http://uy.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gv.9csxet.cn

[U62] PHP：日期对象
来源：http://mr.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yh.nicolike.cn

[U63] PHP：文件读写
来源：http://oj.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vy.hahajie.cn

[U64] PHP：目录遍历
来源：http://de.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://eb.bookmarksfly.cn

[U65] PHP：会话
来源：http://gg.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qz.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://ig.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xe.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://qw.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oc.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://fm.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://to.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://rx.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yo.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://iy.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wu.shxzukj.cn

[U71] PHP：抛出异常
来源：http://ys.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://fl.szxytkj.cn

[U72] PHP：写错误日志
来源：http://sf.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://tc.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://tg.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://jp.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://qk.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://hy.shxzskj.cn

[U75] PHP：依赖注入
来源：http://fj.jctech888.com.cn

composer require psr/container
来源：http://fv.gzmigu.cn

[U76] PHP：简单路由
来源：http://zw.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rz.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://ua.nszjky.cn

composer require twig/twig
来源：http://gx.9csxet.cn

[U78] PHP：单元测试
来源：http://at.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://jx.chemitech.net.cn

[U79] PHP：静态分析
来源：http://vp.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://ny.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://ly.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uz.nicolike.cn

[U81] JS：初始化项目
来源：http://rm.colortex.cn

npm init -y;  npm i express
来源：http://yk.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://um.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ju.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://sw.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hh.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://zs.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fi.wgjwhj.cn

[U85] JS：可选链
来源：http://ax.hahajie.cn

a?.b?.c
来源：http://ot.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://he.colortex.cn

a ?? b
来源：http://in.huanxung.cn

[U87] JS：解构默认值
来源：http://pn.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://pr.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://bk.nicolike.cn

{ ...a, ...b }
来源：http://qz.shxzskj.cn

[U89] JS：数组去重
来源：http://yh.wgjwhj.cn

[...new Set(arr)]
来源：http://zp.lnxyls.cn

[U90] JS：数字数组排序
来源：http://ui.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://ab.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://vk.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://to.szsharing.cn

[U92] JS：深拷贝
来源：http://dv.hahajie.cn

structuredClone(obj)
来源：http://di.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://zh.shxzskj.cn

`共 ${n} 条`
来源：http://lp.chemitech.net.cn

[U94] JS：箭头函数
来源：http://sf.szxytkj.cn

const double = x => x * 2;
来源：http://pk.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://jm.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://gh.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://sj.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mw.newstarts.cn

[U97] JS：并发请求
来源：http://lh.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ar.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://vv.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yg.hnjuh.cn

[U99] JS：事件监听
来源：http://dx.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://gc.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://oa.huanxung.cn

document.querySelector(".item")
来源：http://aa.wgjwhj.cn

[U101] JS：classList 操作
来源：http://eq.szxytkj.cn

el.classList.toggle("active")
来源：http://bn.szxytkj.cn

[U102] JS：本地存储
来源：http://rq.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://de.hahajie.cn

[U103] JS：定时器
来源：http://ng.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yl.szxytkj.cn

[U104] JS：防抖
来源：http://cy.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rq.shxzukj.cn

[U105] JS：节流
来源：http://td.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yl.yuexingan06.cn

[U106] JS：日期格式化
来源：http://bl.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tz.jctech888.com.cn

[U107] JS：数字千分位
来源：http://vn.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vz.bookmarksfly.cn

[U108] JS：随机整数
来源：http://xz.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yf.chemitech.net.cn

[U109] JS：数组分组
来源：http://ce.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://jj.hahajie.cn

[U110] JS：数组分块
来源：http://jf.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mh.newstarts.cn

[U111] JS：对象转 Map
来源：http://yx.hnjuh.cn

new Map(Object.entries(obj))
来源：http://gj.521024.cn

[U112] JS：字符串补位
来源：http://ku.gzmigu.cn

"7".padStart(3, "0")
来源：http://aw.colortex.cn

[U113] JS：正则替换全部
来源：http://og.shxzskj.cn

s.replaceAll("a", "b")
来源：http://iy.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://an.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nz.lnxyls.cn

[U115] JS：生成 UUID
来源：http://ou.szsharing.cn

crypto.randomUUID()
来源：http://lg.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://au.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://ld.nszjky.cn

[U117] JS：单元测试
来源：http://cc.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://jh.hnjuh.cn

[U118] JS：开发服务器
来源：http://lk.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://eo.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://vw.yuexingan06.cn

npx vite build
来源：http://pw.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://eq.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://rn.jctech888.com.cn

================================================================================
来源：http://yi.asd995.cn

统计汇总
来源：http://pu.shtwfgs.cn

================================================================================
来源：http://te.huanxung.cn

按语言统计（条）：
来源：http://dk.colortex.cn

Python ......... 252
来源：http://zu.gzmigu.cn

PHP ............ 252
来源：http://mf.bookmarksfly.cn

JavaScript ..... 252
来源：http://tq.asd995.cn

TypeScript ..... 212
来源：http://fw.lnxyls.cn

Java ........... 212
来源：http://er.hahajie.cn

Go ............. 212
来源：http://zk.521024.cn

Ruby ........... 212
来源：http://ei.nicolike.cn

C# ............. 212
来源：http://ai.bjjhwx.cn

C .............. 30
来源：http://wt.bjjhwx.cn

C++ ............ 30
来源：http://iu.shxzukj.cn

SQL ............ 90
来源：http://hq.haigaiapp.cn

Bash ........... 80
来源：http://yd.asd995.cn

Kotlin ......... 15
来源：http://xs.jctech888.com.cn

Swift .......... 15
来源：http://og.huanxung.cn

Lua ............ 10
来源：http://xi.shxzukj.cn

Perl ........... 10
来源：http://kt.bookmarksfly.cn

Scala .......... 10
来源：http://vd.colortex.cn

------------------------------------
来源：http://np.hnjuh.cn

合计 ........... 2106 条
来源：http://oc.chemitech.net.cn

按章节统计：
来源：http://wt.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jc.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ru.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mw.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rs.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ip.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oo.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ci.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ad.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rg.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://be.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ng.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mw.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mo.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mm.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iv.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yc.chemitech.net.cn

Q SQL 专题                              90
来源：http://qo.lnxyls.cn

R Bash 专题                             80
来源：http://wn.newstarts.cn

S C / C++ 专题                          60
来源：http://jk.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://md.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://dr.jctech888.com.cn

------------------------------------
来源：http://ui.bookmarksfly.cn

合计                                  2106 条
来源：http://he.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ss.bjjhwx.cn

使用提醒
来源：http://ac.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://lb.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xm.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ny.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xt.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mf.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kh.szxytkj.cn

—— 文件结束 ——
来源：http://ta.colortex.cn

================================================================================
来源：http://xw.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://ck.asd995.cn

Common Programming Examples Cheat Book
来源：http://bj.jianghongdianzi.cn

================================================================================
来源：http://cd.bookmarksfly.cn

【收录内容】
来源：http://pr.szsharing.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ma.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bn.wgjwhj.cn

SQL · Bash · C · C++
来源：http://nm.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fy.muxihuayi.cn

【使用说明】
来源：http://zi.bjjhwx.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yn.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gj.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cy.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ul.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ua.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ne.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wf.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fo.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ov.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fs.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tn.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ls.bookmarksfly.cn

【文件统计】
来源：http://im.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ca.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ux.nszjky.cn

目  录
来源：http://zp.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://td.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mo.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kn.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fs.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fc.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lz.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://we.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kx.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zd.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dg.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ek.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vk.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yl.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://by.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rg.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kt.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pq.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wn.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tl.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wh.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hm.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zo.huixiangedu.cn

================================================================================
来源：http://lp.hahajie.cn

A. 基础语法与类型
来源：http://ja.521024.cn

================================================================================
来源：http://pe.yuexingan06.cn

[A01] Hello World
来源：http://qi.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://df.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://oq.521024.cn

JS:   console.log("Hello, World!");
来源：http://rm.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rp.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://mm.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://sn.asd995.cn

Ruby: puts "Hello, World!"
来源：http://ds.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zb.shxzukj.cn

[A02] 变量声明与赋值
来源：http://lx.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lj.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ef.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wn.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nt.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://xc.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://eg.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://bl.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fk.lnxyls.cn

[A03] 常量定义
来源：http://re.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yn.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://no.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://ff.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://qz.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://ui.lnxyls.cn

Go:   const PI = 3.14159
来源：http://va.szxytkj.cn

Ruby: PI = 3.14159
来源：http://ly.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://ch.haigaiapp.cn

[A04] 判断变量类型
来源：http://jo.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vy.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vj.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gs.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://sv.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wx.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fr.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hu.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://pi.jctech888.com.cn

[A05] 整数除法与取模
来源：http://ez.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sq.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ac.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hf.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rg.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://vc.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://pa.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://eo.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://ie.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://pe.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://ib.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oh.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bb.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nu.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fe.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wd.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rl.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bv.yuexingan06.cn

[A07] 数字转字符串
来源：http://zb.huixinmuqiang.cn

Py:   str(42)
来源：http://qb.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://cf.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://ww.yuexingan06.cn

TS:   String(42)
来源：http://ph.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lh.colortex.cn

Go:   strconv.Itoa(42)
来源：http://gl.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://me.wgjwhj.cn

C#:   42.ToString()
来源：http://ba.hnjuh.cn

[A08] 取整与四舍五入
来源：http://jb.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://be.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://on.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kc.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wp.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lm.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ra.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xx.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ao.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://nl.huixinmuqiang.cn


<!-- 参考信息 -->