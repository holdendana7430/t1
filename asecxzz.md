代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://dh.szsharing.cn

sys.stdout.isatty()
来源：http://ot.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://lg.9csxet.cn

print("err", file=sys.stderr)
来源：http://yn.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://nc.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ku.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://pz.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lq.colortex.cn

[U43] PHP：声明命名空间
来源：http://kp.lnxyls.cn

namespace App\Http;
来源：http://vg.szsharing.cn

[U44] PHP：开启严格类型
来源：http://gs.haigaiapp.cn

declare(strict_types=1);
来源：http://hh.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://ja.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://do.asd995.cn

[U46] PHP：可空类型
来源：http://cr.asd995.cn

?string $name = null
来源：http://ri.shtwfgs.cn

[U47] PHP：联合类型
来源：http://yz.nicolike.cn

int|string $id
来源：http://an.hahajie.cn

[U48] PHP：纯枚举
来源：http://tp.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vh.panjiajie.cn

[U49] PHP：只读属性
来源：http://mk.muxihuayi.cn

public readonly string $name
来源：http://wk.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://xt.newstarts.cn

public function __construct(private int $id) {}
来源：http://zi.huanxung.cn

[U51] PHP：数组解构
来源：http://gj.lnxyls.cn

[$a, $b] = $arr;
来源：http://lg.szsharing.cn

[U52] PHP：箭头函数
来源：http://ua.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://sw.hahajie.cn

[U53] PHP：空合并运算符
来源：http://zv.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://xd.lnxyls.cn

[U54] PHP：空安全调用
来源：http://fe.hnjuh.cn

$obj?->method()
来源：http://be.szsharing.cn

[U55] PHP：match 表达式
来源：http://hn.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rm.szsharing.cn

[U56] PHP：命名参数
来源：http://qi.shxzskj.cn

f(a: 1, b: 2)
来源：http://tm.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://gp.jianghongdianzi.cn

"值: {$a}"
来源：http://me.gzmigu.cn

[U58] PHP：数组三件套
来源：http://oi.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wq.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://ii.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ho.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://jx.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xu.hnjuh.cn

[U61] PHP：正则
来源：http://aa.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mg.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://pl.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ni.szsharing.cn

[U63] PHP：文件读写
来源：http://yx.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yg.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://yb.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://va.jctech888.com.cn

[U65] PHP：会话
来源：http://ev.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ns.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://et.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cx.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://ub.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ri.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://kw.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cl.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://ul.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://if.szsharing.cn

[U70] PHP：PDO 事务
来源：http://df.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uf.shxzukj.cn

[U71] PHP：抛出异常
来源：http://vk.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://og.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://mp.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://ro.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://va.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://jt.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://pa.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://vr.panjiajie.cn

[U75] PHP：依赖注入
来源：http://yd.hnjuh.cn

composer require psr/container
来源：http://fb.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://ox.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fb.hahajie.cn

[U77] PHP：模板渲染
来源：http://pk.wgjwhj.cn

composer require twig/twig
来源：http://yr.szxytkj.cn

[U78] PHP：单元测试
来源：http://jg.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://qt.hnjuh.cn

[U79] PHP：静态分析
来源：http://wz.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://xu.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://jp.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cr.asd995.cn

[U81] JS：初始化项目
来源：http://ui.shxzukj.cn

npm init -y;  npm i express
来源：http://jj.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://lz.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ec.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://bg.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yo.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://fr.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qb.szsharing.cn

[U85] JS：可选链
来源：http://am.jianghongdianzi.cn

a?.b?.c
来源：http://ns.shxzukj.cn

[U86] JS：空值合并
来源：http://fs.panjiajie.cn

a ?? b
来源：http://nl.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://qi.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://ae.hahajie.cn

[U88] JS：对象展开合并
来源：http://bd.szsharing.cn

{ ...a, ...b }
来源：http://ih.gzmigu.cn

[U89] JS：数组去重
来源：http://xv.bookmarksfly.cn

[...new Set(arr)]
来源：http://eb.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://tw.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://zu.asd995.cn

[U91] JS：对象键值遍历
来源：http://aa.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bn.jctech888.com.cn

[U92] JS：深拷贝
来源：http://rx.chemitech.net.cn

structuredClone(obj)
来源：http://wq.colortex.cn

[U93] JS：模板字符串
来源：http://lg.huanxung.cn

`共 ${n} 条`
来源：http://hb.muxihuayi.cn

[U94] JS：箭头函数
来源：http://li.9csxet.cn

const double = x => x * 2;
来源：http://nh.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://id.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://ky.521024.cn

[U96] JS：async/await 与异常
来源：http://ex.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jz.huixiangedu.cn

[U97] JS：并发请求
来源：http://jx.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eu.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://zm.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lq.lnxyls.cn

[U99] JS：事件监听
来源：http://uy.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://wa.panjiajie.cn

[U100] JS：DOM 查询
来源：http://ia.huixiangedu.cn

document.querySelector(".item")
来源：http://ux.wgjwhj.cn

[U101] JS：classList 操作
来源：http://ii.wgjwhj.cn

el.classList.toggle("active")
来源：http://em.huixiangedu.cn

[U102] JS：本地存储
来源：http://lh.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zl.chemitech.net.cn

[U103] JS：定时器
来源：http://ug.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kq.hnjuh.cn

[U104] JS：防抖
来源：http://fj.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ar.newstarts.cn

[U105] JS：节流
来源：http://sq.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aw.haigaiapp.cn

[U106] JS：日期格式化
来源：http://og.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nm.szsharing.cn

[U107] JS：数字千分位
来源：http://nx.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ck.huixiangedu.cn

[U108] JS：随机整数
来源：http://sd.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sv.gzmigu.cn

[U109] JS：数组分组
来源：http://bj.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://ml.muxihuayi.cn

[U110] JS：数组分块
来源：http://ik.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ge.gzmigu.cn

[U111] JS：对象转 Map
来源：http://mc.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://gt.9csxet.cn

[U112] JS：字符串补位
来源：http://ud.panjiajie.cn

"7".padStart(3, "0")
来源：http://sp.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://rs.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://vr.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://zm.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mx.szsharing.cn

[U115] JS：生成 UUID
来源：http://dn.9csxet.cn

crypto.randomUUID()
来源：http://ly.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://to.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://ri.shxzukj.cn

[U117] JS：单元测试
来源：http://rz.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://gu.shxzukj.cn

[U118] JS：开发服务器
来源：http://pq.hahajie.cn

npm i -D vite;  npx vite
来源：http://kz.asd995.cn

[U119] JS：生产构建
来源：http://nt.huixiangedu.cn

npx vite build
来源：http://fo.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://me.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://dd.shxzukj.cn

================================================================================
来源：http://qn.nicolike.cn

统计汇总
来源：http://df.colortex.cn

================================================================================
来源：http://zc.shxzukj.cn

按语言统计（条）：
来源：http://kn.9csxet.cn

Python ......... 252
来源：http://gl.panjiajie.cn

PHP ............ 252
来源：http://rv.panjiajie.cn

JavaScript ..... 252
来源：http://ud.muxihuayi.cn

TypeScript ..... 212
来源：http://gs.shxzukj.cn

Java ........... 212
来源：http://yi.huixiangedu.cn

Go ............. 212
来源：http://rf.hahajie.cn

Ruby ........... 212
来源：http://yx.shxzskj.cn

C# ............. 212
来源：http://aw.hnjuh.cn

C .............. 30
来源：http://fr.lnxyls.cn

C++ ............ 30
来源：http://yd.shxzskj.cn

SQL ............ 90
来源：http://hp.shxzskj.cn

Bash ........... 80
来源：http://wd.asd995.cn

Kotlin ......... 15
来源：http://bb.bjjhwx.cn

Swift .......... 15
来源：http://nd.szxytkj.cn

Lua ............ 10
来源：http://xt.panjiajie.cn

Perl ........... 10
来源：http://ex.jianghongdianzi.cn

Scala .......... 10
来源：http://rc.hahajie.cn

------------------------------------
来源：http://yg.haigaiapp.cn

合计 ........... 2106 条
来源：http://sp.wgjwhj.cn

按章节统计：
来源：http://oa.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vx.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gl.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://no.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ts.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ub.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ay.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uu.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dp.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dn.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qz.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ds.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lz.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tt.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ho.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fw.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lt.shtwfgs.cn

Q SQL 专题                              90
来源：http://nr.9csxet.cn

R Bash 专题                             80
来源：http://rb.chemitech.net.cn

S C / C++ 专题                          60
来源：http://vs.chemitech.net.cn

T 其他语言补充                          60
来源：http://yd.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://cu.colortex.cn

------------------------------------
来源：http://nd.bjjhwx.cn

合计                                  2106 条
来源：http://ea.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://wo.jianghongdianzi.cn

使用提醒
来源：http://kj.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zy.shxzukj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ak.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rh.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yl.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pu.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sm.shtwfgs.cn

—— 文件结束 ——
来源：http://pa.hahajie.cn

================================================================================
来源：http://oe.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://wx.9csxet.cn

Common Programming Examples Cheat Book
来源：http://lm.jctech888.com.cn

================================================================================
来源：http://bf.colortex.cn

【收录内容】
来源：http://uc.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wa.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qr.lnxyls.cn

SQL · Bash · C · C++
来源：http://un.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fu.nszjky.cn

【使用说明】
来源：http://ru.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ge.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wr.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ym.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lw.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sn.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jt.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lk.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mi.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nq.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sb.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://us.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ke.wgjwhj.cn

【文件统计】
来源：http://of.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wf.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ee.panjiajie.cn

目  录
来源：http://gr.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://vg.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://er.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yr.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cv.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://je.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fv.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mc.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zv.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bl.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xv.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://af.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rw.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://av.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wm.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ga.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gy.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hc.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vg.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wu.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rp.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lr.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ym.gzmigu.cn

================================================================================
来源：http://dj.muxihuayi.cn

A. 基础语法与类型
来源：http://hj.hahajie.cn

================================================================================
来源：http://rq.9csxet.cn

[A01] Hello World
来源：http://dw.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://sk.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://hw.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://hs.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zr.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://di.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://wq.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://kv.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ok.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://oc.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rd.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qn.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nv.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aw.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://lt.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://ps.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://kk.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kf.bookmarksfly.cn

[A03] 常量定义
来源：http://pn.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iv.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://qa.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://ej.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://gb.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://ju.521024.cn

Go:   const PI = 3.14159
来源：http://yn.newstarts.cn

Ruby: PI = 3.14159
来源：http://bi.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://pb.nszjky.cn

[A04] 判断变量类型
来源：http://xl.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://px.nicolike.cn


<!-- 参考信息 -->