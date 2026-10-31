代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://gz.bjjhwx.cn

sys.stdout.isatty()
来源：http://oe.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://of.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://hj.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://fu.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zq.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://gz.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nv.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://ob.colortex.cn

namespace App\Http;
来源：http://wh.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://ai.muxihuayi.cn

declare(strict_types=1);
来源：http://pf.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://ft.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ul.haigaiapp.cn

[U46] PHP：可空类型
来源：http://zm.panjiajie.cn

?string $name = null
来源：http://ld.haigaiapp.cn

[U47] PHP：联合类型
来源：http://tr.nszjky.cn

int|string $id
来源：http://ec.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://uc.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hq.muxihuayi.cn

[U49] PHP：只读属性
来源：http://uo.muxihuayi.cn

public readonly string $name
来源：http://rb.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://jr.panjiajie.cn

public function __construct(private int $id) {}
来源：http://ky.huanxung.cn

[U51] PHP：数组解构
来源：http://bf.newstarts.cn

[$a, $b] = $arr;
来源：http://lx.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://pe.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://nu.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://qw.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://ts.huanxung.cn

[U54] PHP：空安全调用
来源：http://um.yuntaijiaju.cn

$obj?->method()
来源：http://gg.szsharing.cn

[U55] PHP：match 表达式
来源：http://ac.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mh.szsharing.cn

[U56] PHP：命名参数
来源：http://gh.yuexingan06.cn

f(a: 1, b: 2)
来源：http://tj.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://pa.chemitech.net.cn

"值: {$a}"
来源：http://jv.521024.cn

[U58] PHP：数组三件套
来源：http://kl.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ae.shxzukj.cn

[U59] PHP：自定义排序
来源：http://ho.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rh.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://br.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xz.nicolike.cn

[U61] PHP：正则
来源：http://ux.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dx.shxzukj.cn

[U62] PHP：日期对象
来源：http://be.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fr.colortex.cn

[U63] PHP：文件读写
来源：http://vc.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kd.gzmigu.cn

[U64] PHP：目录遍历
来源：http://ai.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://vg.jianghongdianzi.cn

[U65] PHP：会话
来源：http://ym.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nq.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://bq.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eg.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://cn.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vm.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://mp.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://di.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://zm.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sy.asd995.cn

[U70] PHP：PDO 事务
来源：http://da.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fb.9csxet.cn

[U71] PHP：抛出异常
来源：http://td.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://zt.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://jg.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://jc.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://tj.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://qt.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://oj.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://qh.9csxet.cn

[U75] PHP：依赖注入
来源：http://mq.jianghongdianzi.cn

composer require psr/container
来源：http://nt.shxzukj.cn

[U76] PHP：简单路由
来源：http://yf.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vu.szsharing.cn

[U77] PHP：模板渲染
来源：http://sd.newstarts.cn

composer require twig/twig
来源：http://fm.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://rw.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://zi.chemitech.net.cn

[U79] PHP：静态分析
来源：http://rk.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://hp.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://sr.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nh.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://pa.haigaiapp.cn

npm init -y;  npm i express
来源：http://lb.nicolike.cn

[U82] JS：package.json 脚本
来源：http://wp.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zh.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://sk.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zw.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://pp.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vq.asd995.cn

[U85] JS：可选链
来源：http://nr.gzmigu.cn

a?.b?.c
来源：http://we.bookmarksfly.cn

[U86] JS：空值合并
来源：http://tg.huixinmuqiang.cn

a ?? b
来源：http://cm.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://nz.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://co.asd995.cn

[U88] JS：对象展开合并
来源：http://bc.huanxung.cn

{ ...a, ...b }
来源：http://co.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://je.hnjuh.cn

[...new Set(arr)]
来源：http://pu.panjiajie.cn

[U90] JS：数字数组排序
来源：http://iv.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://tn.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://no.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pg.521024.cn

[U92] JS：深拷贝
来源：http://ae.shxzskj.cn

structuredClone(obj)
来源：http://hp.hnjuh.cn

[U93] JS：模板字符串
来源：http://if.521024.cn

`共 ${n} 条`
来源：http://ld.bjjhwx.cn

[U94] JS：箭头函数
来源：http://bm.gzmigu.cn

const double = x => x * 2;
来源：http://aw.asd995.cn

[U95] JS：Promise 包装
来源：http://le.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://zj.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://yb.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ny.9csxet.cn

[U97] JS：并发请求
来源：http://ae.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vo.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://bd.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ze.gzmigu.cn

[U99] JS：事件监听
来源：http://mj.521024.cn

el.addEventListener("click", e => {})
来源：http://gd.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://zc.huixiangedu.cn

document.querySelector(".item")
来源：http://cf.9csxet.cn

[U101] JS：classList 操作
来源：http://pc.bjjhwx.cn

el.classList.toggle("active")
来源：http://he.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://qu.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yf.jianghongdianzi.cn

[U103] JS：定时器
来源：http://no.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yw.bjjhwx.cn

[U104] JS：防抖
来源：http://nl.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xk.colortex.cn

[U105] JS：节流
来源：http://nu.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ao.bjjhwx.cn

[U106] JS：日期格式化
来源：http://eo.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yd.chemitech.net.cn

[U107] JS：数字千分位
来源：http://rx.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mr.jctech888.com.cn

[U108] JS：随机整数
来源：http://kt.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dp.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://bj.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://yg.bjjhwx.cn

[U110] JS：数组分块
来源：http://gp.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vl.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://xv.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://mb.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://sc.shtwfgs.cn

"7".padStart(3, "0")
来源：http://ys.hnjuh.cn

[U113] JS：正则替换全部
来源：http://ei.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://hz.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://dl.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://od.szxytkj.cn

[U115] JS：生成 UUID
来源：http://dr.huanxung.cn

crypto.randomUUID()
来源：http://lc.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://td.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://uo.shxzskj.cn

[U117] JS：单元测试
来源：http://sz.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://ht.asd995.cn

[U118] JS：开发服务器
来源：http://nc.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://ui.newstarts.cn

[U119] JS：生产构建
来源：http://xj.shxzskj.cn

npx vite build
来源：http://hi.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://vo.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://oj.shxzukj.cn

================================================================================
来源：http://cg.szsharing.cn

统计汇总
来源：http://ze.shxzskj.cn

================================================================================
来源：http://vo.huixinmuqiang.cn

按语言统计（条）：
来源：http://np.chemitech.net.cn

Python ......... 252
来源：http://xy.hnjuh.cn

PHP ............ 252
来源：http://dg.shxzukj.cn

JavaScript ..... 252
来源：http://cx.szxytkj.cn

TypeScript ..... 212
来源：http://vb.gzmigu.cn

Java ........... 212
来源：http://sl.haigaiapp.cn

Go ............. 212
来源：http://nu.chemitech.net.cn

Ruby ........... 212
来源：http://kq.newstarts.cn

C# ............. 212
来源：http://es.haigaiapp.cn

C .............. 30
来源：http://es.huixiangedu.cn

C++ ............ 30
来源：http://xm.huanxung.cn

SQL ............ 90
来源：http://xt.nicolike.cn

Bash ........... 80
来源：http://hr.asd995.cn

Kotlin ......... 15
来源：http://pj.huixinmuqiang.cn

Swift .......... 15
来源：http://ua.bjjhwx.cn

Lua ............ 10
来源：http://ty.huanxung.cn

Perl ........... 10
来源：http://wj.wgjwhj.cn

Scala .......... 10
来源：http://ow.jianghongdianzi.cn

------------------------------------
来源：http://ib.haigaiapp.cn

合计 ........... 2106 条
来源：http://hp.szxytkj.cn

按章节统计：
来源：http://qx.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mg.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gb.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ou.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yj.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bo.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mu.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tf.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gu.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qh.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ke.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zc.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jd.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rr.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rc.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tf.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wu.szsharing.cn

Q SQL 专题                              90
来源：http://gi.yuntaijiaju.cn

R Bash 专题                             80
来源：http://oj.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://pi.9csxet.cn

T 其他语言补充                          60
来源：http://nu.wgjwhj.cn

U 高频实用片段                         120
来源：http://nx.nicolike.cn

------------------------------------
来源：http://mv.bookmarksfly.cn

合计                                  2106 条
来源：http://ka.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://lp.9csxet.cn

使用提醒
来源：http://kv.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ys.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xq.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xv.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yo.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oh.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jh.bookmarksfly.cn

—— 文件结束 ——
来源：http://yf.asd995.cn

================================================================================
来源：http://oz.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://ok.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://gw.yuexingan06.cn

================================================================================
来源：http://pr.muxihuayi.cn

【收录内容】
来源：http://ze.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ci.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tz.haigaiapp.cn

SQL · Bash · C · C++
来源：http://jj.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zc.9csxet.cn

【使用说明】
来源：http://al.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ev.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zw.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ul.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xu.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fq.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ro.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ov.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hr.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xz.szxytkj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uj.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qx.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ay.shtwfgs.cn

【文件统计】
来源：http://gi.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zs.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://gw.hnjuh.cn

目  录
来源：http://dr.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://lq.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ve.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ug.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gm.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ps.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qs.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pv.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fr.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mg.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ot.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lq.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ex.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pd.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gm.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kd.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ck.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://km.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ri.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xz.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ph.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://da.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ux.hnjuh.cn

================================================================================
来源：http://zb.nicolike.cn

A. 基础语法与类型
来源：http://cb.haigaiapp.cn

================================================================================
来源：http://ck.jianghongdianzi.cn

[A01] Hello World
来源：http://pn.jctech888.com.cn

Py:   print("Hello, World!")
来源：http://mx.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://hy.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://qk.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wv.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://ti.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://rq.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://sv.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ug.nszjky.cn

[A02] 变量声明与赋值
来源：http://ar.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ey.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://er.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://io.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ff.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://cf.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://zy.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://ad.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lw.lnxyls.cn

[A03] 常量定义
来源：http://qa.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dx.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://rf.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://hv.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://lc.asd995.cn

Java: static final double PI = 3.14159;
来源：http://gt.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://db.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://fj.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://dn.jctech888.com.cn

[A04] 判断变量类型
来源：http://vl.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xo.newstarts.cn


<!-- 参考信息 -->