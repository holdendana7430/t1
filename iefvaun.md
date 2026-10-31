代发 wailian999

[U63] PHP：文件读写
来源：http://cn.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xz.colortex.cn

[U64] PHP：目录遍历
来源：http://qb.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://bq.yuexingan06.cn

[U65] PHP：会话
来源：http://hr.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eu.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://nl.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dk.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://wm.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ln.colortex.cn

[U68] PHP：PDO 连接
来源：http://rz.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fo.521024.cn

[U69] PHP：PDO 预处理
来源：http://bv.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kt.nszjky.cn

[U70] PHP：PDO 事务
来源：http://yx.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yb.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://zx.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://al.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://yj.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://ny.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://jb.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://to.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://my.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://ak.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://po.newstarts.cn

composer require psr/container
来源：http://oo.bjjhwx.cn

[U76] PHP：简单路由
来源：http://oz.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kg.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://rf.newstarts.cn

composer require twig/twig
来源：http://ke.szsharing.cn

[U78] PHP：单元测试
来源：http://ep.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://zo.shxzskj.cn

[U79] PHP：静态分析
来源：http://mf.521024.cn

composer require --dev phpstan/phpstan
来源：http://sf.szsharing.cn

[U80] PHP：代码规范修复
来源：http://be.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zl.yuexingan06.cn

[U81] JS：初始化项目
来源：http://gp.bjjhwx.cn

npm init -y;  npm i express
来源：http://ab.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://kk.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rg.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://ff.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fi.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://pn.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bj.newstarts.cn

[U85] JS：可选链
来源：http://qb.nszjky.cn

a?.b?.c
来源：http://qk.chemitech.net.cn

[U86] JS：空值合并
来源：http://nv.newstarts.cn

a ?? b
来源：http://dt.huanxung.cn

[U87] JS：解构默认值
来源：http://sw.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://bp.asd995.cn

[U88] JS：对象展开合并
来源：http://dt.bjjhwx.cn

{ ...a, ...b }
来源：http://gu.hnjuh.cn

[U89] JS：数组去重
来源：http://po.panjiajie.cn

[...new Set(arr)]
来源：http://yh.hahajie.cn

[U90] JS：数字数组排序
来源：http://gf.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://jv.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://yh.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zp.panjiajie.cn

[U92] JS：深拷贝
来源：http://dk.huixinmuqiang.cn

structuredClone(obj)
来源：http://iv.panjiajie.cn

[U93] JS：模板字符串
来源：http://lv.yuntaijiaju.cn

`共 ${n} 条`
来源：http://ev.nicolike.cn

[U94] JS：箭头函数
来源：http://po.9csxet.cn

const double = x => x * 2;
来源：http://ds.panjiajie.cn

[U95] JS：Promise 包装
来源：http://bk.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://ic.nicolike.cn

[U96] JS：async/await 与异常
来源：http://la.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://km.hahajie.cn

[U97] JS：并发请求
来源：http://zj.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rg.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://xs.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dm.chemitech.net.cn

[U99] JS：事件监听
来源：http://ku.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://ug.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://ju.panjiajie.cn

document.querySelector(".item")
来源：http://ko.shxzskj.cn

[U101] JS：classList 操作
来源：http://rs.newstarts.cn

el.classList.toggle("active")
来源：http://fi.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://sk.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vq.huanxung.cn

[U103] JS：定时器
来源：http://so.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vf.yuntaijiaju.cn

[U104] JS：防抖
来源：http://ze.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xx.jianghongdianzi.cn

[U105] JS：节流
来源：http://ix.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oh.jctech888.com.cn

[U106] JS：日期格式化
来源：http://hz.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ns.huanxung.cn

[U107] JS：数字千分位
来源：http://yb.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hq.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://dp.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kb.jctech888.com.cn

[U109] JS：数组分组
来源：http://uu.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://di.nicolike.cn

[U110] JS：数组分块
来源：http://lq.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wv.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://jn.newstarts.cn

new Map(Object.entries(obj))
来源：http://wh.shxzukj.cn

[U112] JS：字符串补位
来源：http://ck.shxzukj.cn

"7".padStart(3, "0")
来源：http://gk.szsharing.cn

[U113] JS：正则替换全部
来源：http://po.nicolike.cn

s.replaceAll("a", "b")
来源：http://ed.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://jn.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bs.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://vk.shxzskj.cn

crypto.randomUUID()
来源：http://bm.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://dv.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://uv.chemitech.net.cn

[U117] JS：单元测试
来源：http://jz.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://pl.bjjhwx.cn

[U118] JS：开发服务器
来源：http://rx.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://kg.hnjuh.cn

[U119] JS：生产构建
来源：http://qq.yuexingan06.cn

npx vite build
来源：http://hk.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://cs.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://pn.hnjuh.cn

================================================================================
来源：http://ox.panjiajie.cn

统计汇总
来源：http://kr.huixinmuqiang.cn

================================================================================
来源：http://ev.bjjhwx.cn

按语言统计（条）：
来源：http://xs.hahajie.cn

Python ......... 252
来源：http://dh.chemitech.net.cn

PHP ............ 252
来源：http://iy.yuexingan06.cn

JavaScript ..... 252
来源：http://go.panjiajie.cn

TypeScript ..... 212
来源：http://el.huanxung.cn

Java ........... 212
来源：http://ii.huixinmuqiang.cn

Go ............. 212
来源：http://ae.shxzskj.cn

Ruby ........... 212
来源：http://du.szsharing.cn

C# ............. 212
来源：http://ru.nicolike.cn

C .............. 30
来源：http://dj.muxihuayi.cn

C++ ............ 30
来源：http://sg.shxzskj.cn

SQL ............ 90
来源：http://aa.521024.cn

Bash ........... 80
来源：http://dy.gzmigu.cn

Kotlin ......... 15
来源：http://jg.shxzskj.cn

Swift .......... 15
来源：http://uu.huixiangedu.cn

Lua ............ 10
来源：http://zw.shxzukj.cn

Perl ........... 10
来源：http://hb.9csxet.cn

Scala .......... 10
来源：http://mi.szsharing.cn

------------------------------------
来源：http://uy.521024.cn

合计 ........... 2106 条
来源：http://ap.nicolike.cn

按章节统计：
来源：http://da.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ro.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sk.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ns.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ui.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yd.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qm.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iw.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ds.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gz.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bt.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fe.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tt.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qi.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ky.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gj.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qk.jctech888.com.cn

Q SQL 专题                              90
来源：http://lm.huixinmuqiang.cn

R Bash 专题                             80
来源：http://gp.shtwfgs.cn

S C / C++ 专题                          60
来源：http://ng.wgjwhj.cn

T 其他语言补充                          60
来源：http://iq.shtwfgs.cn

U 高频实用片段                         120
来源：http://lg.haigaiapp.cn

------------------------------------
来源：http://ji.hnjuh.cn

合计                                  2106 条
来源：http://vf.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://um.newstarts.cn

使用提醒
来源：http://do.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://gd.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pd.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ij.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fq.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sn.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kz.shtwfgs.cn

—— 文件结束 ——
来源：http://qt.lnxyls.cn

================================================================================
来源：http://ec.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://gf.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://ah.szsharing.cn

================================================================================
来源：http://pz.muxihuayi.cn

【收录内容】
来源：http://mj.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ux.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jy.bjjhwx.cn

SQL · Bash · C · C++
来源：http://jd.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xf.hahajie.cn

【使用说明】
来源：http://ib.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dm.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ft.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://at.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wh.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mc.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xw.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ha.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rc.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://is.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ni.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kc.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ks.jctech888.com.cn

【文件统计】
来源：http://gr.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ha.colortex.cn

--------------------------------------------------------------------------------
来源：http://lp.yuexingan06.cn

目  录
来源：http://vr.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ne.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ah.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sq.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ya.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ba.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ye.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sz.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dr.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://en.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sg.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ek.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kf.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lo.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hs.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ha.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qa.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gi.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mu.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://df.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qk.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ep.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uy.lnxyls.cn

================================================================================
来源：http://jt.hnjuh.cn

A. 基础语法与类型
来源：http://he.shtwfgs.cn

================================================================================
来源：http://jf.hnjuh.cn

[A01] Hello World
来源：http://gz.nszjky.cn

Py:   print("Hello, World!")
来源：http://cr.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://cy.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://qy.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oh.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://ef.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://no.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://hd.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sp.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://ds.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fe.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://im.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nz.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ib.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://cb.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://qa.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://bk.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ka.chemitech.net.cn

[A03] 常量定义
来源：http://xk.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cm.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://hv.szsharing.cn

JS:   const PI = 3.14159;
来源：http://mb.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://bc.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://vh.shxzukj.cn

Go:   const PI = 3.14159
来源：http://ov.nicolike.cn

Ruby: PI = 3.14159
来源：http://ck.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://ie.9csxet.cn

[A04] 判断变量类型
来源：http://wf.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ig.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tv.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dk.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://eg.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://il.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ds.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ys.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://mj.wgjwhj.cn

[A05] 整数除法与取模
来源：http://cj.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kq.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fs.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ke.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iz.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://qa.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://yy.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://yt.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://uo.shtwfgs.cn

[A06] 字符串转数字
来源：http://kz.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://gh.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hy.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ws.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ys.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ct.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://av.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://il.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iw.huixiangedu.cn

[A07] 数字转字符串
来源：http://ro.haigaiapp.cn

Py:   str(42)
来源：http://ym.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://sd.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://yy.huixiangedu.cn

TS:   String(42)
来源：http://hl.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yk.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://gw.yuexingan06.cn

Ruby: 42.to_s
来源：http://wp.szxytkj.cn

C#:   42.ToString()
来源：http://do.panjiajie.cn

[A08] 取整与四舍五入
来源：http://qe.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jp.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bq.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ki.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xq.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yr.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ho.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ej.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jk.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://qh.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lq.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ev.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yr.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pr.bjjhwx.cn


<!-- 参考信息 -->