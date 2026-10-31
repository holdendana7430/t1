代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://qm.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tm.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://xy.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qx.9csxet.cn

[U43] PHP：声明命名空间
来源：http://oj.nicolike.cn

namespace App\Http;
来源：http://so.521024.cn

[U44] PHP：开启严格类型
来源：http://mk.szsharing.cn

declare(strict_types=1);
来源：http://ku.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://zb.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gk.9csxet.cn

[U46] PHP：可空类型
来源：http://ji.wgjwhj.cn

?string $name = null
来源：http://dj.jctech888.com.cn

[U47] PHP：联合类型
来源：http://zk.hahajie.cn

int|string $id
来源：http://po.gzmigu.cn

[U48] PHP：纯枚举
来源：http://hi.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ht.haigaiapp.cn

[U49] PHP：只读属性
来源：http://dr.bjjhwx.cn

public readonly string $name
来源：http://fg.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://od.hnjuh.cn

public function __construct(private int $id) {}
来源：http://rp.hahajie.cn

[U51] PHP：数组解构
来源：http://vb.chemitech.net.cn

[$a, $b] = $arr;
来源：http://qp.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://cj.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://xp.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://eg.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://us.newstarts.cn

[U54] PHP：空安全调用
来源：http://oe.9csxet.cn

$obj?->method()
来源：http://vx.asd995.cn

[U55] PHP：match 表达式
来源：http://us.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bf.huixiangedu.cn

[U56] PHP：命名参数
来源：http://hj.chemitech.net.cn

f(a: 1, b: 2)
来源：http://mr.shxzukj.cn

[U57] PHP：字符串插值
来源：http://ac.chemitech.net.cn

"值: {$a}"
来源：http://na.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://ah.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lz.szsharing.cn

[U59] PHP：自定义排序
来源：http://pi.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mk.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://il.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xm.muxihuayi.cn

[U61] PHP：正则
来源：http://ln.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bg.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://bq.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://au.shxzskj.cn

[U63] PHP：文件读写
来源：http://mx.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gh.colortex.cn

[U64] PHP：目录遍历
来源：http://ru.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://xk.shxzukj.cn

[U65] PHP：会话
来源：http://ia.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://za.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://vt.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ck.colortex.cn

[U67] PHP：处理文件上传
来源：http://vs.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sp.colortex.cn

[U68] PHP：PDO 连接
来源：http://ma.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://us.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://ak.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vq.huanxung.cn

[U70] PHP：PDO 事务
来源：http://ky.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hr.521024.cn

[U71] PHP：抛出异常
来源：http://un.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://wq.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://xk.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://jf.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://fi.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://sv.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://yx.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://yh.huanxung.cn

[U75] PHP：依赖注入
来源：http://so.panjiajie.cn

composer require psr/container
来源：http://hx.newstarts.cn

[U76] PHP：简单路由
来源：http://uh.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sk.shxzukj.cn

[U77] PHP：模板渲染
来源：http://ls.szsharing.cn

composer require twig/twig
来源：http://hv.haigaiapp.cn

[U78] PHP：单元测试
来源：http://eu.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://uw.haigaiapp.cn

[U79] PHP：静态分析
来源：http://gl.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://lh.szsharing.cn

[U80] PHP：代码规范修复
来源：http://bs.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wz.gzmigu.cn

[U81] JS：初始化项目
来源：http://mq.gzmigu.cn

npm init -y;  npm i express
来源：http://lx.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://ei.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wa.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://ht.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ld.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://ap.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nf.gzmigu.cn

[U85] JS：可选链
来源：http://qd.szxytkj.cn

a?.b?.c
来源：http://sv.panjiajie.cn

[U86] JS：空值合并
来源：http://mw.lnxyls.cn

a ?? b
来源：http://gp.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://re.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://cd.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://tj.hahajie.cn

{ ...a, ...b }
来源：http://qd.nicolike.cn

[U89] JS：数组去重
来源：http://ah.colortex.cn

[...new Set(arr)]
来源：http://id.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://ib.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://yu.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://th.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lc.shtwfgs.cn

[U92] JS：深拷贝
来源：http://cq.bookmarksfly.cn

structuredClone(obj)
来源：http://qm.lnxyls.cn

[U93] JS：模板字符串
来源：http://qq.asd995.cn

`共 ${n} 条`
来源：http://df.muxihuayi.cn

[U94] JS：箭头函数
来源：http://lw.yuntaijiaju.cn

const double = x => x * 2;
来源：http://in.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://wz.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://hv.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://rl.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yq.nicolike.cn

[U97] JS：并发请求
来源：http://hs.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xh.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://rv.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rd.shxzskj.cn

[U99] JS：事件监听
来源：http://fc.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://rz.nszjky.cn

[U100] JS：DOM 查询
来源：http://hx.hahajie.cn

document.querySelector(".item")
来源：http://pg.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://vd.nicolike.cn

el.classList.toggle("active")
来源：http://wj.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://ds.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cj.jctech888.com.cn

[U103] JS：定时器
来源：http://ol.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rq.panjiajie.cn

[U104] JS：防抖
来源：http://cz.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cu.jianghongdianzi.cn

[U105] JS：节流
来源：http://kk.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nr.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://an.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yb.gzmigu.cn

[U107] JS：数字千分位
来源：http://lv.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xs.szxytkj.cn

[U108] JS：随机整数
来源：http://cl.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dp.shtwfgs.cn

[U109] JS：数组分组
来源：http://il.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://ff.muxihuayi.cn

[U110] JS：数组分块
来源：http://ik.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ko.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://pa.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://io.asd995.cn

[U112] JS：字符串补位
来源：http://hp.bjjhwx.cn

"7".padStart(3, "0")
来源：http://hf.9csxet.cn

[U113] JS：正则替换全部
来源：http://mm.521024.cn

s.replaceAll("a", "b")
来源：http://my.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://rj.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jh.colortex.cn

[U115] JS：生成 UUID
来源：http://rz.yuexingan06.cn

crypto.randomUUID()
来源：http://ex.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ad.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://qr.newstarts.cn

[U117] JS：单元测试
来源：http://ye.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://el.hahajie.cn

[U118] JS：开发服务器
来源：http://aa.shxzskj.cn

npm i -D vite;  npx vite
来源：http://ma.shxzskj.cn

[U119] JS：生产构建
来源：http://tj.jctech888.com.cn

npx vite build
来源：http://cp.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://ac.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://nk.yuntaijiaju.cn

================================================================================
来源：http://jc.colortex.cn

统计汇总
来源：http://or.bjjhwx.cn

================================================================================
来源：http://kl.colortex.cn

按语言统计（条）：
来源：http://by.bookmarksfly.cn

Python ......... 252
来源：http://zg.nicolike.cn

PHP ............ 252
来源：http://zy.asd995.cn

JavaScript ..... 252
来源：http://eh.jctech888.com.cn

TypeScript ..... 212
来源：http://ab.wgjwhj.cn

Java ........... 212
来源：http://gu.bjjhwx.cn

Go ............. 212
来源：http://zs.panjiajie.cn

Ruby ........... 212
来源：http://ih.szsharing.cn

C# ............. 212
来源：http://wn.yuexingan06.cn

C .............. 30
来源：http://zk.yuntaijiaju.cn

C++ ............ 30
来源：http://hw.huanxung.cn

SQL ............ 90
来源：http://or.nicolike.cn

Bash ........... 80
来源：http://ff.asd995.cn

Kotlin ......... 15
来源：http://uc.521024.cn

Swift .......... 15
来源：http://rk.hnjuh.cn

Lua ............ 10
来源：http://us.bookmarksfly.cn

Perl ........... 10
来源：http://zk.bjjhwx.cn

Scala .......... 10
来源：http://ke.nicolike.cn

------------------------------------
来源：http://rn.chemitech.net.cn

合计 ........... 2106 条
来源：http://ml.nszjky.cn

按章节统计：
来源：http://jb.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ox.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cq.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jo.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kb.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://br.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eb.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qa.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wj.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ju.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ky.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tb.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xs.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zx.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mk.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hn.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tl.asd995.cn

Q SQL 专题                              90
来源：http://ed.hnjuh.cn

R Bash 专题                             80
来源：http://uf.jctech888.com.cn

S C / C++ 专题                          60
来源：http://tf.szsharing.cn

T 其他语言补充                          60
来源：http://ya.hahajie.cn

U 高频实用片段                         120
来源：http://xm.panjiajie.cn

------------------------------------
来源：http://pt.huixiangedu.cn

合计                                  2106 条
来源：http://lq.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://kk.yuntaijiaju.cn

使用提醒
来源：http://un.asd995.cn

--------------------------------------------------------------------------------
来源：http://vo.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ex.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vf.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gu.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ck.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bd.9csxet.cn

—— 文件结束 ——
来源：http://hi.nszjky.cn

================================================================================
来源：http://bh.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://kn.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://iy.colortex.cn

================================================================================
来源：http://js.shxzukj.cn

【收录内容】
来源：http://ud.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tt.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pm.shxzukj.cn

SQL · Bash · C · C++
来源：http://ot.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yx.huixinmuqiang.cn

【使用说明】
来源：http://dy.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qr.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://we.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qi.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://de.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sz.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uf.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://br.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ql.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vo.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wz.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nw.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yv.hnjuh.cn

【文件统计】
来源：http://vj.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xm.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ac.colortex.cn

目  录
来源：http://hu.nszjky.cn

--------------------------------------------------------------------------------
来源：http://ua.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vv.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://by.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://el.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qq.jianghongdianzi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://py.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://td.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wq.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bx.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ob.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://do.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hl.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bo.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xw.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ve.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bg.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ok.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yg.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qh.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yr.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bd.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vc.asd995.cn

================================================================================
来源：http://oi.huixiangedu.cn

A. 基础语法与类型
来源：http://vj.wgjwhj.cn

================================================================================
来源：http://bv.szxytkj.cn

[A01] Hello World
来源：http://ia.szsharing.cn

Py:   print("Hello, World!")
来源：http://vu.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://so.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://cw.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hg.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://sf.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://iw.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://bs.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fa.huanxung.cn

[A02] 变量声明与赋值
来源：http://lp.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ym.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kw.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yv.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gq.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://lg.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://fv.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://ti.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fv.gzmigu.cn

[A03] 常量定义
来源：http://ir.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mq.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://pz.newstarts.cn

JS:   const PI = 3.14159;
来源：http://wg.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://tz.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://eh.asd995.cn

Go:   const PI = 3.14159
来源：http://hf.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://xe.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://ho.nicolike.cn

[A04] 判断变量类型
来源：http://fm.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tn.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gy.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fh.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://oa.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ye.nszjky.cn


<!-- 参考信息 -->