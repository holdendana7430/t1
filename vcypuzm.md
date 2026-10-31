代发 wailian999

[U53] PHP：空合并运算符
来源：http://qq.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://et.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://xu.shtwfgs.cn

$obj?->method()
来源：http://lm.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://sh.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qy.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://dt.szxytkj.cn

f(a: 1, b: 2)
来源：http://ag.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://ru.chemitech.net.cn

"值: {$a}"
来源：http://bz.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://rj.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vr.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://iu.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://im.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://ns.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hh.jctech888.com.cn

[U61] PHP：正则
来源：http://ik.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gw.nicolike.cn

[U62] PHP：日期对象
来源：http://th.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ne.jctech888.com.cn

[U63] PHP：文件读写
来源：http://vl.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cm.hahajie.cn

[U64] PHP：目录遍历
来源：http://ie.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://zr.shtwfgs.cn

[U65] PHP：会话
来源：http://if.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rv.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://qx.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://au.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://vv.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qf.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://yh.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ut.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://re.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nz.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://ni.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wn.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://ja.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://ww.shxzskj.cn

[U72] PHP：写错误日志
来源：http://xk.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://ts.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://gp.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://mu.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://th.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://dr.newstarts.cn

[U75] PHP：依赖注入
来源：http://rv.gzmigu.cn

composer require psr/container
来源：http://yx.chemitech.net.cn

[U76] PHP：简单路由
来源：http://wk.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xq.panjiajie.cn

[U77] PHP：模板渲染
来源：http://ut.haigaiapp.cn

composer require twig/twig
来源：http://yv.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://zs.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://rf.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://hp.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://ez.nicolike.cn

[U80] PHP：代码规范修复
来源：http://ep.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zb.shtwfgs.cn

[U81] JS：初始化项目
来源：http://en.szsharing.cn

npm init -y;  npm i express
来源：http://yd.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://si.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yl.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://ax.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eq.521024.cn

[U84] JS：CommonJS 写法
来源：http://ya.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wg.9csxet.cn

[U85] JS：可选链
来源：http://lt.nicolike.cn

a?.b?.c
来源：http://jx.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://ho.colortex.cn

a ?? b
来源：http://wv.nicolike.cn

[U87] JS：解构默认值
来源：http://bm.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://za.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://es.panjiajie.cn

{ ...a, ...b }
来源：http://wq.huixiangedu.cn

[U89] JS：数组去重
来源：http://yr.newstarts.cn

[...new Set(arr)]
来源：http://ah.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://ri.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://xd.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://bs.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wl.521024.cn

[U92] JS：深拷贝
来源：http://mq.asd995.cn

structuredClone(obj)
来源：http://cg.9csxet.cn

[U93] JS：模板字符串
来源：http://wy.hnjuh.cn

`共 ${n} 条`
来源：http://so.wgjwhj.cn

[U94] JS：箭头函数
来源：http://ha.muxihuayi.cn

const double = x => x * 2;
来源：http://bl.lnxyls.cn

[U95] JS：Promise 包装
来源：http://ka.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://pu.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://sh.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kt.chemitech.net.cn

[U97] JS：并发请求
来源：http://yn.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mq.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://gq.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ro.newstarts.cn

[U99] JS：事件监听
来源：http://gf.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://sk.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://si.nszjky.cn

document.querySelector(".item")
来源：http://vd.bjjhwx.cn

[U101] JS：classList 操作
来源：http://id.hnjuh.cn

el.classList.toggle("active")
来源：http://tg.gzmigu.cn

[U102] JS：本地存储
来源：http://tz.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oi.hahajie.cn

[U103] JS：定时器
来源：http://iu.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://il.hahajie.cn

[U104] JS：防抖
来源：http://hc.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kq.hnjuh.cn

[U105] JS：节流
来源：http://bs.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kj.bjjhwx.cn

[U106] JS：日期格式化
来源：http://jx.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zh.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://rk.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kt.hahajie.cn

[U108] JS：随机整数
来源：http://nk.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kc.9csxet.cn

[U109] JS：数组分组
来源：http://ls.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://mb.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://da.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tu.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://pb.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://yy.jctech888.com.cn

[U112] JS：字符串补位
来源：http://md.gzmigu.cn

"7".padStart(3, "0")
来源：http://mz.nicolike.cn

[U113] JS：正则替换全部
来源：http://ah.521024.cn

s.replaceAll("a", "b")
来源：http://wa.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://ow.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dv.newstarts.cn

[U115] JS：生成 UUID
来源：http://ir.shxzskj.cn

crypto.randomUUID()
来源：http://wu.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://nz.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://pu.521024.cn

[U117] JS：单元测试
来源：http://io.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://om.hnjuh.cn

[U118] JS：开发服务器
来源：http://xr.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://qp.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://se.yuntaijiaju.cn

npx vite build
来源：http://zv.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://vq.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://hu.huanxung.cn

================================================================================
来源：http://yq.panjiajie.cn

统计汇总
来源：http://yx.9csxet.cn

================================================================================
来源：http://yl.colortex.cn

按语言统计（条）：
来源：http://tm.nicolike.cn

Python ......... 252
来源：http://rn.wgjwhj.cn

PHP ............ 252
来源：http://wl.huixinmuqiang.cn

JavaScript ..... 252
来源：http://im.hahajie.cn

TypeScript ..... 212
来源：http://as.szsharing.cn

Java ........... 212
来源：http://rj.muxihuayi.cn

Go ............. 212
来源：http://so.asd995.cn

Ruby ........... 212
来源：http://ck.panjiajie.cn

C# ............. 212
来源：http://hb.nicolike.cn

C .............. 30
来源：http://qq.colortex.cn

C++ ............ 30
来源：http://fw.jianghongdianzi.cn

SQL ............ 90
来源：http://jw.muxihuayi.cn

Bash ........... 80
来源：http://mu.hnjuh.cn

Kotlin ......... 15
来源：http://mh.muxihuayi.cn

Swift .......... 15
来源：http://rz.panjiajie.cn

Lua ............ 10
来源：http://bm.chemitech.net.cn

Perl ........... 10
来源：http://zi.jctech888.com.cn

Scala .......... 10
来源：http://iq.bookmarksfly.cn

------------------------------------
来源：http://hq.huanxung.cn

合计 ........... 2106 条
来源：http://lf.bookmarksfly.cn

按章节统计：
来源：http://ic.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mt.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ng.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lx.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vz.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wx.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ed.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ic.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://le.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hx.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://si.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tz.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nr.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vi.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://af.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vf.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lf.colortex.cn

Q SQL 专题                              90
来源：http://nu.colortex.cn

R Bash 专题                             80
来源：http://rh.521024.cn

S C / C++ 专题                          60
来源：http://pk.521024.cn

T 其他语言补充                          60
来源：http://un.chemitech.net.cn

U 高频实用片段                         120
来源：http://bk.gzmigu.cn

------------------------------------
来源：http://fl.colortex.cn

合计                                  2106 条
来源：http://dk.nszjky.cn

--------------------------------------------------------------------------------
来源：http://bu.huanxung.cn

使用提醒
来源：http://od.szsharing.cn

--------------------------------------------------------------------------------
来源：http://lq.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gf.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tv.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ym.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xi.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ft.bjjhwx.cn

—— 文件结束 ——
来源：http://ot.huanxung.cn

================================================================================
来源：http://st.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://xk.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://ow.colortex.cn

================================================================================
来源：http://qq.hahajie.cn

【收录内容】
来源：http://po.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://td.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qz.hnjuh.cn

SQL · Bash · C · C++
来源：http://zl.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ya.bookmarksfly.cn

【使用说明】
来源：http://mo.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gz.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wk.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ju.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://th.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hf.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fi.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://di.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jh.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tw.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://md.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sc.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wx.521024.cn

【文件统计】
来源：http://jg.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://on.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://gp.wgjwhj.cn

目  录
来源：http://kn.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://cz.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ne.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zp.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vq.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dc.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ga.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gd.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mw.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ip.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pi.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jh.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pp.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ku.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kc.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ik.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://la.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://no.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kf.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://im.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yv.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lv.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yt.haigaiapp.cn

================================================================================
来源：http://wk.colortex.cn

A. 基础语法与类型
来源：http://vz.panjiajie.cn

================================================================================
来源：http://is.hnjuh.cn

[A01] Hello World
来源：http://ob.panjiajie.cn

Py:   print("Hello, World!")
来源：http://sj.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://ot.asd995.cn

JS:   console.log("Hello, World!");
来源：http://rp.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uu.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://ch.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://hs.521024.cn

Ruby: puts "Hello, World!"
来源：http://qz.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://se.newstarts.cn

[A02] 变量声明与赋值
来源：http://db.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vn.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qh.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oy.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ag.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://mi.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://aq.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://lw.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ge.gzmigu.cn

[A03] 常量定义
来源：http://qg.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://be.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://ea.521024.cn

JS:   const PI = 3.14159;
来源：http://su.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://rv.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://fv.shxzskj.cn

Go:   const PI = 3.14159
来源：http://jl.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://yf.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://bz.hahajie.cn

[A04] 判断变量类型
来源：http://ty.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ig.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ge.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xk.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://ol.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zj.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ri.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kg.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://ca.nicolike.cn

[A05] 整数除法与取模
来源：http://hs.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://we.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kv.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zo.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://if.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://kg.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://rn.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://qn.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://ed.lnxyls.cn

[A06] 字符串转数字
来源：http://uc.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://ld.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dw.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hm.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pk.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wd.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ac.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xu.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://et.hahajie.cn

[A07] 数字转字符串
来源：http://ve.nicolike.cn

Py:   str(42)
来源：http://la.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://zz.huixiangedu.cn


<!-- 参考信息 -->