代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://jk.shtwfgs.cn

sys.stdout.isatty()
来源：http://ns.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://xl.hnjuh.cn

print("err", file=sys.stderr)
来源：http://qj.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://xr.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qb.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://sn.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dv.521024.cn

[U43] PHP：声明命名空间
来源：http://jb.gzmigu.cn

namespace App\Http;
来源：http://lb.huanxung.cn

[U44] PHP：开启严格类型
来源：http://ml.szxytkj.cn

declare(strict_types=1);
来源：http://fx.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://gv.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tn.colortex.cn

[U46] PHP：可空类型
来源：http://sq.bookmarksfly.cn

?string $name = null
来源：http://ea.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://nh.lnxyls.cn

int|string $id
来源：http://pg.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://sy.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ng.bjjhwx.cn

[U49] PHP：只读属性
来源：http://gv.jianghongdianzi.cn

public readonly string $name
来源：http://bz.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://fc.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://cw.huixiangedu.cn

[U51] PHP：数组解构
来源：http://tx.gzmigu.cn

[$a, $b] = $arr;
来源：http://uo.asd995.cn

[U52] PHP：箭头函数
来源：http://rr.asd995.cn

$double = fn($x) => $x * 2;
来源：http://sr.nicolike.cn

[U53] PHP：空合并运算符
来源：http://yi.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://fk.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://zq.jctech888.com.cn

$obj?->method()
来源：http://wn.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://hk.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uy.szsharing.cn

[U56] PHP：命名参数
来源：http://zj.muxihuayi.cn

f(a: 1, b: 2)
来源：http://fl.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://ni.hahajie.cn

"值: {$a}"
来源：http://qw.lnxyls.cn

[U58] PHP：数组三件套
来源：http://bv.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bp.gzmigu.cn

[U59] PHP：自定义排序
来源：http://cl.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xj.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://sr.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lz.hnjuh.cn

[U61] PHP：正则
来源：http://da.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xt.newstarts.cn

[U62] PHP：日期对象
来源：http://ld.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://if.shxzskj.cn

[U63] PHP：文件读写
来源：http://jm.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://we.nszjky.cn

[U64] PHP：目录遍历
来源：http://ig.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ow.gzmigu.cn

[U65] PHP：会话
来源：http://ry.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://le.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://mt.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lv.521024.cn

[U67] PHP：处理文件上传
来源：http://gk.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pu.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://rw.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wh.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://af.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zp.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://sz.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ek.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://od.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://tf.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://pg.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://sh.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://yu.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://lb.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://id.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://ak.szxytkj.cn

[U75] PHP：依赖注入
来源：http://lg.shxzukj.cn

composer require psr/container
来源：http://ve.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://fo.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ty.9csxet.cn

[U77] PHP：模板渲染
来源：http://ld.jianghongdianzi.cn

composer require twig/twig
来源：http://uw.asd995.cn

[U78] PHP：单元测试
来源：http://he.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://wd.hnjuh.cn

[U79] PHP：静态分析
来源：http://ee.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://uz.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://vg.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kg.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://zv.panjiajie.cn

npm init -y;  npm i express
来源：http://gz.nicolike.cn

[U82] JS：package.json 脚本
来源：http://jb.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sg.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://ts.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://he.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://kt.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cr.chemitech.net.cn

[U85] JS：可选链
来源：http://kq.hnjuh.cn

a?.b?.c
来源：http://kc.gzmigu.cn

[U86] JS：空值合并
来源：http://yw.wgjwhj.cn

a ?? b
来源：http://df.newstarts.cn

[U87] JS：解构默认值
来源：http://ko.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://bw.asd995.cn

[U88] JS：对象展开合并
来源：http://as.bjjhwx.cn

{ ...a, ...b }
来源：http://kh.panjiajie.cn

[U89] JS：数组去重
来源：http://po.hahajie.cn

[...new Set(arr)]
来源：http://tz.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://nc.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://nq.521024.cn

[U91] JS：对象键值遍历
来源：http://na.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fm.haigaiapp.cn

[U92] JS：深拷贝
来源：http://vu.hnjuh.cn

structuredClone(obj)
来源：http://jr.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://td.asd995.cn

`共 ${n} 条`
来源：http://eb.9csxet.cn

[U94] JS：箭头函数
来源：http://hw.szsharing.cn

const double = x => x * 2;
来源：http://db.szsharing.cn

[U95] JS：Promise 包装
来源：http://li.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://kz.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://no.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dt.wgjwhj.cn

[U97] JS：并发请求
来源：http://yw.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lp.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://yj.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ue.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://fj.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://th.nszjky.cn

[U100] JS：DOM 查询
来源：http://lk.yuntaijiaju.cn

document.querySelector(".item")
来源：http://ti.521024.cn

[U101] JS：classList 操作
来源：http://fb.chemitech.net.cn

el.classList.toggle("active")
来源：http://ds.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://ar.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://by.asd995.cn

[U103] JS：定时器
来源：http://qw.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://al.jctech888.com.cn

[U104] JS：防抖
来源：http://nw.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ap.huixinmuqiang.cn

[U105] JS：节流
来源：http://ab.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pf.colortex.cn

[U106] JS：日期格式化
来源：http://ch.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fn.panjiajie.cn

[U107] JS：数字千分位
来源：http://td.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wc.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://vy.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pu.gzmigu.cn

[U109] JS：数组分组
来源：http://lr.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://zf.lnxyls.cn

[U110] JS：数组分块
来源：http://gn.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oz.nszjky.cn

[U111] JS：对象转 Map
来源：http://rd.huanxung.cn

new Map(Object.entries(obj))
来源：http://vy.gzmigu.cn

[U112] JS：字符串补位
来源：http://jm.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://qi.521024.cn

[U113] JS：正则替换全部
来源：http://ym.521024.cn

s.replaceAll("a", "b")
来源：http://dc.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://lx.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vo.521024.cn

[U115] JS：生成 UUID
来源：http://mv.nszjky.cn

crypto.randomUUID()
来源：http://of.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://mu.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://bc.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://od.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://le.hahajie.cn

[U118] JS：开发服务器
来源：http://sr.lnxyls.cn

npm i -D vite;  npx vite
来源：http://ad.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://br.shxzskj.cn

npx vite build
来源：http://rv.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://dj.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://qf.haigaiapp.cn

================================================================================
来源：http://dy.shxzukj.cn

统计汇总
来源：http://pa.521024.cn

================================================================================
来源：http://sr.shxzukj.cn

按语言统计（条）：
来源：http://oe.chemitech.net.cn

Python ......... 252
来源：http://ze.haigaiapp.cn

PHP ............ 252
来源：http://eg.jctech888.com.cn

JavaScript ..... 252
来源：http://ua.521024.cn

TypeScript ..... 212
来源：http://zq.huanxung.cn

Java ........... 212
来源：http://ap.gzmigu.cn

Go ............. 212
来源：http://lx.wgjwhj.cn

Ruby ........... 212
来源：http://qn.chemitech.net.cn

C# ............. 212
来源：http://ud.yuexingan06.cn

C .............. 30
来源：http://kn.jctech888.com.cn

C++ ............ 30
来源：http://af.hnjuh.cn

SQL ............ 90
来源：http://au.lnxyls.cn

Bash ........... 80
来源：http://pl.bookmarksfly.cn

Kotlin ......... 15
来源：http://in.yuntaijiaju.cn

Swift .......... 15
来源：http://tu.hnjuh.cn

Lua ............ 10
来源：http://fp.shxzskj.cn

Perl ........... 10
来源：http://pk.nszjky.cn

Scala .......... 10
来源：http://la.colortex.cn

------------------------------------
来源：http://qc.shtwfgs.cn

合计 ........... 2106 条
来源：http://cd.wgjwhj.cn

按章节统计：
来源：http://iy.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://in.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ie.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sr.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yw.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ce.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wt.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fm.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://as.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mk.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pv.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dl.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cd.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jx.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://od.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rd.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iq.nicolike.cn

Q SQL 专题                              90
来源：http://gq.jctech888.com.cn

R Bash 专题                             80
来源：http://bz.jctech888.com.cn

S C / C++ 专题                          60
来源：http://rg.panjiajie.cn

T 其他语言补充                          60
来源：http://ew.szsharing.cn

U 高频实用片段                         120
来源：http://rm.bjjhwx.cn

------------------------------------
来源：http://ta.haigaiapp.cn

合计                                  2106 条
来源：http://hw.hahajie.cn

--------------------------------------------------------------------------------
来源：http://rk.colortex.cn

使用提醒
来源：http://bh.nszjky.cn

--------------------------------------------------------------------------------
来源：http://gr.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lj.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qz.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zx.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dj.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://us.lnxyls.cn

—— 文件结束 ——
来源：http://tj.yuexingan06.cn

================================================================================
来源：http://oa.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://by.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://wh.yuexingan06.cn

================================================================================
来源：http://vn.hahajie.cn

【收录内容】
来源：http://rl.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pe.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sv.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://ob.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wi.haigaiapp.cn

【使用说明】
来源：http://da.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iq.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zq.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pp.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://je.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ty.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vs.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ie.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yj.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zk.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zj.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vx.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://da.huixiangedu.cn

【文件统计】
来源：http://yl.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yq.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://jy.szxytkj.cn

目  录
来源：http://kt.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://dc.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uy.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yh.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aa.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rl.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://km.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ro.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mh.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ws.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hg.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qu.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oc.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://on.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qs.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xf.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fc.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nk.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pv.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ds.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sk.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://om.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yq.muxihuayi.cn

================================================================================
来源：http://ye.bookmarksfly.cn

A. 基础语法与类型
来源：http://mq.521024.cn

================================================================================
来源：http://co.jianghongdianzi.cn

[A01] Hello World
来源：http://pe.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://oy.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://xl.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://zo.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hv.521024.cn

Java: System.out.println("Hello, World!");
来源：http://se.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://th.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://tf.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ra.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://pw.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zl.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://na.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ot.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://si.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://nb.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://yw.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://uf.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gt.wgjwhj.cn

[A03] 常量定义
来源：http://pu.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gc.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://pz.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://ke.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://bb.521024.cn

Java: static final double PI = 3.14159;
来源：http://js.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://sl.gzmigu.cn

Ruby: PI = 3.14159
来源：http://gp.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://dr.colortex.cn

[A04] 判断变量类型
来源：http://lr.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uq.colortex.cn


<!-- 参考信息 -->