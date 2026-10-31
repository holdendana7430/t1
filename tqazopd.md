代发 wailian999

[U43] PHP：声明命名空间
来源：http://yy.szsharing.cn

namespace App\Http;
来源：http://xx.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://kt.shtwfgs.cn

declare(strict_types=1);
来源：http://dt.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://pr.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tk.9csxet.cn

[U46] PHP：可空类型
来源：http://jl.chemitech.net.cn

?string $name = null
来源：http://ck.shxzukj.cn

[U47] PHP：联合类型
来源：http://rz.huanxung.cn

int|string $id
来源：http://ml.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://ps.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://md.huixiangedu.cn

[U49] PHP：只读属性
来源：http://nr.colortex.cn

public readonly string $name
来源：http://cu.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://zz.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://un.9csxet.cn

[U51] PHP：数组解构
来源：http://rv.nicolike.cn

[$a, $b] = $arr;
来源：http://gq.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://lf.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://ku.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://kb.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://dn.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://pm.bjjhwx.cn

$obj?->method()
来源：http://ie.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://ry.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://re.lnxyls.cn

[U56] PHP：命名参数
来源：http://sr.shxzskj.cn

f(a: 1, b: 2)
来源：http://nc.huanxung.cn

[U57] PHP：字符串插值
来源：http://al.yuntaijiaju.cn

"值: {$a}"
来源：http://pq.newstarts.cn

[U58] PHP：数组三件套
来源：http://fl.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jd.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://oc.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tf.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://nv.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wc.colortex.cn

[U61] PHP：正则
来源：http://yk.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jo.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://ya.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jg.newstarts.cn

[U63] PHP：文件读写
来源：http://zr.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hd.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://eg.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://ay.jianghongdianzi.cn

[U65] PHP：会话
来源：http://zr.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kb.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://wa.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://az.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://xa.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hs.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://rq.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jh.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://kj.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ix.521024.cn

[U70] PHP：PDO 事务
来源：http://cq.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kt.9csxet.cn

[U71] PHP：抛出异常
来源：http://lo.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://wf.szxytkj.cn

[U72] PHP：写错误日志
来源：http://er.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://yg.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://hw.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://wz.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://sp.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://pk.hahajie.cn

[U75] PHP：依赖注入
来源：http://ov.jianghongdianzi.cn

composer require psr/container
来源：http://iv.hnjuh.cn

[U76] PHP：简单路由
来源：http://ui.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fb.lnxyls.cn

[U77] PHP：模板渲染
来源：http://rg.nicolike.cn

composer require twig/twig
来源：http://tk.haigaiapp.cn

[U78] PHP：单元测试
来源：http://vl.colortex.cn

composer require --dev phpunit/phpunit
来源：http://mp.bjjhwx.cn

[U79] PHP：静态分析
来源：http://fl.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://vq.nszjky.cn

[U80] PHP：代码规范修复
来源：http://nc.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nx.asd995.cn

[U81] JS：初始化项目
来源：http://bs.gzmigu.cn

npm init -y;  npm i express
来源：http://wo.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://ra.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fx.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://ja.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://us.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://et.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ri.huixiangedu.cn

[U85] JS：可选链
来源：http://ex.hahajie.cn

a?.b?.c
来源：http://ex.lnxyls.cn

[U86] JS：空值合并
来源：http://ay.gzmigu.cn

a ?? b
来源：http://sz.szsharing.cn

[U87] JS：解构默认值
来源：http://zq.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://hj.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://cf.huanxung.cn

{ ...a, ...b }
来源：http://pt.chemitech.net.cn

[U89] JS：数组去重
来源：http://lp.nszjky.cn

[...new Set(arr)]
来源：http://ku.nszjky.cn

[U90] JS：数字数组排序
来源：http://xa.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://xy.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://gg.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tb.hahajie.cn

[U92] JS：深拷贝
来源：http://qe.hahajie.cn

structuredClone(obj)
来源：http://ob.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://no.yuntaijiaju.cn

`共 ${n} 条`
来源：http://oi.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://cw.bjjhwx.cn

const double = x => x * 2;
来源：http://be.nicolike.cn

[U95] JS：Promise 包装
来源：http://rm.colortex.cn

new Promise((resolve, reject) => {})
来源：http://qx.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://ec.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gz.wgjwhj.cn

[U97] JS：并发请求
来源：http://jk.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wc.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://km.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bl.asd995.cn

[U99] JS：事件监听
来源：http://tr.9csxet.cn

el.addEventListener("click", e => {})
来源：http://um.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://cw.nszjky.cn

document.querySelector(".item")
来源：http://fq.bjjhwx.cn

[U101] JS：classList 操作
来源：http://jm.shxzukj.cn

el.classList.toggle("active")
来源：http://og.nszjky.cn

[U102] JS：本地存储
来源：http://vg.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wk.521024.cn

[U103] JS：定时器
来源：http://qi.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://do.hnjuh.cn

[U104] JS：防抖
来源：http://nm.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jd.huixiangedu.cn

[U105] JS：节流
来源：http://zv.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ww.chemitech.net.cn

[U106] JS：日期格式化
来源：http://nj.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lh.gzmigu.cn

[U107] JS：数字千分位
来源：http://rn.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ko.asd995.cn

[U108] JS：随机整数
来源：http://wf.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ji.shxzskj.cn

[U109] JS：数组分组
来源：http://jh.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://ub.9csxet.cn

[U110] JS：数组分块
来源：http://mm.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ry.9csxet.cn

[U111] JS：对象转 Map
来源：http://oh.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://tn.hnjuh.cn

[U112] JS：字符串补位
来源：http://jw.lnxyls.cn

"7".padStart(3, "0")
来源：http://vz.szsharing.cn

[U113] JS：正则替换全部
来源：http://nd.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://ui.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://jt.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ii.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://ew.nicolike.cn

crypto.randomUUID()
来源：http://wt.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ai.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://ef.shtwfgs.cn

[U117] JS：单元测试
来源：http://ji.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://rl.panjiajie.cn

[U118] JS：开发服务器
来源：http://nx.lnxyls.cn

npm i -D vite;  npx vite
来源：http://yl.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://ia.wgjwhj.cn

npx vite build
来源：http://vq.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ox.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://bc.muxihuayi.cn

================================================================================
来源：http://bn.szsharing.cn

统计汇总
来源：http://gq.panjiajie.cn

================================================================================
来源：http://nm.hahajie.cn

按语言统计（条）：
来源：http://tj.jctech888.com.cn

Python ......... 252
来源：http://cs.chemitech.net.cn

PHP ............ 252
来源：http://zz.huixiangedu.cn

JavaScript ..... 252
来源：http://yr.lnxyls.cn

TypeScript ..... 212
来源：http://hk.bjjhwx.cn

Java ........... 212
来源：http://ty.shxzukj.cn

Go ............. 212
来源：http://he.asd995.cn

Ruby ........... 212
来源：http://em.shxzskj.cn

C# ............. 212
来源：http://au.hnjuh.cn

C .............. 30
来源：http://ma.muxihuayi.cn

C++ ............ 30
来源：http://lg.521024.cn

SQL ............ 90
来源：http://hb.shxzukj.cn

Bash ........... 80
来源：http://rp.asd995.cn

Kotlin ......... 15
来源：http://fu.panjiajie.cn

Swift .......... 15
来源：http://va.lnxyls.cn

Lua ............ 10
来源：http://mx.huixinmuqiang.cn

Perl ........... 10
来源：http://zk.shxzskj.cn

Scala .......... 10
来源：http://jd.huixiangedu.cn

------------------------------------
来源：http://fk.shxzukj.cn

合计 ........... 2106 条
来源：http://gi.colortex.cn

按章节统计：
来源：http://uo.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nm.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wz.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://as.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uz.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ny.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dj.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ie.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xg.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dp.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ax.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pm.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yp.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ml.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aj.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://je.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yq.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://iz.nszjky.cn

R Bash 专题                             80
来源：http://jk.szxytkj.cn

S C / C++ 专题                          60
来源：http://fl.shxzskj.cn

T 其他语言补充                          60
来源：http://ap.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://ub.huixinmuqiang.cn

------------------------------------
来源：http://mf.muxihuayi.cn

合计                                  2106 条
来源：http://gr.szsharing.cn

--------------------------------------------------------------------------------
来源：http://cd.9csxet.cn

使用提醒
来源：http://qq.huanxung.cn

--------------------------------------------------------------------------------
来源：http://no.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iq.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pn.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hp.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zo.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xn.szxytkj.cn

—— 文件结束 ——
来源：http://yv.chemitech.net.cn

================================================================================
来源：http://el.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://dh.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://uf.jianghongdianzi.cn

================================================================================
来源：http://bu.hahajie.cn

【收录内容】
来源：http://jw.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bp.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bh.wgjwhj.cn

SQL · Bash · C · C++
来源：http://cp.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nq.yuntaijiaju.cn

【使用说明】
来源：http://jl.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jw.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nc.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vw.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ve.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wr.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sm.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://al.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sz.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kq.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gv.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ui.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qk.asd995.cn

【文件统计】
来源：http://sl.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qj.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://do.szxytkj.cn

目  录
来源：http://mj.hahajie.cn

--------------------------------------------------------------------------------
来源：http://wy.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gn.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://an.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kx.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pv.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ug.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lc.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zs.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fs.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://km.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rb.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://de.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://co.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mj.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jz.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uv.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nn.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bl.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xr.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jo.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xz.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xx.muxihuayi.cn

================================================================================
来源：http://xs.521024.cn

A. 基础语法与类型
来源：http://lb.521024.cn

================================================================================
来源：http://ik.muxihuayi.cn

[A01] Hello World
来源：http://dl.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://bf.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://eg.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://fz.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fj.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://jw.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://kc.shxzskj.cn

Ruby: puts "Hello, World!"
来源：http://zk.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://le.szsharing.cn

[A02] 变量声明与赋值
来源：http://fw.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fx.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fq.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bs.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://te.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://kz.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://xl.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://st.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dm.szsharing.cn

[A03] 常量定义
来源：http://of.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yz.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://ua.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://um.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://sf.521024.cn

Java: static final double PI = 3.14159;
来源：http://uh.shxzukj.cn

Go:   const PI = 3.14159
来源：http://rv.colortex.cn

Ruby: PI = 3.14159
来源：http://nj.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://pz.huanxung.cn

[A04] 判断变量类型
来源：http://qi.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dv.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ta.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pi.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://du.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yl.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pv.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zh.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://ty.nicolike.cn

[A05] 整数除法与取模
来源：http://vm.hahajie.cn


<!-- 参考信息 -->