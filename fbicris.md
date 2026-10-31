代发 wailian999

[U57] PHP：字符串插值
来源：http://ea.jctech888.com.cn

"值: {$a}"
来源：http://zn.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://fa.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mn.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://yd.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jj.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://cg.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jh.panjiajie.cn

[U61] PHP：正则
来源：http://kr.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pd.shtwfgs.cn

[U62] PHP：日期对象
来源：http://av.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uu.hahajie.cn

[U63] PHP：文件读写
来源：http://du.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hy.gzmigu.cn

[U64] PHP：目录遍历
来源：http://ch.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://qi.shxzukj.cn

[U65] PHP：会话
来源：http://wo.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kb.asd995.cn

[U66] PHP：设置 Cookie
来源：http://ab.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qg.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://pg.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ou.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://gh.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oi.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://sz.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lp.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://fq.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tk.szsharing.cn

[U71] PHP：抛出异常
来源：http://so.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://el.asd995.cn

[U72] PHP：写错误日志
来源：http://bp.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://bz.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://fq.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://lg.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://ru.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://yv.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://eb.shtwfgs.cn

composer require psr/container
来源：http://cc.jctech888.com.cn

[U76] PHP：简单路由
来源：http://xj.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rl.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://tx.huanxung.cn

composer require twig/twig
来源：http://wf.colortex.cn

[U78] PHP：单元测试
来源：http://xe.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://dw.wgjwhj.cn

[U79] PHP：静态分析
来源：http://ox.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://oq.szsharing.cn

[U80] PHP：代码规范修复
来源：http://tj.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://me.wgjwhj.cn

[U81] JS：初始化项目
来源：http://vz.haigaiapp.cn

npm init -y;  npm i express
来源：http://qh.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://pw.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ww.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://op.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wc.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://ow.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tm.nszjky.cn

[U85] JS：可选链
来源：http://di.hahajie.cn

a?.b?.c
来源：http://vv.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://gw.521024.cn

a ?? b
来源：http://ba.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://gk.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://wi.szxytkj.cn

[U88] JS：对象展开合并
来源：http://hq.asd995.cn

{ ...a, ...b }
来源：http://ji.chemitech.net.cn

[U89] JS：数组去重
来源：http://kr.colortex.cn

[...new Set(arr)]
来源：http://xb.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://lp.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://lv.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://jn.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://co.jctech888.com.cn

[U92] JS：深拷贝
来源：http://th.wgjwhj.cn

structuredClone(obj)
来源：http://ls.colortex.cn

[U93] JS：模板字符串
来源：http://ah.shxzukj.cn

`共 ${n} 条`
来源：http://hv.chemitech.net.cn

[U94] JS：箭头函数
来源：http://ah.haigaiapp.cn

const double = x => x * 2;
来源：http://ak.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://bc.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://pg.9csxet.cn

[U96] JS：async/await 与异常
来源：http://gw.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ni.wgjwhj.cn

[U97] JS：并发请求
来源：http://tp.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://id.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://ai.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://im.panjiajie.cn

[U99] JS：事件监听
来源：http://ld.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://lk.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://us.bjjhwx.cn

document.querySelector(".item")
来源：http://ev.nicolike.cn

[U101] JS：classList 操作
来源：http://jx.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://jx.yuexingan06.cn

[U102] JS：本地存储
来源：http://lj.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sp.bookmarksfly.cn

[U103] JS：定时器
来源：http://lg.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ak.szsharing.cn

[U104] JS：防抖
来源：http://oe.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ml.521024.cn

[U105] JS：节流
来源：http://rf.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dk.jctech888.com.cn

[U106] JS：日期格式化
来源：http://zb.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lr.muxihuayi.cn

[U107] JS：数字千分位
来源：http://dw.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zx.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://xd.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ua.huanxung.cn

[U109] JS：数组分组
来源：http://xu.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://op.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://iq.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ka.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://pz.hahajie.cn

new Map(Object.entries(obj))
来源：http://mj.haigaiapp.cn

[U112] JS：字符串补位
来源：http://rr.hnjuh.cn

"7".padStart(3, "0")
来源：http://sq.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://jj.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://hj.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://lu.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://of.shxzukj.cn

[U115] JS：生成 UUID
来源：http://ys.9csxet.cn

crypto.randomUUID()
来源：http://sy.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://cn.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://pv.bjjhwx.cn

[U117] JS：单元测试
来源：http://uf.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://wv.szxytkj.cn

[U118] JS：开发服务器
来源：http://dm.hnjuh.cn

npm i -D vite;  npx vite
来源：http://vc.shxzskj.cn

[U119] JS：生产构建
来源：http://we.shxzskj.cn

npx vite build
来源：http://od.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://sr.521024.cn

import.meta.env.VITE_API_URL
来源：http://wy.szsharing.cn

================================================================================
来源：http://zg.haigaiapp.cn

统计汇总
来源：http://fq.521024.cn

================================================================================
来源：http://vp.wgjwhj.cn

按语言统计（条）：
来源：http://cp.shxzskj.cn

Python ......... 252
来源：http://wl.chemitech.net.cn

PHP ............ 252
来源：http://qc.chemitech.net.cn

JavaScript ..... 252
来源：http://ty.jianghongdianzi.cn

TypeScript ..... 212
来源：http://ag.jctech888.com.cn

Java ........... 212
来源：http://zr.huanxung.cn

Go ............. 212
来源：http://mc.yuntaijiaju.cn

Ruby ........... 212
来源：http://ib.9csxet.cn

C# ............. 212
来源：http://li.szsharing.cn

C .............. 30
来源：http://or.szsharing.cn

C++ ............ 30
来源：http://mg.chemitech.net.cn

SQL ............ 90
来源：http://fo.nicolike.cn

Bash ........... 80
来源：http://fd.bookmarksfly.cn

Kotlin ......... 15
来源：http://jw.shtwfgs.cn

Swift .......... 15
来源：http://gp.shtwfgs.cn

Lua ............ 10
来源：http://sl.colortex.cn

Perl ........... 10
来源：http://nb.szsharing.cn

Scala .......... 10
来源：http://og.huixinmuqiang.cn

------------------------------------
来源：http://je.wgjwhj.cn

合计 ........... 2106 条
来源：http://xa.gzmigu.cn

按章节统计：
来源：http://hi.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gq.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uo.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cv.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jp.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oy.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yz.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fg.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zh.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cf.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zw.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sk.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nf.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dr.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cb.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bq.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ur.gzmigu.cn

Q SQL 专题                              90
来源：http://oc.nszjky.cn

R Bash 专题                             80
来源：http://ck.9csxet.cn

S C / C++ 专题                          60
来源：http://ne.haigaiapp.cn

T 其他语言补充                          60
来源：http://sp.colortex.cn

U 高频实用片段                         120
来源：http://tn.huixiangedu.cn

------------------------------------
来源：http://zh.jianghongdianzi.cn

合计                                  2106 条
来源：http://vp.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://hx.newstarts.cn

使用提醒
来源：http://jy.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://kw.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cx.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bb.shxzskj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ka.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ab.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hq.szxytkj.cn

—— 文件结束 ——
来源：http://bb.hnjuh.cn

================================================================================
来源：http://cq.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://ap.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://fl.9csxet.cn

================================================================================
来源：http://ey.jianghongdianzi.cn

【收录内容】
来源：http://lv.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://np.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yq.yuexingan06.cn

SQL · Bash · C · C++
来源：http://ah.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ot.huanxung.cn

【使用说明】
来源：http://ih.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://al.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zk.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lz.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dv.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bm.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qm.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nz.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oy.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lm.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://om.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qy.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tp.haigaiapp.cn

【文件统计】
来源：http://gm.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://le.nicolike.cn

--------------------------------------------------------------------------------
来源：http://xx.jctech888.com.cn

目  录
来源：http://ka.huanxung.cn

--------------------------------------------------------------------------------
来源：http://om.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sb.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://je.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jj.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dk.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ac.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nh.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gk.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yu.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ja.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qi.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://np.hnjuh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hk.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oc.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jh.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rg.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://am.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cn.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cy.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bz.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hd.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fg.gzmigu.cn

================================================================================
来源：http://ey.muxihuayi.cn

A. 基础语法与类型
来源：http://du.huixinmuqiang.cn

================================================================================
来源：http://uf.yuexingan06.cn

[A01] Hello World
来源：http://mq.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://mh.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://wy.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://ts.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wl.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://xs.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://vj.asd995.cn

Ruby: puts "Hello, World!"
来源：http://yp.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wo.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://nu.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://su.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ar.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cg.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://js.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://bq.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://oh.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://ew.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xl.asd995.cn

[A03] 常量定义
来源：http://mi.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sk.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://eu.colortex.cn

JS:   const PI = 3.14159;
来源：http://nb.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://fa.asd995.cn

Java: static final double PI = 3.14159;
来源：http://nd.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://zi.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://ld.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://qj.szxytkj.cn

[A04] 判断变量类型
来源：http://wi.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ui.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yr.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vu.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://ak.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://in.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dd.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yp.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://df.bjjhwx.cn

[A05] 整数除法与取模
来源：http://dm.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ra.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mk.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rf.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://br.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://vv.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://iu.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://my.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://ou.wgjwhj.cn

[A06] 字符串转数字
来源：http://mq.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://hc.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ac.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xl.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lk.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vm.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ed.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://am.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uw.hnjuh.cn

[A07] 数字转字符串
来源：http://lr.hnjuh.cn

Py:   str(42)
来源：http://js.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://zs.nszjky.cn

JS:   String(42); (42).toString()
来源：http://qo.chemitech.net.cn

TS:   String(42)
来源：http://sy.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://et.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://ba.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://jc.huixinmuqiang.cn

C#:   42.ToString()
来源：http://bf.szsharing.cn

[A08] 取整与四舍五入
来源：http://ib.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lh.nicolike.cn


<!-- 参考信息 -->