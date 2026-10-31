代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://kv.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oc.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://pr.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bp.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://aw.szxytkj.cn

namespace App\Http;
来源：http://py.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://gt.chemitech.net.cn

declare(strict_types=1);
来源：http://aa.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://jx.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zb.hahajie.cn

[U46] PHP：可空类型
来源：http://rw.szsharing.cn

?string $name = null
来源：http://ly.hnjuh.cn

[U47] PHP：联合类型
来源：http://lb.shtwfgs.cn

int|string $id
来源：http://wl.colortex.cn

[U48] PHP：纯枚举
来源：http://fa.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sf.jctech888.com.cn

[U49] PHP：只读属性
来源：http://ou.huixiangedu.cn

public readonly string $name
来源：http://mt.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://uj.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://bj.chemitech.net.cn

[U51] PHP：数组解构
来源：http://ls.huanxung.cn

[$a, $b] = $arr;
来源：http://er.huanxung.cn

[U52] PHP：箭头函数
来源：http://jf.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://hg.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://ex.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://eg.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://ye.521024.cn

$obj?->method()
来源：http://hp.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://fu.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://er.nicolike.cn

[U56] PHP：命名参数
来源：http://yc.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://wy.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://bg.panjiajie.cn

"值: {$a}"
来源：http://lb.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://qw.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qj.hnjuh.cn

[U59] PHP：自定义排序
来源：http://df.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://at.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://ke.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gn.haigaiapp.cn

[U61] PHP：正则
来源：http://qu.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ha.shtwfgs.cn

[U62] PHP：日期对象
来源：http://ze.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ti.hnjuh.cn

[U63] PHP：文件读写
来源：http://op.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sr.szxytkj.cn

[U64] PHP：目录遍历
来源：http://kh.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://pi.wgjwhj.cn

[U65] PHP：会话
来源：http://dz.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ez.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://nf.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bv.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://di.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vk.nicolike.cn

[U68] PHP：PDO 连接
来源：http://rd.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hm.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://ab.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cl.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://bw.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://un.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://fb.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://xk.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://tc.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://mz.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://wp.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://ls.9csxet.cn

[U74] PHP：读取环境变量
来源：http://pd.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://xk.colortex.cn

[U75] PHP：依赖注入
来源：http://ny.huanxung.cn

composer require psr/container
来源：http://ta.jctech888.com.cn

[U76] PHP：简单路由
来源：http://ij.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gn.shxzskj.cn

[U77] PHP：模板渲染
来源：http://yh.asd995.cn

composer require twig/twig
来源：http://pw.521024.cn

[U78] PHP：单元测试
来源：http://ii.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://zn.colortex.cn

[U79] PHP：静态分析
来源：http://rz.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://bb.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://vs.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://us.huanxung.cn

[U81] JS：初始化项目
来源：http://lx.yuexingan06.cn

npm init -y;  npm i express
来源：http://gr.nszjky.cn

[U82] JS：package.json 脚本
来源：http://cc.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hl.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://or.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qu.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://sx.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eo.szxytkj.cn

[U85] JS：可选链
来源：http://dz.szsharing.cn

a?.b?.c
来源：http://wu.hahajie.cn

[U86] JS：空值合并
来源：http://te.newstarts.cn

a ?? b
来源：http://lg.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ju.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://ws.9csxet.cn

[U88] JS：对象展开合并
来源：http://fx.hahajie.cn

{ ...a, ...b }
来源：http://dy.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://rh.muxihuayi.cn

[...new Set(arr)]
来源：http://od.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://fv.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://em.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://wd.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nh.gzmigu.cn

[U92] JS：深拷贝
来源：http://ce.nicolike.cn

structuredClone(obj)
来源：http://rb.9csxet.cn

[U93] JS：模板字符串
来源：http://ui.huixiangedu.cn

`共 ${n} 条`
来源：http://kh.chemitech.net.cn

[U94] JS：箭头函数
来源：http://ne.9csxet.cn

const double = x => x * 2;
来源：http://qs.panjiajie.cn

[U95] JS：Promise 包装
来源：http://rf.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://nv.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://xd.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yv.yuexingan06.cn

[U97] JS：并发请求
来源：http://xq.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ao.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://ty.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gp.nszjky.cn

[U99] JS：事件监听
来源：http://pt.nszjky.cn

el.addEventListener("click", e => {})
来源：http://eo.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://tp.jctech888.com.cn

document.querySelector(".item")
来源：http://qw.szsharing.cn

[U101] JS：classList 操作
来源：http://pb.shxzukj.cn

el.classList.toggle("active")
来源：http://nm.nszjky.cn

[U102] JS：本地存储
来源：http://nf.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xh.hnjuh.cn

[U103] JS：定时器
来源：http://yn.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vc.lnxyls.cn

[U104] JS：防抖
来源：http://sj.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ae.asd995.cn

[U105] JS：节流
来源：http://ex.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lo.shxzskj.cn

[U106] JS：日期格式化
来源：http://fb.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rj.huixiangedu.cn

[U107] JS：数字千分位
来源：http://xr.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cx.gzmigu.cn

[U108] JS：随机整数
来源：http://ou.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gm.nszjky.cn

[U109] JS：数组分组
来源：http://tp.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://fx.hahajie.cn

[U110] JS：数组分块
来源：http://tw.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://di.9csxet.cn

[U111] JS：对象转 Map
来源：http://ld.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://qa.hnjuh.cn

[U112] JS：字符串补位
来源：http://md.chemitech.net.cn

"7".padStart(3, "0")
来源：http://cj.shxzskj.cn

[U113] JS：正则替换全部
来源：http://qs.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://tk.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://mc.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rr.huanxung.cn

[U115] JS：生成 UUID
来源：http://fh.colortex.cn

crypto.randomUUID()
来源：http://nn.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://rn.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://su.muxihuayi.cn

[U117] JS：单元测试
来源：http://zr.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://bk.nszjky.cn

[U118] JS：开发服务器
来源：http://fx.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://mb.lnxyls.cn

[U119] JS：生产构建
来源：http://lr.huixiangedu.cn

npx vite build
来源：http://da.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://vd.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://lo.yuexingan06.cn

================================================================================
来源：http://xa.521024.cn

统计汇总
来源：http://tp.nszjky.cn

================================================================================
来源：http://ld.szsharing.cn

按语言统计（条）：
来源：http://ae.shtwfgs.cn

Python ......... 252
来源：http://ku.nszjky.cn

PHP ............ 252
来源：http://yd.lnxyls.cn

JavaScript ..... 252
来源：http://oa.bjjhwx.cn

TypeScript ..... 212
来源：http://dq.wgjwhj.cn

Java ........... 212
来源：http://lf.521024.cn

Go ............. 212
来源：http://cj.newstarts.cn

Ruby ........... 212
来源：http://ks.lnxyls.cn

C# ............. 212
来源：http://rj.nicolike.cn

C .............. 30
来源：http://jk.jctech888.com.cn

C++ ............ 30
来源：http://fg.jctech888.com.cn

SQL ............ 90
来源：http://jb.521024.cn

Bash ........... 80
来源：http://lr.szsharing.cn

Kotlin ......... 15
来源：http://oi.haigaiapp.cn

Swift .......... 15
来源：http://nk.newstarts.cn

Lua ............ 10
来源：http://tr.szsharing.cn

Perl ........... 10
来源：http://aw.wgjwhj.cn

Scala .......... 10
来源：http://gd.shxzukj.cn

------------------------------------
来源：http://bm.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://wt.wgjwhj.cn

按章节统计：
来源：http://yl.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wf.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xv.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nq.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kw.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hm.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ev.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://em.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ef.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gs.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jq.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uq.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yd.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ks.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sw.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rr.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cw.bjjhwx.cn

Q SQL 专题                              90
来源：http://gg.szxytkj.cn

R Bash 专题                             80
来源：http://vs.gzmigu.cn

S C / C++ 专题                          60
来源：http://ah.huanxung.cn

T 其他语言补充                          60
来源：http://fx.nszjky.cn

U 高频实用片段                         120
来源：http://uj.bookmarksfly.cn

------------------------------------
来源：http://qk.newstarts.cn

合计                                  2106 条
来源：http://wt.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ap.shxzukj.cn

使用提醒
来源：http://jo.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://uh.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zr.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bx.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bh.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://it.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ma.asd995.cn

—— 文件结束 ——
来源：http://jg.szxytkj.cn

================================================================================
来源：http://oz.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://cy.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://gy.haigaiapp.cn

================================================================================
来源：http://sw.nicolike.cn

【收录内容】
来源：http://wy.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fl.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rv.colortex.cn

SQL · Bash · C · C++
来源：http://rp.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kn.haigaiapp.cn

【使用说明】
来源：http://sw.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ne.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pi.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qg.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yh.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cr.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gg.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hv.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lc.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tc.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yu.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jq.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nk.huanxung.cn

【文件统计】
来源：http://xp.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yg.nszjky.cn

--------------------------------------------------------------------------------
来源：http://az.nicolike.cn

目  录
来源：http://ag.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://xp.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pr.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hm.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vd.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://do.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zg.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://or.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sg.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://co.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://na.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xw.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ox.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qx.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kt.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cq.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://el.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://id.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://px.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ap.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hv.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qe.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nj.wgjwhj.cn

================================================================================
来源：http://zv.shtwfgs.cn

A. 基础语法与类型
来源：http://ue.newstarts.cn

================================================================================
来源：http://mg.9csxet.cn

[A01] Hello World
来源：http://wu.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://zi.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://ii.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://aa.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qr.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://kx.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://ru.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://so.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wh.hnjuh.cn

[A02] 变量声明与赋值
来源：http://yt.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nl.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pd.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vs.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gw.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://nj.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://oh.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://pp.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tr.nszjky.cn

[A03] 常量定义
来源：http://sc.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bq.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://fa.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://jc.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://hv.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://rx.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://be.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://km.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://yi.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://hq.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://an.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lw.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yz.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://fn.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pr.hahajie.cn


<!-- 参考信息 -->