代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://ay.9csxet.cn

sys.stdout.isatty()
来源：http://kk.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://qh.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://wp.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://qo.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wi.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://gf.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://au.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://qh.asd995.cn

namespace App\Http;
来源：http://be.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://nk.chemitech.net.cn

declare(strict_types=1);
来源：http://ym.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://te.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xh.huixiangedu.cn

[U46] PHP：可空类型
来源：http://kd.shxzukj.cn

?string $name = null
来源：http://mo.szxytkj.cn

[U47] PHP：联合类型
来源：http://od.colortex.cn

int|string $id
来源：http://dp.szxytkj.cn

[U48] PHP：纯枚举
来源：http://kp.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wy.nszjky.cn

[U49] PHP：只读属性
来源：http://du.chemitech.net.cn

public readonly string $name
来源：http://cb.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://ek.szxytkj.cn

public function __construct(private int $id) {}
来源：http://bu.hnjuh.cn

[U51] PHP：数组解构
来源：http://oe.huixiangedu.cn

[$a, $b] = $arr;
来源：http://ra.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://nk.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://fb.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://jj.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://dz.nszjky.cn

[U54] PHP：空安全调用
来源：http://qx.szxytkj.cn

$obj?->method()
来源：http://gc.lnxyls.cn

[U55] PHP：match 表达式
来源：http://dg.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tk.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://om.chemitech.net.cn

f(a: 1, b: 2)
来源：http://hb.huanxung.cn

[U57] PHP：字符串插值
来源：http://ct.yuexingan06.cn

"值: {$a}"
来源：http://qq.panjiajie.cn

[U58] PHP：数组三件套
来源：http://jb.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sn.nszjky.cn

[U59] PHP：自定义排序
来源：http://do.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hk.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://tj.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://am.huixinmuqiang.cn

[U61] PHP：正则
来源：http://nh.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pb.nszjky.cn

[U62] PHP：日期对象
来源：http://ib.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://la.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://km.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dv.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://ca.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://np.hahajie.cn

[U65] PHP：会话
来源：http://vb.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yn.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://pf.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gf.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://fl.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lv.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://ee.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://os.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://vj.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vw.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://af.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uy.asd995.cn

[U71] PHP：抛出异常
来源：http://ck.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://pn.hnjuh.cn

[U72] PHP：写错误日志
来源：http://ax.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://ym.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://bl.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://gv.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://ad.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://bu.huanxung.cn

[U75] PHP：依赖注入
来源：http://lu.shtwfgs.cn

composer require psr/container
来源：http://tn.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://tn.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jv.panjiajie.cn

[U77] PHP：模板渲染
来源：http://pu.haigaiapp.cn

composer require twig/twig
来源：http://cm.colortex.cn

[U78] PHP：单元测试
来源：http://sq.asd995.cn

composer require --dev phpunit/phpunit
来源：http://rz.wgjwhj.cn

[U79] PHP：静态分析
来源：http://cz.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://hf.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://uy.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vo.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://ez.wgjwhj.cn

npm init -y;  npm i express
来源：http://lo.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://rt.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nh.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://pz.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bb.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://ye.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gp.shtwfgs.cn

[U85] JS：可选链
来源：http://fp.shxzukj.cn

a?.b?.c
来源：http://va.jctech888.com.cn

[U86] JS：空值合并
来源：http://ov.jianghongdianzi.cn

a ?? b
来源：http://lq.muxihuayi.cn

[U87] JS：解构默认值
来源：http://xe.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://bc.newstarts.cn

[U88] JS：对象展开合并
来源：http://yt.shxzskj.cn

{ ...a, ...b }
来源：http://fc.9csxet.cn

[U89] JS：数组去重
来源：http://mq.szxytkj.cn

[...new Set(arr)]
来源：http://kb.panjiajie.cn

[U90] JS：数字数组排序
来源：http://kg.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://ri.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://fr.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ga.nszjky.cn

[U92] JS：深拷贝
来源：http://ow.panjiajie.cn

structuredClone(obj)
来源：http://ru.521024.cn

[U93] JS：模板字符串
来源：http://ol.wgjwhj.cn

`共 ${n} 条`
来源：http://ya.chemitech.net.cn

[U94] JS：箭头函数
来源：http://vp.asd995.cn

const double = x => x * 2;
来源：http://qm.nicolike.cn

[U95] JS：Promise 包装
来源：http://gk.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://wn.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://nu.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ed.nicolike.cn

[U97] JS：并发请求
来源：http://qx.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bm.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://fu.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pw.wgjwhj.cn

[U99] JS：事件监听
来源：http://rg.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://rp.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://wr.hnjuh.cn

document.querySelector(".item")
来源：http://gp.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://no.asd995.cn

el.classList.toggle("active")
来源：http://ri.huixiangedu.cn

[U102] JS：本地存储
来源：http://jh.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vp.hnjuh.cn

[U103] JS：定时器
来源：http://ti.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://td.shtwfgs.cn

[U104] JS：防抖
来源：http://qu.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gl.jctech888.com.cn

[U105] JS：节流
来源：http://sb.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sp.hahajie.cn

[U106] JS：日期格式化
来源：http://fe.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ns.nicolike.cn

[U107] JS：数字千分位
来源：http://dc.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gl.shxzskj.cn

[U108] JS：随机整数
来源：http://jp.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ve.chemitech.net.cn

[U109] JS：数组分组
来源：http://bk.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://xs.shxzukj.cn

[U110] JS：数组分块
来源：http://ml.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ka.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://jb.nszjky.cn

new Map(Object.entries(obj))
来源：http://fy.colortex.cn

[U112] JS：字符串补位
来源：http://yc.jctech888.com.cn

"7".padStart(3, "0")
来源：http://tt.huanxung.cn

[U113] JS：正则替换全部
来源：http://ys.hnjuh.cn

s.replaceAll("a", "b")
来源：http://wf.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://ba.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zd.hahajie.cn

[U115] JS：生成 UUID
来源：http://hg.newstarts.cn

crypto.randomUUID()
来源：http://im.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://te.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://ua.jctech888.com.cn

[U117] JS：单元测试
来源：http://mx.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://wz.szxytkj.cn

[U118] JS：开发服务器
来源：http://ed.panjiajie.cn

npm i -D vite;  npx vite
来源：http://ed.shxzskj.cn

[U119] JS：生产构建
来源：http://pd.521024.cn

npx vite build
来源：http://qu.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://xr.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://mt.yuexingan06.cn

================================================================================
来源：http://tu.hnjuh.cn

统计汇总
来源：http://qh.shxzskj.cn

================================================================================
来源：http://fz.shtwfgs.cn

按语言统计（条）：
来源：http://lf.huixiangedu.cn

Python ......... 252
来源：http://cx.muxihuayi.cn

PHP ............ 252
来源：http://mp.lnxyls.cn

JavaScript ..... 252
来源：http://so.gzmigu.cn

TypeScript ..... 212
来源：http://tt.gzmigu.cn

Java ........... 212
来源：http://fv.nszjky.cn

Go ............. 212
来源：http://dq.colortex.cn

Ruby ........... 212
来源：http://sl.521024.cn

C# ............. 212
来源：http://bd.shtwfgs.cn

C .............. 30
来源：http://ce.shxzskj.cn

C++ ............ 30
来源：http://bo.hahajie.cn

SQL ............ 90
来源：http://qp.yuntaijiaju.cn

Bash ........... 80
来源：http://ue.haigaiapp.cn

Kotlin ......... 15
来源：http://tw.yuntaijiaju.cn

Swift .......... 15
来源：http://kv.wgjwhj.cn

Lua ............ 10
来源：http://og.huanxung.cn

Perl ........... 10
来源：http://ij.szxytkj.cn

Scala .......... 10
来源：http://nh.haigaiapp.cn

------------------------------------
来源：http://df.panjiajie.cn

合计 ........... 2106 条
来源：http://aa.chemitech.net.cn

按章节统计：
来源：http://or.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bt.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://un.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lj.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ub.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ml.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yc.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hb.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rz.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vl.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qi.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ul.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ua.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vq.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jc.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yd.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vj.huanxung.cn

Q SQL 专题                              90
来源：http://iq.yuexingan06.cn

R Bash 专题                             80
来源：http://cg.panjiajie.cn

S C / C++ 专题                          60
来源：http://as.colortex.cn

T 其他语言补充                          60
来源：http://dz.lnxyls.cn

U 高频实用片段                         120
来源：http://eg.newstarts.cn

------------------------------------
来源：http://lb.colortex.cn

合计                                  2106 条
来源：http://xv.521024.cn

--------------------------------------------------------------------------------
来源：http://ao.gzmigu.cn

使用提醒
来源：http://zo.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://cd.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pw.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mt.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mb.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yj.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eo.bookmarksfly.cn

—— 文件结束 ——
来源：http://lh.newstarts.cn

================================================================================
来源：http://kw.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://xa.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://co.panjiajie.cn

================================================================================
来源：http://qw.shtwfgs.cn

【收录内容】
来源：http://mn.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nj.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yw.shxzukj.cn

SQL · Bash · C · C++
来源：http://sn.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wy.shxzskj.cn

【使用说明】
来源：http://js.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lp.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uw.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sm.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rr.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://do.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ng.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ep.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tt.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lq.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zw.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pq.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ja.bookmarksfly.cn

【文件统计】
来源：http://vn.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uy.nszjky.cn

--------------------------------------------------------------------------------
来源：http://ao.huixinmuqiang.cn

目  录
来源：http://yi.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://rv.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://av.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://av.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tk.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wr.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fj.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oq.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://au.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ac.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ld.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://td.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sk.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ch.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ro.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kl.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lk.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dx.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ax.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mq.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xt.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://av.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bu.huixinmuqiang.cn

================================================================================
来源：http://zt.panjiajie.cn

A. 基础语法与类型
来源：http://ij.nicolike.cn

================================================================================
来源：http://do.huanxung.cn

[A01] Hello World
来源：http://dr.nszjky.cn

Py:   print("Hello, World!")
来源：http://vw.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://dn.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://wb.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wo.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://am.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://dm.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://vj.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yy.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://my.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tq.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hq.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ld.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://to.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://wq.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://zf.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://vr.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cl.hnjuh.cn

[A03] 常量定义
来源：http://cn.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sp.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://of.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://qa.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://oy.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://eu.asd995.cn

Go:   const PI = 3.14159
来源：http://xu.szxytkj.cn

Ruby: PI = 3.14159
来源：http://zf.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://rt.nicolike.cn

[A04] 判断变量类型
来源：http://ti.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zx.muxihuayi.cn


<!-- 参考信息 -->