代发 wailian999

[U57] PHP：字符串插值
来源：http://gn.colortex.cn

"值: {$a}"
来源：http://ro.panjiajie.cn

[U58] PHP：数组三件套
来源：http://fp.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vj.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://uo.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yp.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://wx.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lm.panjiajie.cn

[U61] PHP：正则
来源：http://qz.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ja.szsharing.cn

[U62] PHP：日期对象
来源：http://qm.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rk.szsharing.cn

[U63] PHP：文件读写
来源：http://lu.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sn.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://fl.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://ii.nszjky.cn

[U65] PHP：会话
来源：http://ag.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sh.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://ku.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zj.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://sq.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mt.newstarts.cn

[U68] PHP：PDO 连接
来源：http://ko.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ib.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://wq.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xf.newstarts.cn

[U70] PHP：PDO 事务
来源：http://eq.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rl.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://qy.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://ts.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://hw.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://cb.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://tq.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://zv.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://uq.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://sh.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://lq.newstarts.cn

composer require psr/container
来源：http://zl.asd995.cn

[U76] PHP：简单路由
来源：http://vo.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jp.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://is.gzmigu.cn

composer require twig/twig
来源：http://wt.szxytkj.cn

[U78] PHP：单元测试
来源：http://xj.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://ca.chemitech.net.cn

[U79] PHP：静态分析
来源：http://lm.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://db.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://qf.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://al.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://vk.shxzskj.cn

npm init -y;  npm i express
来源：http://gz.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://ph.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ef.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://yu.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ej.colortex.cn

[U84] JS：CommonJS 写法
来源：http://lb.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ze.chemitech.net.cn

[U85] JS：可选链
来源：http://we.yuexingan06.cn

a?.b?.c
来源：http://md.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://sa.wgjwhj.cn

a ?? b
来源：http://bh.szsharing.cn

[U87] JS：解构默认值
来源：http://cj.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://ij.shxzukj.cn

[U88] JS：对象展开合并
来源：http://fv.bjjhwx.cn

{ ...a, ...b }
来源：http://ug.szxytkj.cn

[U89] JS：数组去重
来源：http://eu.hahajie.cn

[...new Set(arr)]
来源：http://sb.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://ys.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://uq.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://xa.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rb.haigaiapp.cn

[U92] JS：深拷贝
来源：http://xk.colortex.cn

structuredClone(obj)
来源：http://ph.yuexingan06.cn

[U93] JS：模板字符串
来源：http://xq.szxytkj.cn

`共 ${n} 条`
来源：http://yp.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://og.huixinmuqiang.cn

const double = x => x * 2;
来源：http://gw.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://lk.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://ha.nszjky.cn

[U96] JS：async/await 与异常
来源：http://pg.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vn.shxzskj.cn

[U97] JS：并发请求
来源：http://lm.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pc.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://wf.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ci.asd995.cn

[U99] JS：事件监听
来源：http://ei.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://cr.shxzukj.cn

[U100] JS：DOM 查询
来源：http://cy.szsharing.cn

document.querySelector(".item")
来源：http://cn.hnjuh.cn

[U101] JS：classList 操作
来源：http://ur.muxihuayi.cn

el.classList.toggle("active")
来源：http://hq.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://yn.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fh.gzmigu.cn

[U103] JS：定时器
来源：http://tb.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ht.bookmarksfly.cn

[U104] JS：防抖
来源：http://ru.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hu.yuexingan06.cn

[U105] JS：节流
来源：http://vj.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rs.newstarts.cn

[U106] JS：日期格式化
来源：http://aq.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bd.hahajie.cn

[U107] JS：数字千分位
来源：http://ik.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ar.huanxung.cn

[U108] JS：随机整数
来源：http://lp.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ye.asd995.cn

[U109] JS：数组分组
来源：http://zz.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://lt.nszjky.cn

[U110] JS：数组分块
来源：http://wd.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zx.shxzskj.cn

[U111] JS：对象转 Map
来源：http://pi.shxzukj.cn

new Map(Object.entries(obj))
来源：http://it.yuexingan06.cn

[U112] JS：字符串补位
来源：http://fv.gzmigu.cn

"7".padStart(3, "0")
来源：http://yl.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://wk.shxzskj.cn

s.replaceAll("a", "b")
来源：http://uv.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://ip.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hc.nszjky.cn

[U115] JS：生成 UUID
来源：http://we.huixinmuqiang.cn

crypto.randomUUID()
来源：http://hk.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://kh.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://gm.gzmigu.cn

[U117] JS：单元测试
来源：http://fg.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://cv.muxihuayi.cn

[U118] JS：开发服务器
来源：http://mp.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://ub.newstarts.cn

[U119] JS：生产构建
来源：http://dn.jctech888.com.cn

npx vite build
来源：http://pa.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://dq.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://uw.szsharing.cn

================================================================================
来源：http://nf.lnxyls.cn

统计汇总
来源：http://oy.lnxyls.cn

================================================================================
来源：http://ah.asd995.cn

按语言统计（条）：
来源：http://cw.szxytkj.cn

Python ......... 252
来源：http://xr.lnxyls.cn

PHP ............ 252
来源：http://yh.521024.cn

JavaScript ..... 252
来源：http://jd.panjiajie.cn

TypeScript ..... 212
来源：http://dj.nszjky.cn

Java ........... 212
来源：http://fx.bookmarksfly.cn

Go ............. 212
来源：http://ip.shxzukj.cn

Ruby ........... 212
来源：http://oo.shtwfgs.cn

C# ............. 212
来源：http://jn.huixinmuqiang.cn

C .............. 30
来源：http://ja.gzmigu.cn

C++ ............ 30
来源：http://pm.hnjuh.cn

SQL ............ 90
来源：http://eb.9csxet.cn

Bash ........... 80
来源：http://ul.huixiangedu.cn

Kotlin ......... 15
来源：http://eg.panjiajie.cn

Swift .......... 15
来源：http://vs.yuexingan06.cn

Lua ............ 10
来源：http://mv.hnjuh.cn

Perl ........... 10
来源：http://dw.huixiangedu.cn

Scala .......... 10
来源：http://hf.newstarts.cn

------------------------------------
来源：http://ac.shxzukj.cn

合计 ........... 2106 条
来源：http://td.huanxung.cn

按章节统计：
来源：http://ku.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fe.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sr.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tv.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ty.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hx.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fd.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kh.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nj.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xs.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jx.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fw.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zc.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ye.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kl.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fo.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ag.muxihuayi.cn

Q SQL 专题                              90
来源：http://nt.wgjwhj.cn

R Bash 专题                             80
来源：http://vi.wgjwhj.cn

S C / C++ 专题                          60
来源：http://cz.bjjhwx.cn

T 其他语言补充                          60
来源：http://br.bookmarksfly.cn

U 高频实用片段                         120
来源：http://qn.wgjwhj.cn

------------------------------------
来源：http://yn.yuexingan06.cn

合计                                  2106 条
来源：http://dw.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://jk.huanxung.cn

使用提醒
来源：http://ze.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://eo.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tj.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vt.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rd.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qn.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fj.shtwfgs.cn

—— 文件结束 ——
来源：http://ai.huixinmuqiang.cn

================================================================================
来源：http://dk.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://eg.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://xa.jctech888.com.cn

================================================================================
来源：http://yx.panjiajie.cn

【收录内容】
来源：http://ig.shxzukj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fa.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vx.lnxyls.cn

SQL · Bash · C · C++
来源：http://cd.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mu.muxihuayi.cn

【使用说明】
来源：http://ut.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vy.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yp.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ws.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pj.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mn.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tj.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bc.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mr.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vr.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ov.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zy.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kb.bjjhwx.cn

【文件统计】
来源：http://qf.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xt.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://zl.nszjky.cn

目  录
来源：http://hs.szsharing.cn

--------------------------------------------------------------------------------
来源：http://aj.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ep.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qw.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yq.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ni.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://un.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xu.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wv.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fu.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qe.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jg.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xw.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://em.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cd.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bz.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zm.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mx.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jb.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lx.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sf.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fd.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ym.huanxung.cn

================================================================================
来源：http://dg.szxytkj.cn

A. 基础语法与类型
来源：http://of.muxihuayi.cn

================================================================================
来源：http://bt.colortex.cn

[A01] Hello World
来源：http://sy.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://yh.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://ar.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://qu.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lb.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://gc.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://in.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://iw.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ri.hahajie.cn

[A02] 变量声明与赋值
来源：http://vw.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bc.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hw.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://am.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lr.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://hw.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://bl.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://pz.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nz.colortex.cn

[A03] 常量定义
来源：http://xk.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bb.colortex.cn

PHP:  const PI = 3.14159;
来源：http://xa.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://qz.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://pw.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://ro.gzmigu.cn

Go:   const PI = 3.14159
来源：http://lh.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://ws.colortex.cn

C#:   const double PI = 3.14159;
来源：http://iv.9csxet.cn

[A04] 判断变量类型
来源：http://vr.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ug.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jz.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xs.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://xp.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://an.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vu.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hy.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://mb.newstarts.cn

[A05] 整数除法与取模
来源：http://zz.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lj.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://po.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jd.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://or.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://lo.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://hm.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://dj.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://ru.521024.cn

[A06] 字符串转数字
来源：http://yk.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://nz.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://id.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fm.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zw.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gs.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pn.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ei.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fj.bookmarksfly.cn

[A07] 数字转字符串
来源：http://ku.haigaiapp.cn

Py:   str(42)
来源：http://fh.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://ta.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://pk.szsharing.cn

TS:   String(42)
来源：http://pn.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jr.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://no.shxzukj.cn

Ruby: 42.to_s
来源：http://mp.wgjwhj.cn

C#:   42.ToString()
来源：http://im.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://ab.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ek.szsharing.cn


<!-- 参考信息 -->