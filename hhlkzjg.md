代发 wailian999

[U57] PHP：字符串插值
来源：http://gw.huanxung.cn

"值: {$a}"
来源：http://dq.hahajie.cn

[U58] PHP：数组三件套
来源：http://bo.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jg.gzmigu.cn

[U59] PHP：自定义排序
来源：http://bb.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dl.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://rt.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uu.jianghongdianzi.cn

[U61] PHP：正则
来源：http://mi.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zh.newstarts.cn

[U62] PHP：日期对象
来源：http://lt.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://de.yuexingan06.cn

[U63] PHP：文件读写
来源：http://wv.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yk.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://eg.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://bl.huixiangedu.cn

[U65] PHP：会话
来源：http://gb.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fs.colortex.cn

[U66] PHP：设置 Cookie
来源：http://ps.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ki.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://hu.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zj.newstarts.cn

[U68] PHP：PDO 连接
来源：http://no.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jl.asd995.cn

[U69] PHP：PDO 预处理
来源：http://zn.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xv.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://im.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mk.shxzskj.cn

[U71] PHP：抛出异常
来源：http://yb.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://hy.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://tr.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://ae.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://fz.521024.cn

parse_ini_file("config.ini", true)
来源：http://fe.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://oa.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://ip.szsharing.cn

[U75] PHP：依赖注入
来源：http://go.colortex.cn

composer require psr/container
来源：http://he.huanxung.cn

[U76] PHP：简单路由
来源：http://rk.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yy.lnxyls.cn

[U77] PHP：模板渲染
来源：http://jn.shxzukj.cn

composer require twig/twig
来源：http://dc.wgjwhj.cn

[U78] PHP：单元测试
来源：http://lk.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://az.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://fn.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://ww.szsharing.cn

[U80] PHP：代码规范修复
来源：http://fn.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ej.hahajie.cn

[U81] JS：初始化项目
来源：http://yv.hahajie.cn

npm init -y;  npm i express
来源：http://ll.nicolike.cn

[U82] JS：package.json 脚本
来源：http://tu.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nf.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://an.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vq.asd995.cn

[U84] JS：CommonJS 写法
来源：http://ji.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uj.shxzukj.cn

[U85] JS：可选链
来源：http://ry.hnjuh.cn

a?.b?.c
来源：http://oc.lnxyls.cn

[U86] JS：空值合并
来源：http://fc.asd995.cn

a ?? b
来源：http://va.huanxung.cn

[U87] JS：解构默认值
来源：http://lq.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://oh.hahajie.cn

[U88] JS：对象展开合并
来源：http://op.bjjhwx.cn

{ ...a, ...b }
来源：http://vy.jctech888.com.cn

[U89] JS：数组去重
来源：http://xs.lnxyls.cn

[...new Set(arr)]
来源：http://ot.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://im.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://gd.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://dg.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zs.shxzukj.cn

[U92] JS：深拷贝
来源：http://qq.shxzukj.cn

structuredClone(obj)
来源：http://pd.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://ec.521024.cn

`共 ${n} 条`
来源：http://dm.colortex.cn

[U94] JS：箭头函数
来源：http://on.bookmarksfly.cn

const double = x => x * 2;
来源：http://ey.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://ko.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://xb.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://fo.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cn.hahajie.cn

[U97] JS：并发请求
来源：http://db.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mc.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://vd.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hv.hnjuh.cn

[U99] JS：事件监听
来源：http://zf.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://ve.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://ey.nicolike.cn

document.querySelector(".item")
来源：http://au.newstarts.cn

[U101] JS：classList 操作
来源：http://po.yuexingan06.cn

el.classList.toggle("active")
来源：http://vg.shxzskj.cn

[U102] JS：本地存储
来源：http://ic.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://eq.colortex.cn

[U103] JS：定时器
来源：http://tx.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oe.haigaiapp.cn

[U104] JS：防抖
来源：http://ya.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oy.lnxyls.cn

[U105] JS：节流
来源：http://jp.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ei.9csxet.cn

[U106] JS：日期格式化
来源：http://yp.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tv.nicolike.cn

[U107] JS：数字千分位
来源：http://ug.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ii.huanxung.cn

[U108] JS：随机整数
来源：http://vk.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cn.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://wx.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://vk.nszjky.cn

[U110] JS：数组分块
来源：http://oo.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hq.panjiajie.cn

[U111] JS：对象转 Map
来源：http://nq.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://mk.huanxung.cn

[U112] JS：字符串补位
来源：http://xd.szsharing.cn

"7".padStart(3, "0")
来源：http://cy.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://vw.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://ap.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://uj.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ew.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://zl.521024.cn

crypto.randomUUID()
来源：http://jn.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://uh.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://dr.haigaiapp.cn

[U117] JS：单元测试
来源：http://cl.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://aj.nszjky.cn

[U118] JS：开发服务器
来源：http://qs.shxzukj.cn

npm i -D vite;  npx vite
来源：http://kk.gzmigu.cn

[U119] JS：生产构建
来源：http://hk.yuntaijiaju.cn

npx vite build
来源：http://qa.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://jh.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://jt.jctech888.com.cn

================================================================================
来源：http://ft.panjiajie.cn

统计汇总
来源：http://hw.gzmigu.cn

================================================================================
来源：http://yl.bjjhwx.cn

按语言统计（条）：
来源：http://wj.hnjuh.cn

Python ......... 252
来源：http://ps.hnjuh.cn

PHP ............ 252
来源：http://sg.colortex.cn

JavaScript ..... 252
来源：http://fe.lnxyls.cn

TypeScript ..... 212
来源：http://zy.shxzukj.cn

Java ........... 212
来源：http://ht.521024.cn

Go ............. 212
来源：http://xv.shxzskj.cn

Ruby ........... 212
来源：http://lu.9csxet.cn

C# ............. 212
来源：http://kz.chemitech.net.cn

C .............. 30
来源：http://fx.yuntaijiaju.cn

C++ ............ 30
来源：http://gw.9csxet.cn

SQL ............ 90
来源：http://wk.newstarts.cn

Bash ........... 80
来源：http://ae.haigaiapp.cn

Kotlin ......... 15
来源：http://rq.newstarts.cn

Swift .......... 15
来源：http://ch.huixiangedu.cn

Lua ............ 10
来源：http://xr.asd995.cn

Perl ........... 10
来源：http://lw.newstarts.cn

Scala .......... 10
来源：http://tk.9csxet.cn

------------------------------------
来源：http://jb.lnxyls.cn

合计 ........... 2106 条
来源：http://ys.nicolike.cn

按章节统计：
来源：http://gh.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ap.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wi.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rs.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vm.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ge.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://og.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xq.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://am.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bg.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ax.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nv.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jy.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://po.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cf.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zu.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ks.hnjuh.cn

Q SQL 专题                              90
来源：http://sy.wgjwhj.cn

R Bash 专题                             80
来源：http://nu.hnjuh.cn

S C / C++ 专题                          60
来源：http://zs.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://ru.nicolike.cn

U 高频实用片段                         120
来源：http://um.gzmigu.cn

------------------------------------
来源：http://nc.jianghongdianzi.cn

合计                                  2106 条
来源：http://sf.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://sw.shxzskj.cn

使用提醒
来源：http://nd.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://yb.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nk.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yy.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ay.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tw.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ob.shxzskj.cn

—— 文件结束 ——
来源：http://kv.jctech888.com.cn

================================================================================
来源：http://nf.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://xt.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://av.gzmigu.cn

================================================================================
来源：http://qj.wgjwhj.cn

【收录内容】
来源：http://ty.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://un.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qa.haigaiapp.cn

SQL · Bash · C · C++
来源：http://iv.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gc.jianghongdianzi.cn

【使用说明】
来源：http://gr.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fq.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wh.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ue.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mz.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sm.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eu.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sh.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sn.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://or.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kh.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hn.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oz.hnjuh.cn

【文件统计】
来源：http://ib.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://da.asd995.cn

--------------------------------------------------------------------------------
来源：http://ho.huixinmuqiang.cn

目  录
来源：http://gv.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://fa.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ik.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ht.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mf.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mq.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ne.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dk.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yg.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qc.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://na.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ni.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mb.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ty.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ol.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://na.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ax.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wz.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sz.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mz.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uu.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ph.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lg.colortex.cn

================================================================================
来源：http://af.shxzukj.cn

A. 基础语法与类型
来源：http://si.9csxet.cn

================================================================================
来源：http://qs.chemitech.net.cn

[A01] Hello World
来源：http://ir.shxzukj.cn

Py:   print("Hello, World!")
来源：http://jo.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://nk.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://bw.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ft.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://uv.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://uq.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://td.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kd.521024.cn

[A02] 变量声明与赋值
来源：http://xc.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ou.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gh.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qo.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cp.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://ev.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://xg.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://gt.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rr.szxytkj.cn

[A03] 常量定义
来源：http://do.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zd.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://jr.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://ui.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://ew.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://zv.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://ea.nicolike.cn

Ruby: PI = 3.14159
来源：http://wt.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://du.shxzukj.cn

[A04] 判断变量类型
来源：http://xo.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://is.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zy.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ho.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://sv.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bv.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://of.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://na.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://wt.asd995.cn

[A05] 整数除法与取模
来源：http://vd.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ra.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pl.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gp.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gf.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://tw.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://vb.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://qh.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://nv.gzmigu.cn

[A06] 字符串转数字
来源：http://zn.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://rc.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fo.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ki.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xq.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ys.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gz.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hg.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qy.yuexingan06.cn

[A07] 数字转字符串
来源：http://sq.colortex.cn

Py:   str(42)
来源：http://vb.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://cz.asd995.cn

JS:   String(42); (42).toString()
来源：http://cv.huixiangedu.cn

TS:   String(42)
来源：http://vf.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hh.asd995.cn

Go:   strconv.Itoa(42)
来源：http://fd.hnjuh.cn

Ruby: 42.to_s
来源：http://oy.colortex.cn

C#:   42.ToString()
来源：http://em.nicolike.cn

[A08] 取整与四舍五入
来源：http://tt.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jw.panjiajie.cn


<!-- 参考信息 -->