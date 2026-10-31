代发 wailian999

[U51] PHP：数组解构
来源：http://qw.nszjky.cn

[$a, $b] = $arr;
来源：http://fa.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://qh.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://bd.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://ky.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://aq.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://ot.jianghongdianzi.cn

$obj?->method()
来源：http://vz.newstarts.cn

[U55] PHP：match 表达式
来源：http://vn.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://in.jctech888.com.cn

[U56] PHP：命名参数
来源：http://iz.hahajie.cn

f(a: 1, b: 2)
来源：http://ua.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://pj.shtwfgs.cn

"值: {$a}"
来源：http://xg.colortex.cn

[U58] PHP：数组三件套
来源：http://jb.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mh.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://qi.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mx.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://ih.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kz.521024.cn

[U61] PHP：正则
来源：http://ab.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mb.szsharing.cn

[U62] PHP：日期对象
来源：http://pj.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xc.9csxet.cn

[U63] PHP：文件读写
来源：http://wh.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yp.asd995.cn

[U64] PHP：目录遍历
来源：http://uc.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://sd.hnjuh.cn

[U65] PHP：会话
来源：http://js.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cq.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://cu.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pm.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://tm.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tm.521024.cn

[U68] PHP：PDO 连接
来源：http://ef.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wq.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://ku.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ng.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://rx.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fd.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://pv.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://tx.szsharing.cn

[U72] PHP：写错误日志
来源：http://xw.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://io.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://ob.asd995.cn

parse_ini_file("config.ini", true)
来源：http://mr.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://ub.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://xd.shxzukj.cn

[U75] PHP：依赖注入
来源：http://iw.hnjuh.cn

composer require psr/container
来源：http://sb.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://sk.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uh.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://yb.huanxung.cn

composer require twig/twig
来源：http://pz.jctech888.com.cn

[U78] PHP：单元测试
来源：http://lv.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://ip.szsharing.cn

[U79] PHP：静态分析
来源：http://qw.asd995.cn

composer require --dev phpstan/phpstan
来源：http://we.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://qb.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qi.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://ze.yuexingan06.cn

npm init -y;  npm i express
来源：http://fn.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://lu.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dm.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://qz.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qc.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://wb.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pg.jianghongdianzi.cn

[U85] JS：可选链
来源：http://df.haigaiapp.cn

a?.b?.c
来源：http://ve.hahajie.cn

[U86] JS：空值合并
来源：http://cy.hnjuh.cn

a ?? b
来源：http://al.haigaiapp.cn

[U87] JS：解构默认值
来源：http://xt.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://dy.521024.cn

[U88] JS：对象展开合并
来源：http://xq.chemitech.net.cn

{ ...a, ...b }
来源：http://oo.nszjky.cn

[U89] JS：数组去重
来源：http://lq.huixinmuqiang.cn

[...new Set(arr)]
来源：http://yu.lnxyls.cn

[U90] JS：数字数组排序
来源：http://ur.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://cr.colortex.cn

[U91] JS：对象键值遍历
来源：http://wu.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wx.szsharing.cn

[U92] JS：深拷贝
来源：http://nb.yuexingan06.cn

structuredClone(obj)
来源：http://sh.colortex.cn

[U93] JS：模板字符串
来源：http://gd.huixiangedu.cn

`共 ${n} 条`
来源：http://jc.shxzskj.cn

[U94] JS：箭头函数
来源：http://cg.jianghongdianzi.cn

const double = x => x * 2;
来源：http://js.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://ue.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://oo.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://mr.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jl.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://oa.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ed.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://ae.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ow.yuexingan06.cn

[U99] JS：事件监听
来源：http://ii.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://jh.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://kd.haigaiapp.cn

document.querySelector(".item")
来源：http://qv.muxihuayi.cn

[U101] JS：classList 操作
来源：http://pk.nszjky.cn

el.classList.toggle("active")
来源：http://oz.bjjhwx.cn

[U102] JS：本地存储
来源：http://qf.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ay.asd995.cn

[U103] JS：定时器
来源：http://zv.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ty.shxzskj.cn

[U104] JS：防抖
来源：http://yq.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://au.yuexingan06.cn

[U105] JS：节流
来源：http://lt.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dp.yuexingan06.cn

[U106] JS：日期格式化
来源：http://on.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pc.bjjhwx.cn

[U107] JS：数字千分位
来源：http://up.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gi.huanxung.cn

[U108] JS：随机整数
来源：http://xv.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dd.nszjky.cn

[U109] JS：数组分组
来源：http://rf.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://qj.bookmarksfly.cn

[U110] JS：数组分块
来源：http://wr.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bt.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://ih.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://zf.panjiajie.cn

[U112] JS：字符串补位
来源：http://qt.huanxung.cn

"7".padStart(3, "0")
来源：http://fj.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://aj.szsharing.cn

s.replaceAll("a", "b")
来源：http://le.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://iw.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pt.colortex.cn

[U115] JS：生成 UUID
来源：http://wc.newstarts.cn

crypto.randomUUID()
来源：http://cl.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://yp.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://sn.bookmarksfly.cn

[U117] JS：单元测试
来源：http://lx.521024.cn

npm i -D vitest;  npx vitest
来源：http://bu.nszjky.cn

[U118] JS：开发服务器
来源：http://fn.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://ld.szsharing.cn

[U119] JS：生产构建
来源：http://qi.nicolike.cn

npx vite build
来源：http://rz.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://wv.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://tx.wgjwhj.cn

================================================================================
来源：http://qh.yuexingan06.cn

统计汇总
来源：http://oq.colortex.cn

================================================================================
来源：http://cf.asd995.cn

按语言统计（条）：
来源：http://ez.jianghongdianzi.cn

Python ......... 252
来源：http://hz.shxzukj.cn

PHP ............ 252
来源：http://rp.newstarts.cn

JavaScript ..... 252
来源：http://zs.huanxung.cn

TypeScript ..... 212
来源：http://mh.bjjhwx.cn

Java ........... 212
来源：http://iu.nicolike.cn

Go ............. 212
来源：http://hf.hahajie.cn

Ruby ........... 212
来源：http://cw.bookmarksfly.cn

C# ............. 212
来源：http://wp.szsharing.cn

C .............. 30
来源：http://xu.nszjky.cn

C++ ............ 30
来源：http://cw.szxytkj.cn

SQL ............ 90
来源：http://iy.hahajie.cn

Bash ........... 80
来源：http://qx.nicolike.cn

Kotlin ......... 15
来源：http://mr.yuexingan06.cn

Swift .......... 15
来源：http://nl.shxzukj.cn

Lua ............ 10
来源：http://ci.colortex.cn

Perl ........... 10
来源：http://zn.muxihuayi.cn

Scala .......... 10
来源：http://zc.nicolike.cn

------------------------------------
来源：http://tq.muxihuayi.cn

合计 ........... 2106 条
来源：http://up.yuntaijiaju.cn

按章节统计：
来源：http://ye.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rk.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://me.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cg.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pj.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pu.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://de.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rq.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hc.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jb.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cf.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fa.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nn.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://za.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wd.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dh.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ez.9csxet.cn

Q SQL 专题                              90
来源：http://qt.newstarts.cn

R Bash 专题                             80
来源：http://wo.szxytkj.cn

S C / C++ 专题                          60
来源：http://qi.yuexingan06.cn

T 其他语言补充                          60
来源：http://uc.521024.cn

U 高频实用片段                         120
来源：http://hk.asd995.cn

------------------------------------
来源：http://in.yuexingan06.cn

合计                                  2106 条
来源：http://hr.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://rj.nszjky.cn

使用提醒
来源：http://fm.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://nj.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://na.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hi.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://er.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pb.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tj.huixiangedu.cn

—— 文件结束 ——
来源：http://kf.lnxyls.cn

================================================================================
来源：http://yh.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://up.hahajie.cn

Common Programming Examples Cheat Book
来源：http://vl.chemitech.net.cn

================================================================================
来源：http://ap.szxytkj.cn

【收录内容】
来源：http://zl.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://di.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ml.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://oe.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hb.lnxyls.cn

【使用说明】
来源：http://cb.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yx.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ym.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ad.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sr.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ef.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pd.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pz.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ev.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cj.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ri.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rn.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zn.szsharing.cn

【文件统计】
来源：http://hj.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kv.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ew.gzmigu.cn

目  录
来源：http://sp.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://wq.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ne.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qb.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vx.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pj.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://da.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wx.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nf.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://er.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lv.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qo.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sf.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://io.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://su.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mg.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aq.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://na.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ba.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nz.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lg.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lz.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xs.yuntaijiaju.cn

================================================================================
来源：http://wo.szxytkj.cn

A. 基础语法与类型
来源：http://tb.yuexingan06.cn

================================================================================
来源：http://uq.9csxet.cn

[A01] Hello World
来源：http://sh.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://cp.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://jq.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://yj.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cj.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://em.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://gr.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://eg.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mz.colortex.cn

[A02] 变量声明与赋值
来源：http://sz.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jc.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kb.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lk.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tm.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://lb.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://cc.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://gi.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nh.colortex.cn

[A03] 常量定义
来源：http://pg.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bx.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://mr.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://xm.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://ch.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://op.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://da.muxihuayi.cn

Ruby: PI = 3.14159
来源：http://id.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://ed.haigaiapp.cn

[A04] 判断变量类型
来源：http://qm.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ty.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ek.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://au.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://am.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bd.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fz.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mr.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://lo.shxzukj.cn

[A05] 整数除法与取模
来源：http://if.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ax.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gk.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://es.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gm.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://be.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://yq.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://fi.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://rt.hahajie.cn

[A06] 字符串转数字
来源：http://sg.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://ov.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://py.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dw.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kv.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ah.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hl.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dc.muxihuayi.cn


<!-- 参考信息 -->