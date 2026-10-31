代发 wailian999

[U47] PHP：联合类型
来源：http://tl.nicolike.cn

int|string $id
来源：http://py.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://df.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ij.huixiangedu.cn

[U49] PHP：只读属性
来源：http://br.colortex.cn

public readonly string $name
来源：http://ls.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://zh.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://am.hahajie.cn

[U51] PHP：数组解构
来源：http://hf.chemitech.net.cn

[$a, $b] = $arr;
来源：http://jy.szxytkj.cn

[U52] PHP：箭头函数
来源：http://og.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://dw.9csxet.cn

[U53] PHP：空合并运算符
来源：http://ip.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://my.nszjky.cn

[U54] PHP：空安全调用
来源：http://wb.yuntaijiaju.cn

$obj?->method()
来源：http://qh.lnxyls.cn

[U55] PHP：match 表达式
来源：http://fe.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zm.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://mz.haigaiapp.cn

f(a: 1, b: 2)
来源：http://ta.shxzskj.cn

[U57] PHP：字符串插值
来源：http://la.huixinmuqiang.cn

"值: {$a}"
来源：http://qc.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://pl.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uc.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://jf.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://do.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://fj.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eh.nszjky.cn

[U61] PHP：正则
来源：http://ix.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mw.huixiangedu.cn

[U62] PHP：日期对象
来源：http://jz.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jf.gzmigu.cn

[U63] PHP：文件读写
来源：http://hc.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vl.hahajie.cn

[U64] PHP：目录遍历
来源：http://xi.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://kw.chemitech.net.cn

[U65] PHP：会话
来源：http://lq.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://in.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://rx.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ow.szsharing.cn

[U67] PHP：处理文件上传
来源：http://tj.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qg.szsharing.cn

[U68] PHP：PDO 连接
来源：http://kr.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yf.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://wp.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uk.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://dq.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sq.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://op.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://uh.lnxyls.cn

[U72] PHP：写错误日志
来源：http://ba.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://nw.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://lh.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://gu.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://oz.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://ue.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://ci.hahajie.cn

composer require psr/container
来源：http://vq.szsharing.cn

[U76] PHP：简单路由
来源：http://lk.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://md.521024.cn

[U77] PHP：模板渲染
来源：http://dc.jianghongdianzi.cn

composer require twig/twig
来源：http://yt.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://ko.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://bd.521024.cn

[U79] PHP：静态分析
来源：http://uj.521024.cn

composer require --dev phpstan/phpstan
来源：http://di.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://uv.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qa.shxzukj.cn

[U81] JS：初始化项目
来源：http://jy.lnxyls.cn

npm init -y;  npm i express
来源：http://ze.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://vv.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fa.521024.cn

[U83] JS：ES Module 导入导出
来源：http://hp.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vr.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://re.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ee.yuntaijiaju.cn

[U85] JS：可选链
来源：http://kx.newstarts.cn

a?.b?.c
来源：http://pw.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://rf.yuexingan06.cn

a ?? b
来源：http://qs.shtwfgs.cn

[U87] JS：解构默认值
来源：http://xg.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://of.hnjuh.cn

[U88] JS：对象展开合并
来源：http://fe.asd995.cn

{ ...a, ...b }
来源：http://tp.shxzukj.cn

[U89] JS：数组去重
来源：http://qm.newstarts.cn

[...new Set(arr)]
来源：http://zv.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://ih.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://qx.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://fi.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ra.chemitech.net.cn

[U92] JS：深拷贝
来源：http://zz.hnjuh.cn

structuredClone(obj)
来源：http://wr.gzmigu.cn

[U93] JS：模板字符串
来源：http://xm.yuntaijiaju.cn

`共 ${n} 条`
来源：http://xd.hnjuh.cn

[U94] JS：箭头函数
来源：http://nc.lnxyls.cn

const double = x => x * 2;
来源：http://rp.asd995.cn

[U95] JS：Promise 包装
来源：http://es.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://jr.nszjky.cn

[U96] JS：async/await 与异常
来源：http://of.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fz.gzmigu.cn

[U97] JS：并发请求
来源：http://aw.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uj.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://mp.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sc.9csxet.cn

[U99] JS：事件监听
来源：http://pj.9csxet.cn

el.addEventListener("click", e => {})
来源：http://bx.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://ey.bjjhwx.cn

document.querySelector(".item")
来源：http://tv.jctech888.com.cn

[U101] JS：classList 操作
来源：http://id.shxzskj.cn

el.classList.toggle("active")
来源：http://ju.chemitech.net.cn

[U102] JS：本地存储
来源：http://wd.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://je.huixinmuqiang.cn

[U103] JS：定时器
来源：http://yn.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oh.szxytkj.cn

[U104] JS：防抖
来源：http://ow.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lv.bjjhwx.cn

[U105] JS：节流
来源：http://oj.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wc.haigaiapp.cn

[U106] JS：日期格式化
来源：http://mq.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vr.wgjwhj.cn

[U107] JS：数字千分位
来源：http://gj.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ab.9csxet.cn

[U108] JS：随机整数
来源：http://in.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yh.szxytkj.cn

[U109] JS：数组分组
来源：http://nl.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://jg.wgjwhj.cn

[U110] JS：数组分块
来源：http://hy.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ml.gzmigu.cn

[U111] JS：对象转 Map
来源：http://ps.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://ea.huixiangedu.cn

[U112] JS：字符串补位
来源：http://lk.wgjwhj.cn

"7".padStart(3, "0")
来源：http://zj.nicolike.cn

[U113] JS：正则替换全部
来源：http://tl.hahajie.cn

s.replaceAll("a", "b")
来源：http://vv.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://ar.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cu.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://fz.hahajie.cn

crypto.randomUUID()
来源：http://bu.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ps.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://bb.szsharing.cn

[U117] JS：单元测试
来源：http://eh.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://pr.shxzskj.cn

[U118] JS：开发服务器
来源：http://dr.panjiajie.cn

npm i -D vite;  npx vite
来源：http://oc.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://fc.haigaiapp.cn

npx vite build
来源：http://mq.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://hp.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://io.huixinmuqiang.cn

================================================================================
来源：http://ej.huixinmuqiang.cn

统计汇总
来源：http://gd.asd995.cn

================================================================================
来源：http://qw.nszjky.cn

按语言统计（条）：
来源：http://ec.chemitech.net.cn

Python ......... 252
来源：http://xm.jctech888.com.cn

PHP ............ 252
来源：http://fy.hnjuh.cn

JavaScript ..... 252
来源：http://gj.haigaiapp.cn

TypeScript ..... 212
来源：http://qi.shxzukj.cn

Java ........... 212
来源：http://nr.huixiangedu.cn

Go ............. 212
来源：http://ei.9csxet.cn

Ruby ........... 212
来源：http://pw.huixinmuqiang.cn

C# ............. 212
来源：http://zw.9csxet.cn

C .............. 30
来源：http://vb.huixiangedu.cn

C++ ............ 30
来源：http://qt.muxihuayi.cn

SQL ............ 90
来源：http://kc.huixinmuqiang.cn

Bash ........... 80
来源：http://sw.wgjwhj.cn

Kotlin ......... 15
来源：http://fh.shxzskj.cn

Swift .......... 15
来源：http://tn.szsharing.cn

Lua ............ 10
来源：http://dg.haigaiapp.cn

Perl ........... 10
来源：http://mi.nicolike.cn

Scala .......... 10
来源：http://ku.asd995.cn

------------------------------------
来源：http://ek.panjiajie.cn

合计 ........... 2106 条
来源：http://xz.bjjhwx.cn

按章节统计：
来源：http://gv.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tg.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gg.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cc.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hw.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xo.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gs.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cs.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rv.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yv.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ml.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wy.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mi.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mv.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wp.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qa.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://at.521024.cn

Q SQL 专题                              90
来源：http://kq.jianghongdianzi.cn

R Bash 专题                             80
来源：http://ul.nszjky.cn

S C / C++ 专题                          60
来源：http://ph.haigaiapp.cn

T 其他语言补充                          60
来源：http://ti.szxytkj.cn

U 高频实用片段                         120
来源：http://ro.huixinmuqiang.cn

------------------------------------
来源：http://kl.yuexingan06.cn

合计                                  2106 条
来源：http://sn.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://xs.yuntaijiaju.cn

使用提醒
来源：http://dq.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://cb.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ao.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qg.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xh.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pr.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sv.gzmigu.cn

—— 文件结束 ——
来源：http://ag.shxzukj.cn

================================================================================
来源：http://yy.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://kz.521024.cn

Common Programming Examples Cheat Book
来源：http://ux.hnjuh.cn

================================================================================
来源：http://ej.shxzskj.cn

【收录内容】
来源：http://fr.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ee.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://br.9csxet.cn

SQL · Bash · C · C++
来源：http://ss.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yt.newstarts.cn

【使用说明】
来源：http://mj.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jn.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lh.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ya.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ph.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qc.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://os.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://di.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://el.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ot.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nh.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gg.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lt.chemitech.net.cn

【文件统计】
来源：http://iu.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ni.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://wd.shtwfgs.cn

目  录
来源：http://fx.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://mq.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ba.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gd.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fs.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tz.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kx.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rz.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lx.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hr.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xg.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zx.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mq.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pi.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mp.huixiangedu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://en.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://us.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ua.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ls.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ve.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://di.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kd.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ui.szsharing.cn

================================================================================
来源：http://hx.gzmigu.cn

A. 基础语法与类型
来源：http://hf.shxzukj.cn

================================================================================
来源：http://qx.muxihuayi.cn

[A01] Hello World
来源：http://dd.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://ka.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://ep.521024.cn

JS:   console.log("Hello, World!");
来源：http://gk.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ql.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://dw.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://zo.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://hm.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gq.newstarts.cn

[A02] 变量声明与赋值
来源：http://tn.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fv.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fu.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mk.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yf.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://lk.521024.cn

Go:   name := "Alex"; age := 20
来源：http://cx.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://fw.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://un.huixinmuqiang.cn

[A03] 常量定义
来源：http://od.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xv.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://jm.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://ja.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://sk.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://su.gzmigu.cn

Go:   const PI = 3.14159
来源：http://ox.shxzskj.cn

Ruby: PI = 3.14159
来源：http://bd.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://di.yuexingan06.cn

[A04] 判断变量类型
来源：http://tu.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://os.gzmigu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pz.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qw.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://ug.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pb.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ul.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hq.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://sh.shtwfgs.cn

[A05] 整数除法与取模
来源：http://ho.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://op.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ct.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://na.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rv.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://hh.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://uk.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://uc.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://fy.colortex.cn


<!-- 参考信息 -->