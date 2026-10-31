代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://vr.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zb.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://lx.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://su.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://ra.521024.cn

namespace App\Http;
来源：http://gj.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://dv.wgjwhj.cn

declare(strict_types=1);
来源：http://uk.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://om.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://el.lnxyls.cn

[U46] PHP：可空类型
来源：http://wo.chemitech.net.cn

?string $name = null
来源：http://ne.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://uk.muxihuayi.cn

int|string $id
来源：http://kq.hnjuh.cn

[U48] PHP：纯枚举
来源：http://pg.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://de.shxzskj.cn

[U49] PHP：只读属性
来源：http://qe.nszjky.cn

public readonly string $name
来源：http://bn.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://zz.colortex.cn

public function __construct(private int $id) {}
来源：http://yg.bjjhwx.cn

[U51] PHP：数组解构
来源：http://oq.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://tn.newstarts.cn

[U52] PHP：箭头函数
来源：http://ie.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://as.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://em.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://hi.szsharing.cn

[U54] PHP：空安全调用
来源：http://bi.yuntaijiaju.cn

$obj?->method()
来源：http://vs.shxzukj.cn

[U55] PHP：match 表达式
来源：http://en.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zr.szxytkj.cn

[U56] PHP：命名参数
来源：http://zc.hahajie.cn

f(a: 1, b: 2)
来源：http://gy.szsharing.cn

[U57] PHP：字符串插值
来源：http://ld.shxzukj.cn

"值: {$a}"
来源：http://sq.gzmigu.cn

[U58] PHP：数组三件套
来源：http://sk.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pj.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://ha.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bc.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://rj.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ig.lnxyls.cn

[U61] PHP：正则
来源：http://yn.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ws.yuexingan06.cn

[U62] PHP：日期对象
来源：http://of.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xk.shxzskj.cn

[U63] PHP：文件读写
来源：http://yk.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mn.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://wc.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://kl.lnxyls.cn

[U65] PHP：会话
来源：http://tv.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qk.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://aw.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gh.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://eu.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ij.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://tc.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yg.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://dj.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jt.521024.cn

[U70] PHP：PDO 事务
来源：http://nb.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xg.hahajie.cn

[U71] PHP：抛出异常
来源：http://dj.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://iv.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://lj.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://km.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://rx.asd995.cn

parse_ini_file("config.ini", true)
来源：http://he.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://qz.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://vk.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://bt.jctech888.com.cn

composer require psr/container
来源：http://gt.shtwfgs.cn

[U76] PHP：简单路由
来源：http://ij.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jh.shxzukj.cn

[U77] PHP：模板渲染
来源：http://yo.bjjhwx.cn

composer require twig/twig
来源：http://ov.haigaiapp.cn

[U78] PHP：单元测试
来源：http://rx.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://hb.hahajie.cn

[U79] PHP：静态分析
来源：http://og.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://fj.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://dr.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ro.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://mq.lnxyls.cn

npm init -y;  npm i express
来源：http://yh.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://wk.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jj.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://bm.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aw.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://dz.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ly.bookmarksfly.cn

[U85] JS：可选链
来源：http://mv.panjiajie.cn

a?.b?.c
来源：http://mq.521024.cn

[U86] JS：空值合并
来源：http://cc.szxytkj.cn

a ?? b
来源：http://kh.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://td.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://ol.szxytkj.cn

[U88] JS：对象展开合并
来源：http://jw.jctech888.com.cn

{ ...a, ...b }
来源：http://gr.huanxung.cn

[U89] JS：数组去重
来源：http://em.szxytkj.cn

[...new Set(arr)]
来源：http://wg.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://cn.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://to.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://tz.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dq.muxihuayi.cn

[U92] JS：深拷贝
来源：http://zl.shxzukj.cn

structuredClone(obj)
来源：http://uv.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://vz.nicolike.cn

`共 ${n} 条`
来源：http://pi.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://ux.bookmarksfly.cn

const double = x => x * 2;
来源：http://sn.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://xv.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://en.9csxet.cn

[U96] JS：async/await 与异常
来源：http://xi.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vo.shtwfgs.cn

[U97] JS：并发请求
来源：http://sx.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bk.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://nc.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rh.colortex.cn

[U99] JS：事件监听
来源：http://eb.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://gd.newstarts.cn

[U100] JS：DOM 查询
来源：http://de.hnjuh.cn

document.querySelector(".item")
来源：http://zm.nicolike.cn

[U101] JS：classList 操作
来源：http://xu.hahajie.cn

el.classList.toggle("active")
来源：http://gs.jctech888.com.cn

[U102] JS：本地存储
来源：http://ym.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://js.hahajie.cn

[U103] JS：定时器
来源：http://nc.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nb.colortex.cn

[U104] JS：防抖
来源：http://ve.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://od.bookmarksfly.cn

[U105] JS：节流
来源：http://ex.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ua.jctech888.com.cn

[U106] JS：日期格式化
来源：http://cr.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://re.panjiajie.cn

[U107] JS：数字千分位
来源：http://br.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yf.gzmigu.cn

[U108] JS：随机整数
来源：http://bl.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ur.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://ar.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://ns.huixiangedu.cn

[U110] JS：数组分块
来源：http://jc.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gp.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://ae.nszjky.cn

new Map(Object.entries(obj))
来源：http://lr.chemitech.net.cn

[U112] JS：字符串补位
来源：http://hk.9csxet.cn

"7".padStart(3, "0")
来源：http://he.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://rh.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://ne.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://tz.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qu.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://zw.hnjuh.cn

crypto.randomUUID()
来源：http://de.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://ns.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://tk.panjiajie.cn

[U117] JS：单元测试
来源：http://kh.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://ba.nicolike.cn

[U118] JS：开发服务器
来源：http://sy.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://vq.szsharing.cn

[U119] JS：生产构建
来源：http://qm.nszjky.cn

npx vite build
来源：http://di.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://so.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://sh.shxzskj.cn

================================================================================
来源：http://zi.shxzukj.cn

统计汇总
来源：http://it.huixiangedu.cn

================================================================================
来源：http://dj.bookmarksfly.cn

按语言统计（条）：
来源：http://hk.jianghongdianzi.cn

Python ......... 252
来源：http://mm.yuexingan06.cn

PHP ............ 252
来源：http://lc.szxytkj.cn

JavaScript ..... 252
来源：http://ew.huixinmuqiang.cn

TypeScript ..... 212
来源：http://mo.colortex.cn

Java ........... 212
来源：http://mq.haigaiapp.cn

Go ............. 212
来源：http://ec.jianghongdianzi.cn

Ruby ........... 212
来源：http://ky.nicolike.cn

C# ............. 212
来源：http://zs.yuexingan06.cn

C .............. 30
来源：http://nx.nicolike.cn

C++ ............ 30
来源：http://qc.asd995.cn

SQL ............ 90
来源：http://rh.bookmarksfly.cn

Bash ........... 80
来源：http://bl.gzmigu.cn

Kotlin ......... 15
来源：http://ra.gzmigu.cn

Swift .......... 15
来源：http://tg.yuexingan06.cn

Lua ............ 10
来源：http://gi.muxihuayi.cn

Perl ........... 10
来源：http://it.jianghongdianzi.cn

Scala .......... 10
来源：http://ab.shxzukj.cn

------------------------------------
来源：http://jo.newstarts.cn

合计 ........... 2106 条
来源：http://ia.haigaiapp.cn

按章节统计：
来源：http://ao.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rf.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sn.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tm.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sp.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bs.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ds.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lj.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wz.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://np.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ou.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sg.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ff.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rj.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fb.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eu.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dj.9csxet.cn

Q SQL 专题                              90
来源：http://te.jctech888.com.cn

R Bash 专题                             80
来源：http://ie.nicolike.cn

S C / C++ 专题                          60
来源：http://xy.shxzukj.cn

T 其他语言补充                          60
来源：http://xo.shxzukj.cn

U 高频实用片段                         120
来源：http://gu.huixinmuqiang.cn

------------------------------------
来源：http://bt.colortex.cn

合计                                  2106 条
来源：http://gw.9csxet.cn

--------------------------------------------------------------------------------
来源：http://al.nszjky.cn

使用提醒
来源：http://jy.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://dh.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tc.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://um.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qn.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cg.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yj.lnxyls.cn

—— 文件结束 ——
来源：http://hh.szsharing.cn

================================================================================
来源：http://uq.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://ta.newstarts.cn

Common Programming Examples Cheat Book
来源：http://rf.shtwfgs.cn

================================================================================
来源：http://mv.gzmigu.cn

【收录内容】
来源：http://pb.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wk.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zh.shxzukj.cn

SQL · Bash · C · C++
来源：http://zn.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pi.9csxet.cn

【使用说明】
来源：http://ni.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zu.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tp.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yq.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lg.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://df.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uc.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ex.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xd.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lm.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fb.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://al.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gc.yuexingan06.cn

【文件统计】
来源：http://lc.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nw.521024.cn

--------------------------------------------------------------------------------
来源：http://fy.panjiajie.cn

目  录
来源：http://jy.colortex.cn

--------------------------------------------------------------------------------
来源：http://yw.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cs.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uh.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rj.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xx.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sj.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rr.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qb.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dl.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://la.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iv.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vf.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wn.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://po.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rc.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qu.haigaiapp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pe.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kn.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wt.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zn.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xp.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ik.shtwfgs.cn

================================================================================
来源：http://zl.chemitech.net.cn

A. 基础语法与类型
来源：http://ez.newstarts.cn

================================================================================
来源：http://dl.szxytkj.cn

[A01] Hello World
来源：http://lo.newstarts.cn

Py:   print("Hello, World!")
来源：http://rn.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://qy.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://tq.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wg.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://xj.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://dk.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://uz.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dn.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://go.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gh.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ts.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://py.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xb.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://pz.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://bc.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://ad.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fy.521024.cn

[A03] 常量定义
来源：http://vc.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://du.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://pg.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://hk.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://py.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://ri.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://my.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://sa.colortex.cn

C#:   const double PI = 3.14159;
来源：http://dz.szsharing.cn

[A04] 判断变量类型
来源：http://yi.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vd.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sx.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bd.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://ab.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tl.nszjky.cn


<!-- 参考信息 -->