代发 wailian999

[U53] PHP：空合并运算符
来源：http://hf.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://vb.521024.cn

[U54] PHP：空安全调用
来源：http://wd.asd995.cn

$obj?->method()
来源：http://il.szsharing.cn

[U55] PHP：match 表达式
来源：http://ns.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fh.shtwfgs.cn

[U56] PHP：命名参数
来源：http://gu.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://cl.colortex.cn

[U57] PHP：字符串插值
来源：http://yz.haigaiapp.cn

"值: {$a}"
来源：http://cv.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://wq.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lg.9csxet.cn

[U59] PHP：自定义排序
来源：http://ss.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jo.colortex.cn

[U60] PHP：JSON 编解码
来源：http://vi.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hj.shxzskj.cn

[U61] PHP：正则
来源：http://ew.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fq.huixiangedu.cn

[U62] PHP：日期对象
来源：http://bp.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qx.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://xf.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://au.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://wd.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://wr.hnjuh.cn

[U65] PHP：会话
来源：http://zd.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rc.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://ng.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bd.szsharing.cn

[U67] PHP：处理文件上传
来源：http://gh.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xs.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://ig.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ah.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://wg.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wa.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://vs.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qf.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://bu.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://po.gzmigu.cn

[U72] PHP：写错误日志
来源：http://zm.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://or.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://wm.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://gz.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://wd.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://sj.szsharing.cn

[U75] PHP：依赖注入
来源：http://it.shtwfgs.cn

composer require psr/container
来源：http://ed.newstarts.cn

[U76] PHP：简单路由
来源：http://ux.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xy.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://zz.hahajie.cn

composer require twig/twig
来源：http://cv.szsharing.cn

[U78] PHP：单元测试
来源：http://cx.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://xj.nszjky.cn

[U79] PHP：静态分析
来源：http://bl.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://td.colortex.cn

[U80] PHP：代码规范修复
来源：http://dz.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ym.hnjuh.cn

[U81] JS：初始化项目
来源：http://jp.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://at.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://fw.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rp.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://eu.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vd.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://pa.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wb.9csxet.cn

[U85] JS：可选链
来源：http://wa.wgjwhj.cn

a?.b?.c
来源：http://md.chemitech.net.cn

[U86] JS：空值合并
来源：http://sw.hahajie.cn

a ?? b
来源：http://ry.szxytkj.cn

[U87] JS：解构默认值
来源：http://ap.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://un.colortex.cn

[U88] JS：对象展开合并
来源：http://ba.nicolike.cn

{ ...a, ...b }
来源：http://cn.chemitech.net.cn

[U89] JS：数组去重
来源：http://iq.chemitech.net.cn

[...new Set(arr)]
来源：http://ar.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://yr.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://cc.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://pn.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ai.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://hu.szxytkj.cn

structuredClone(obj)
来源：http://mh.huixiangedu.cn

[U93] JS：模板字符串
来源：http://zo.9csxet.cn

`共 ${n} 条`
来源：http://ej.shxzskj.cn

[U94] JS：箭头函数
来源：http://za.jianghongdianzi.cn

const double = x => x * 2;
来源：http://oy.hnjuh.cn

[U95] JS：Promise 包装
来源：http://vb.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://bn.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://zs.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://np.asd995.cn

[U97] JS：并发请求
来源：http://nz.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dk.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://uf.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://de.szxytkj.cn

[U99] JS：事件监听
来源：http://kw.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://ec.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://ld.9csxet.cn

document.querySelector(".item")
来源：http://ke.chemitech.net.cn

[U101] JS：classList 操作
来源：http://xr.huixiangedu.cn

el.classList.toggle("active")
来源：http://do.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://hi.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fl.panjiajie.cn

[U103] JS：定时器
来源：http://yj.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qr.haigaiapp.cn

[U104] JS：防抖
来源：http://xu.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kb.nicolike.cn

[U105] JS：节流
来源：http://yk.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://se.shxzukj.cn

[U106] JS：日期格式化
来源：http://jg.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wh.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://km.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xx.wgjwhj.cn

[U108] JS：随机整数
来源：http://qm.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sv.haigaiapp.cn

[U109] JS：数组分组
来源：http://od.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://vq.gzmigu.cn

[U110] JS：数组分块
来源：http://qx.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uu.szsharing.cn

[U111] JS：对象转 Map
来源：http://eg.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://wl.haigaiapp.cn

[U112] JS：字符串补位
来源：http://cb.colortex.cn

"7".padStart(3, "0")
来源：http://iz.nszjky.cn

[U113] JS：正则替换全部
来源：http://qr.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://ja.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://ee.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wx.lnxyls.cn

[U115] JS：生成 UUID
来源：http://oi.jianghongdianzi.cn

crypto.randomUUID()
来源：http://zu.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://ql.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://yu.bjjhwx.cn

[U117] JS：单元测试
来源：http://vd.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://ld.shxzukj.cn

[U118] JS：开发服务器
来源：http://nk.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://is.hahajie.cn

[U119] JS：生产构建
来源：http://nc.yuexingan06.cn

npx vite build
来源：http://mx.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://no.asd995.cn

import.meta.env.VITE_API_URL
来源：http://by.szxytkj.cn

================================================================================
来源：http://jo.shtwfgs.cn

统计汇总
来源：http://tm.panjiajie.cn

================================================================================
来源：http://fw.bookmarksfly.cn

按语言统计（条）：
来源：http://go.shxzskj.cn

Python ......... 252
来源：http://ow.yuexingan06.cn

PHP ............ 252
来源：http://xx.shtwfgs.cn

JavaScript ..... 252
来源：http://ig.yuntaijiaju.cn

TypeScript ..... 212
来源：http://ia.hahajie.cn

Java ........... 212
来源：http://ke.jianghongdianzi.cn

Go ............. 212
来源：http://ms.bjjhwx.cn

Ruby ........... 212
来源：http://zj.colortex.cn

C# ............. 212
来源：http://bf.szxytkj.cn

C .............. 30
来源：http://ho.muxihuayi.cn

C++ ............ 30
来源：http://pq.hnjuh.cn

SQL ............ 90
来源：http://jk.hnjuh.cn

Bash ........... 80
来源：http://dk.huixinmuqiang.cn

Kotlin ......... 15
来源：http://yx.huanxung.cn

Swift .......... 15
来源：http://vq.jctech888.com.cn

Lua ............ 10
来源：http://zi.nicolike.cn

Perl ........... 10
来源：http://bd.nicolike.cn

Scala .......... 10
来源：http://gk.huanxung.cn

------------------------------------
来源：http://ta.szsharing.cn

合计 ........... 2106 条
来源：http://za.bookmarksfly.cn

按章节统计：
来源：http://en.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hy.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sp.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zv.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bm.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fo.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ea.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nk.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bt.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ox.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vf.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yv.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ln.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wy.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cg.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ck.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mj.9csxet.cn

Q SQL 专题                              90
来源：http://fy.asd995.cn

R Bash 专题                             80
来源：http://yp.huixiangedu.cn

S C / C++ 专题                          60
来源：http://rm.bjjhwx.cn

T 其他语言补充                          60
来源：http://qk.asd995.cn

U 高频实用片段                         120
来源：http://zt.nszjky.cn

------------------------------------
来源：http://xs.nszjky.cn

合计                                  2106 条
来源：http://cr.szsharing.cn

--------------------------------------------------------------------------------
来源：http://io.chemitech.net.cn

使用提醒
来源：http://da.nszjky.cn

--------------------------------------------------------------------------------
来源：http://op.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gm.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jt.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cn.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ay.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zp.hahajie.cn

—— 文件结束 ——
来源：http://xa.huanxung.cn

================================================================================
来源：http://fp.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://wx.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://al.hnjuh.cn

================================================================================
来源：http://hn.huixiangedu.cn

【收录内容】
来源：http://en.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ot.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kt.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://jn.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bk.nszjky.cn

【使用说明】
来源：http://tz.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ui.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wn.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kn.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ik.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jw.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ul.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oy.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zd.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qq.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gl.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sv.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ms.szsharing.cn

【文件统计】
来源：http://ka.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vh.521024.cn

--------------------------------------------------------------------------------
来源：http://ur.szsharing.cn

目  录
来源：http://on.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ce.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://og.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ow.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sd.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cf.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yv.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xs.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mt.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dd.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ur.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eq.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://by.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ji.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nf.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ji.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bh.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qv.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ee.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ya.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vt.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ia.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kl.huixiangedu.cn

================================================================================
来源：http://gs.muxihuayi.cn

A. 基础语法与类型
来源：http://fb.9csxet.cn

================================================================================
来源：http://uz.wgjwhj.cn

[A01] Hello World
来源：http://op.521024.cn

Py:   print("Hello, World!")
来源：http://qi.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://tp.colortex.cn

JS:   console.log("Hello, World!");
来源：http://km.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bu.521024.cn

Java: System.out.println("Hello, World!");
来源：http://ez.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://de.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://bs.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pn.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://nd.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://or.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ae.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sv.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ks.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://yo.521024.cn

Go:   name := "Alex"; age := 20
来源：http://zi.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://tx.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ml.nszjky.cn

[A03] 常量定义
来源：http://ns.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ix.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://yg.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://dm.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://fs.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://ga.nszjky.cn

Go:   const PI = 3.14159
来源：http://cl.shxzskj.cn

Ruby: PI = 3.14159
来源：http://ks.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://nt.yuexingan06.cn

[A04] 判断变量类型
来源：http://ai.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bh.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rm.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fc.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://gh.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mk.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://eu.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://he.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://dg.asd995.cn

[A05] 整数除法与取模
来源：http://os.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ij.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oo.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ux.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://js.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://gc.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://xl.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://kv.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://wp.yuexingan06.cn

[A06] 字符串转数字
来源：http://lj.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://kg.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://za.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hy.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xf.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://by.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ro.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wt.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zq.hnjuh.cn

[A07] 数字转字符串
来源：http://tf.yuexingan06.cn

Py:   str(42)
来源：http://ov.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://al.jctech888.com.cn


<!-- 参考信息 -->