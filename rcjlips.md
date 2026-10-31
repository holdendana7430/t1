代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://fp.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rx.huixiangedu.cn

[U46] PHP：可空类型
来源：http://vk.gzmigu.cn

?string $name = null
来源：http://ga.gzmigu.cn

[U47] PHP：联合类型
来源：http://hp.asd995.cn

int|string $id
来源：http://zu.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://jv.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kh.huanxung.cn

[U49] PHP：只读属性
来源：http://gz.newstarts.cn

public readonly string $name
来源：http://sx.colortex.cn

[U50] PHP：构造器属性提升
来源：http://xs.nszjky.cn

public function __construct(private int $id) {}
来源：http://uq.9csxet.cn

[U51] PHP：数组解构
来源：http://kq.haigaiapp.cn

[$a, $b] = $arr;
来源：http://so.gzmigu.cn

[U52] PHP：箭头函数
来源：http://bg.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://lk.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://fj.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://dk.lnxyls.cn

[U54] PHP：空安全调用
来源：http://fa.haigaiapp.cn

$obj?->method()
来源：http://fr.asd995.cn

[U55] PHP：match 表达式
来源：http://gg.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://av.gzmigu.cn

[U56] PHP：命名参数
来源：http://mb.yuexingan06.cn

f(a: 1, b: 2)
来源：http://hl.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://pt.muxihuayi.cn

"值: {$a}"
来源：http://am.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://wv.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eb.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://bl.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://be.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://dr.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://td.panjiajie.cn

[U61] PHP：正则
来源：http://hp.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://py.huixiangedu.cn

[U62] PHP：日期对象
来源：http://nf.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zl.hahajie.cn

[U63] PHP：文件读写
来源：http://yg.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jv.colortex.cn

[U64] PHP：目录遍历
来源：http://xw.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://vr.colortex.cn

[U65] PHP：会话
来源：http://nh.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ae.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://zj.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rv.nszjky.cn

[U67] PHP：处理文件上传
来源：http://sx.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ws.colortex.cn

[U68] PHP：PDO 连接
来源：http://dq.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ru.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://zf.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vi.szsharing.cn

[U70] PHP：PDO 事务
来源：http://xa.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hl.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://py.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://ri.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://pn.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://uj.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://bl.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://ur.9csxet.cn

[U74] PHP：读取环境变量
来源：http://rp.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://gt.nszjky.cn

[U75] PHP：依赖注入
来源：http://dw.wgjwhj.cn

composer require psr/container
来源：http://db.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://cf.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ek.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://tr.hnjuh.cn

composer require twig/twig
来源：http://aw.9csxet.cn

[U78] PHP：单元测试
来源：http://lc.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://hi.yuexingan06.cn

[U79] PHP：静态分析
来源：http://yg.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://op.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://du.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pk.huanxung.cn

[U81] JS：初始化项目
来源：http://cn.chemitech.net.cn

npm init -y;  npm i express
来源：http://hi.colortex.cn

[U82] JS：package.json 脚本
来源：http://sx.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yw.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://hu.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qi.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://vr.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cx.bookmarksfly.cn

[U85] JS：可选链
来源：http://ze.colortex.cn

a?.b?.c
来源：http://gp.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://vg.gzmigu.cn

a ?? b
来源：http://qg.bjjhwx.cn

[U87] JS：解构默认值
来源：http://wa.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://bk.nszjky.cn

[U88] JS：对象展开合并
来源：http://op.hahajie.cn

{ ...a, ...b }
来源：http://la.haigaiapp.cn

[U89] JS：数组去重
来源：http://fs.yuexingan06.cn

[...new Set(arr)]
来源：http://sg.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://gu.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://mp.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://wh.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aj.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://wd.9csxet.cn

structuredClone(obj)
来源：http://px.asd995.cn

[U93] JS：模板字符串
来源：http://yo.szxytkj.cn

`共 ${n} 条`
来源：http://jq.chemitech.net.cn

[U94] JS：箭头函数
来源：http://oa.asd995.cn

const double = x => x * 2;
来源：http://zb.hahajie.cn

[U95] JS：Promise 包装
来源：http://sv.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://pe.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://um.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tx.szsharing.cn

[U97] JS：并发请求
来源：http://rf.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eh.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://co.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uh.hahajie.cn

[U99] JS：事件监听
来源：http://co.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://ko.asd995.cn

[U100] JS：DOM 查询
来源：http://uz.jianghongdianzi.cn

document.querySelector(".item")
来源：http://lg.nszjky.cn

[U101] JS：classList 操作
来源：http://uk.shxzukj.cn

el.classList.toggle("active")
来源：http://nc.colortex.cn

[U102] JS：本地存储
来源：http://gn.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cj.yuexingan06.cn

[U103] JS：定时器
来源：http://yi.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://du.nicolike.cn

[U104] JS：防抖
来源：http://kj.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fe.jctech888.com.cn

[U105] JS：节流
来源：http://ki.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pv.9csxet.cn

[U106] JS：日期格式化
来源：http://ov.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mr.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://vj.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ad.muxihuayi.cn

[U108] JS：随机整数
来源：http://bb.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iz.wgjwhj.cn

[U109] JS：数组分组
来源：http://ih.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://av.jctech888.com.cn

[U110] JS：数组分块
来源：http://ds.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tr.shxzukj.cn

[U111] JS：对象转 Map
来源：http://fc.huanxung.cn

new Map(Object.entries(obj))
来源：http://lx.gzmigu.cn

[U112] JS：字符串补位
来源：http://rn.newstarts.cn

"7".padStart(3, "0")
来源：http://fu.hahajie.cn

[U113] JS：正则替换全部
来源：http://or.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://qp.nszjky.cn

[U114] JS：JSON 深比较
来源：http://kp.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ka.521024.cn

[U115] JS：生成 UUID
来源：http://lh.jianghongdianzi.cn

crypto.randomUUID()
来源：http://go.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://sa.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://xn.hnjuh.cn

[U117] JS：单元测试
来源：http://es.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://yc.szxytkj.cn

[U118] JS：开发服务器
来源：http://rv.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://ib.lnxyls.cn

[U119] JS：生产构建
来源：http://ri.yuexingan06.cn

npx vite build
来源：http://cx.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://iw.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://na.szxytkj.cn

================================================================================
来源：http://ec.muxihuayi.cn

统计汇总
来源：http://en.yuexingan06.cn

================================================================================
来源：http://eu.hahajie.cn

按语言统计（条）：
来源：http://ik.shxzskj.cn

Python ......... 252
来源：http://uw.asd995.cn

PHP ............ 252
来源：http://jx.shxzukj.cn

JavaScript ..... 252
来源：http://ne.huanxung.cn

TypeScript ..... 212
来源：http://ku.muxihuayi.cn

Java ........... 212
来源：http://wg.muxihuayi.cn

Go ............. 212
来源：http://oy.yuntaijiaju.cn

Ruby ........... 212
来源：http://bd.colortex.cn

C# ............. 212
来源：http://ft.szxytkj.cn

C .............. 30
来源：http://wc.hahajie.cn

C++ ............ 30
来源：http://vv.wgjwhj.cn

SQL ............ 90
来源：http://ur.yuntaijiaju.cn

Bash ........... 80
来源：http://ps.hahajie.cn

Kotlin ......... 15
来源：http://zy.asd995.cn

Swift .......... 15
来源：http://fo.chemitech.net.cn

Lua ............ 10
来源：http://lq.nszjky.cn

Perl ........... 10
来源：http://jc.lnxyls.cn

Scala .......... 10
来源：http://jq.colortex.cn

------------------------------------
来源：http://ty.huanxung.cn

合计 ........... 2106 条
来源：http://eo.bookmarksfly.cn

按章节统计：
来源：http://vt.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hg.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wl.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rg.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xg.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gp.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yf.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ik.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pa.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ua.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dy.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zy.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eh.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ny.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://el.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ch.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rt.colortex.cn

Q SQL 专题                              90
来源：http://tp.jctech888.com.cn

R Bash 专题                             80
来源：http://sn.bjjhwx.cn

S C / C++ 专题                          60
来源：http://vr.nszjky.cn

T 其他语言补充                          60
来源：http://tp.nszjky.cn

U 高频实用片段                         120
来源：http://ed.bjjhwx.cn

------------------------------------
来源：http://ko.szsharing.cn

合计                                  2106 条
来源：http://cf.huanxung.cn

--------------------------------------------------------------------------------
来源：http://vx.hahajie.cn

使用提醒
来源：http://tp.nszjky.cn

--------------------------------------------------------------------------------
来源：http://xr.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kb.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bm.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vm.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bj.hnjuh.cn

—— 文件结束 ——
来源：http://mq.gzmigu.cn

================================================================================
来源：http://dj.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://ck.asd995.cn

Common Programming Examples Cheat Book
来源：http://gb.9csxet.cn

================================================================================
来源：http://uo.bookmarksfly.cn

【收录内容】
来源：http://nl.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ks.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pk.9csxet.cn

SQL · Bash · C · C++
来源：http://xw.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pn.muxihuayi.cn

【使用说明】
来源：http://dw.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tr.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://px.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ab.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tj.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mc.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jl.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vp.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yi.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ls.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dz.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dp.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gm.panjiajie.cn

【文件统计】
来源：http://jx.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mp.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ir.chemitech.net.cn

目  录
来源：http://vi.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://hw.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://up.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sq.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bc.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lj.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fr.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ce.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ko.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qz.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mr.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nb.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vv.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://px.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oe.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ad.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hd.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jh.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zr.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xq.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vk.jianghongdianzi.cn

================================================================================
来源：http://rl.asd995.cn

A. 基础语法与类型
来源：http://gv.colortex.cn

================================================================================
来源：http://ib.newstarts.cn

[A01] Hello World
来源：http://vx.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://xd.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://qv.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://my.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kc.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://wb.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://fu.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://xe.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zv.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://ip.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vt.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pp.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://so.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gr.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://fo.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://rb.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://fb.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wc.hnjuh.cn

[A03] 常量定义
来源：http://md.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sf.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://xf.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://rw.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://jz.521024.cn

Java: static final double PI = 3.14159;
来源：http://ot.9csxet.cn

Go:   const PI = 3.14159
来源：http://ui.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://zo.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://ju.newstarts.cn

[A04] 判断变量类型
来源：http://je.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zu.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://be.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lj.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://zp.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dd.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cz.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mm.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://kj.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://kg.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wx.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hi.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jk.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bc.yuntaijiaju.cn


<!-- 参考信息 -->