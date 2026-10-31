代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://rc.9csxet.cn

sys.stdout.isatty()
来源：http://pi.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://ut.nszjky.cn

print("err", file=sys.stderr)
来源：http://ss.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://dk.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vs.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://oc.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gg.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://xh.chemitech.net.cn

namespace App\Http;
来源：http://yw.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://xp.huixinmuqiang.cn

declare(strict_types=1);
来源：http://vx.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://ff.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dz.haigaiapp.cn

[U46] PHP：可空类型
来源：http://ad.lnxyls.cn

?string $name = null
来源：http://qj.shxzskj.cn

[U47] PHP：联合类型
来源：http://oo.jctech888.com.cn

int|string $id
来源：http://xd.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://ct.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lk.jctech888.com.cn

[U49] PHP：只读属性
来源：http://be.yuexingan06.cn

public readonly string $name
来源：http://ff.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://yk.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://bg.lnxyls.cn

[U51] PHP：数组解构
来源：http://jf.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://os.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://su.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://lf.newstarts.cn

[U53] PHP：空合并运算符
来源：http://wp.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://uc.colortex.cn

[U54] PHP：空安全调用
来源：http://qq.jctech888.com.cn

$obj?->method()
来源：http://ht.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://hb.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qn.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://sw.shxzskj.cn

f(a: 1, b: 2)
来源：http://ru.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://zl.wgjwhj.cn

"值: {$a}"
来源：http://yn.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://mo.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sz.shxzskj.cn

[U59] PHP：自定义排序
来源：http://cx.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gj.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://ut.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wh.lnxyls.cn

[U61] PHP：正则
来源：http://kt.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kr.bjjhwx.cn

[U62] PHP：日期对象
来源：http://vr.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dk.521024.cn

[U63] PHP：文件读写
来源：http://yn.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fo.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://td.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://pq.shxzukj.cn

[U65] PHP：会话
来源：http://bo.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hy.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://uu.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xy.newstarts.cn

[U67] PHP：处理文件上传
来源：http://kq.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hi.huanxung.cn

[U68] PHP：PDO 连接
来源：http://et.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fs.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://nj.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ga.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://ns.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fd.newstarts.cn

[U71] PHP：抛出异常
来源：http://je.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://ss.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://rg.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://hv.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://wp.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://nd.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://uu.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://jw.huanxung.cn

[U75] PHP：依赖注入
来源：http://pt.szsharing.cn

composer require psr/container
来源：http://ap.haigaiapp.cn

[U76] PHP：简单路由
来源：http://sd.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ja.nicolike.cn

[U77] PHP：模板渲染
来源：http://gr.nszjky.cn

composer require twig/twig
来源：http://tx.chemitech.net.cn

[U78] PHP：单元测试
来源：http://yk.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://dy.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://em.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://nl.521024.cn

[U80] PHP：代码规范修复
来源：http://dt.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wm.521024.cn

[U81] JS：初始化项目
来源：http://to.9csxet.cn

npm init -y;  npm i express
来源：http://aq.newstarts.cn

[U82] JS：package.json 脚本
来源：http://bw.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ul.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://vo.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tp.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://xt.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vd.wgjwhj.cn

[U85] JS：可选链
来源：http://yi.521024.cn

a?.b?.c
来源：http://fb.bjjhwx.cn

[U86] JS：空值合并
来源：http://ly.bookmarksfly.cn

a ?? b
来源：http://mr.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://eh.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://bn.gzmigu.cn

[U88] JS：对象展开合并
来源：http://xt.newstarts.cn

{ ...a, ...b }
来源：http://vb.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://et.nicolike.cn

[...new Set(arr)]
来源：http://mv.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://eh.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://sw.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://ci.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vh.gzmigu.cn

[U92] JS：深拷贝
来源：http://cz.yuexingan06.cn

structuredClone(obj)
来源：http://lv.shxzukj.cn

[U93] JS：模板字符串
来源：http://cg.521024.cn

`共 ${n} 条`
来源：http://av.shtwfgs.cn

[U94] JS：箭头函数
来源：http://aq.521024.cn

const double = x => x * 2;
来源：http://hz.lnxyls.cn

[U95] JS：Promise 包装
来源：http://pi.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://gf.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://sz.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jt.shxzskj.cn

[U97] JS：并发请求
来源：http://zs.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ec.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://fs.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fo.hahajie.cn

[U99] JS：事件监听
来源：http://md.hahajie.cn

el.addEventListener("click", e => {})
来源：http://kw.shxzukj.cn

[U100] JS：DOM 查询
来源：http://ru.yuexingan06.cn

document.querySelector(".item")
来源：http://td.nszjky.cn

[U101] JS：classList 操作
来源：http://xv.gzmigu.cn

el.classList.toggle("active")
来源：http://fv.521024.cn

[U102] JS：本地存储
来源：http://lk.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kz.szxytkj.cn

[U103] JS：定时器
来源：http://ua.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bf.bjjhwx.cn

[U104] JS：防抖
来源：http://zf.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nc.colortex.cn

[U105] JS：节流
来源：http://il.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yf.shxzukj.cn

[U106] JS：日期格式化
来源：http://re.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lc.newstarts.cn

[U107] JS：数字千分位
来源：http://cm.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tr.szsharing.cn

[U108] JS：随机整数
来源：http://ug.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bb.asd995.cn

[U109] JS：数组分组
来源：http://tr.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://it.nicolike.cn

[U110] JS：数组分块
来源：http://dv.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ql.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://og.gzmigu.cn

new Map(Object.entries(obj))
来源：http://cd.yuexingan06.cn

[U112] JS：字符串补位
来源：http://lf.nszjky.cn

"7".padStart(3, "0")
来源：http://qa.newstarts.cn

[U113] JS：正则替换全部
来源：http://gm.gzmigu.cn

s.replaceAll("a", "b")
来源：http://hf.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://kv.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wf.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://lt.huixiangedu.cn

crypto.randomUUID()
来源：http://gi.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://tt.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://mv.yuexingan06.cn

[U117] JS：单元测试
来源：http://cp.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://zy.panjiajie.cn

[U118] JS：开发服务器
来源：http://sa.gzmigu.cn

npm i -D vite;  npx vite
来源：http://so.asd995.cn

[U119] JS：生产构建
来源：http://dr.nszjky.cn

npx vite build
来源：http://jl.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ck.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://yn.nicolike.cn

================================================================================
来源：http://ta.chemitech.net.cn

统计汇总
来源：http://pv.yuntaijiaju.cn

================================================================================
来源：http://lj.521024.cn

按语言统计（条）：
来源：http://bp.bookmarksfly.cn

Python ......... 252
来源：http://yd.bookmarksfly.cn

PHP ............ 252
来源：http://dv.asd995.cn

JavaScript ..... 252
来源：http://th.shxzukj.cn

TypeScript ..... 212
来源：http://ie.yuexingan06.cn

Java ........... 212
来源：http://de.bjjhwx.cn

Go ............. 212
来源：http://ty.yuntaijiaju.cn

Ruby ........... 212
来源：http://ws.colortex.cn

C# ............. 212
来源：http://hg.bookmarksfly.cn

C .............. 30
来源：http://sx.asd995.cn

C++ ............ 30
来源：http://fz.nszjky.cn

SQL ............ 90
来源：http://hk.gzmigu.cn

Bash ........... 80
来源：http://iq.521024.cn

Kotlin ......... 15
来源：http://te.nicolike.cn

Swift .......... 15
来源：http://rj.nszjky.cn

Lua ............ 10
来源：http://im.bookmarksfly.cn

Perl ........... 10
来源：http://kx.yuntaijiaju.cn

Scala .......... 10
来源：http://ml.panjiajie.cn

------------------------------------
来源：http://qt.colortex.cn

合计 ........... 2106 条
来源：http://ko.huixiangedu.cn

按章节统计：
来源：http://yd.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rp.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xg.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lw.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mf.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://co.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://km.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wo.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rt.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dx.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nj.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yl.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kd.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jq.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dh.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tm.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uj.szsharing.cn

Q SQL 专题                              90
来源：http://jw.huanxung.cn

R Bash 专题                             80
来源：http://bx.521024.cn

S C / C++ 专题                          60
来源：http://iv.huanxung.cn

T 其他语言补充                          60
来源：http://gw.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://db.nszjky.cn

------------------------------------
来源：http://vv.shxzskj.cn

合计                                  2106 条
来源：http://id.newstarts.cn

--------------------------------------------------------------------------------
来源：http://sw.huixiangedu.cn

使用提醒
来源：http://hd.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://dt.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ou.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kp.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://we.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://od.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ka.nszjky.cn

—— 文件结束 ——
来源：http://fj.nszjky.cn

================================================================================
来源：http://gk.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://dy.nicolike.cn

Common Programming Examples Cheat Book
来源：http://rk.shxzukj.cn

================================================================================
来源：http://xz.huixinmuqiang.cn

【收录内容】
来源：http://iv.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://in.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tu.gzmigu.cn

SQL · Bash · C · C++
来源：http://ev.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://js.haigaiapp.cn

【使用说明】
来源：http://aa.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zh.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ni.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://um.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fg.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tn.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lr.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vb.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yu.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vh.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rp.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zj.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ko.gzmigu.cn

【文件统计】
来源：http://ze.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ac.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://qm.huixiangedu.cn

目  录
来源：http://ex.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ez.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yj.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xy.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hx.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hg.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yo.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hj.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fq.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ew.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tn.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ux.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bq.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hr.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://to.huixiangedu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lr.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qe.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ip.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dd.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xk.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mn.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tz.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zp.wgjwhj.cn

================================================================================
来源：http://xa.panjiajie.cn

A. 基础语法与类型
来源：http://ze.nszjky.cn

================================================================================
来源：http://en.gzmigu.cn

[A01] Hello World
来源：http://mq.nicolike.cn

Py:   print("Hello, World!")
来源：http://oz.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://jr.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://le.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uo.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://hd.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://qz.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://zo.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ws.gzmigu.cn

[A02] 变量声明与赋值
来源：http://hj.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qg.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tz.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yy.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ug.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://ih.521024.cn

Go:   name := "Alex"; age := 20
来源：http://pl.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://dq.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ls.bjjhwx.cn

[A03] 常量定义
来源：http://ng.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wh.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://qg.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://mb.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://ll.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://gq.newstarts.cn

Go:   const PI = 3.14159
来源：http://du.lnxyls.cn

Ruby: PI = 3.14159
来源：http://dz.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://kw.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://vh.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xz.muxihuayi.cn


<!-- 参考信息 -->