代发 wailian999

[U37] Py：读写 Excel
来源：http://ya.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eg.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://rt.colortex.cn

Path(__file__).resolve().parent
来源：http://st.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://ll.hahajie.cn

sys.stdout.isatty()
来源：http://am.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://oj.szsharing.cn

print("err", file=sys.stderr)
来源：http://bw.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://xe.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ea.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vg.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ip.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://sz.shtwfgs.cn

namespace App\Http;
来源：http://oz.colortex.cn

[U44] PHP：开启严格类型
来源：http://jf.szsharing.cn

declare(strict_types=1);
来源：http://yr.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://kt.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://en.shxzskj.cn

[U46] PHP：可空类型
来源：http://je.panjiajie.cn

?string $name = null
来源：http://ek.hahajie.cn

[U47] PHP：联合类型
来源：http://of.shtwfgs.cn

int|string $id
来源：http://zn.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://fd.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mo.muxihuayi.cn

[U49] PHP：只读属性
来源：http://tg.huixinmuqiang.cn

public readonly string $name
来源：http://yd.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://nn.panjiajie.cn

public function __construct(private int $id) {}
来源：http://qk.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://gk.shtwfgs.cn

[$a, $b] = $arr;
来源：http://xf.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://hv.asd995.cn

$double = fn($x) => $x * 2;
来源：http://he.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://nr.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://fy.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://jk.chemitech.net.cn

$obj?->method()
来源：http://qb.nszjky.cn

[U55] PHP：match 表达式
来源：http://il.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iv.szxytkj.cn

[U56] PHP：命名参数
来源：http://is.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ck.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://zz.colortex.cn

"值: {$a}"
来源：http://jw.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://ut.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ax.szxytkj.cn

[U59] PHP：自定义排序
来源：http://ms.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://it.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://fm.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oe.wgjwhj.cn

[U61] PHP：正则
来源：http://ri.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nw.muxihuayi.cn

[U62] PHP：日期对象
来源：http://hr.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rw.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://ls.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ix.asd995.cn

[U64] PHP：目录遍历
来源：http://wv.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://bj.hnjuh.cn

[U65] PHP：会话
来源：http://ap.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lc.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://wz.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fg.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://nm.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kt.hahajie.cn

[U68] PHP：PDO 连接
来源：http://ya.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ke.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://mp.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mu.9csxet.cn

[U70] PHP：PDO 事务
来源：http://mg.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://df.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://bg.521024.cn

throw new RuntimeException("失败", 500);
来源：http://bs.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://cj.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://sw.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://kv.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://ww.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://ti.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://kd.colortex.cn

[U75] PHP：依赖注入
来源：http://es.hahajie.cn

composer require psr/container
来源：http://sb.nszjky.cn

[U76] PHP：简单路由
来源：http://kh.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qg.shxzskj.cn

[U77] PHP：模板渲染
来源：http://bs.9csxet.cn

composer require twig/twig
来源：http://bo.haigaiapp.cn

[U78] PHP：单元测试
来源：http://qt.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://wr.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://ew.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://xj.nicolike.cn

[U80] PHP：代码规范修复
来源：http://na.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eg.muxihuayi.cn

[U81] JS：初始化项目
来源：http://yp.huixiangedu.cn

npm init -y;  npm i express
来源：http://ct.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://jh.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oi.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://tw.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zm.521024.cn

[U84] JS：CommonJS 写法
来源：http://vl.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kk.panjiajie.cn

[U85] JS：可选链
来源：http://ib.shtwfgs.cn

a?.b?.c
来源：http://kb.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://km.bookmarksfly.cn

a ?? b
来源：http://un.chemitech.net.cn

[U87] JS：解构默认值
来源：http://mn.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://fk.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://cn.bookmarksfly.cn

{ ...a, ...b }
来源：http://ug.yuexingan06.cn

[U89] JS：数组去重
来源：http://uq.jianghongdianzi.cn

[...new Set(arr)]
来源：http://ob.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://oi.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://cy.hahajie.cn

[U91] JS：对象键值遍历
来源：http://ei.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xj.shxzukj.cn

[U92] JS：深拷贝
来源：http://hh.muxihuayi.cn

structuredClone(obj)
来源：http://ez.yuexingan06.cn

[U93] JS：模板字符串
来源：http://kr.521024.cn

`共 ${n} 条`
来源：http://tk.hahajie.cn

[U94] JS：箭头函数
来源：http://ap.shtwfgs.cn

const double = x => x * 2;
来源：http://ly.asd995.cn

[U95] JS：Promise 包装
来源：http://ox.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://cl.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://ki.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ss.hahajie.cn

[U97] JS：并发请求
来源：http://vv.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pz.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://hk.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fj.yuexingan06.cn

[U99] JS：事件监听
来源：http://ks.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://gm.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://zl.gzmigu.cn

document.querySelector(".item")
来源：http://vj.lnxyls.cn

[U101] JS：classList 操作
来源：http://xy.gzmigu.cn

el.classList.toggle("active")
来源：http://rp.shxzukj.cn

[U102] JS：本地存储
来源：http://ia.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dl.nicolike.cn

[U103] JS：定时器
来源：http://ya.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qt.szsharing.cn

[U104] JS：防抖
来源：http://xj.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xy.shtwfgs.cn

[U105] JS：节流
来源：http://jc.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sf.521024.cn

[U106] JS：日期格式化
来源：http://yk.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vu.shxzukj.cn

[U107] JS：数字千分位
来源：http://kv.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fy.nszjky.cn

[U108] JS：随机整数
来源：http://iy.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pw.yuexingan06.cn

[U109] JS：数组分组
来源：http://lg.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://pg.shxzukj.cn

[U110] JS：数组分块
来源：http://op.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zm.szxytkj.cn

[U111] JS：对象转 Map
来源：http://jm.asd995.cn

new Map(Object.entries(obj))
来源：http://da.szxytkj.cn

[U112] JS：字符串补位
来源：http://cx.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://om.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://ty.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://cz.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://ma.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gd.9csxet.cn

[U115] JS：生成 UUID
来源：http://xa.hahajie.cn

crypto.randomUUID()
来源：http://yy.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://kk.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://fr.yuexingan06.cn

[U117] JS：单元测试
来源：http://ym.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://bc.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://wz.gzmigu.cn

npm i -D vite;  npx vite
来源：http://la.newstarts.cn

[U119] JS：生产构建
来源：http://tu.gzmigu.cn

npx vite build
来源：http://ur.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://tv.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://ve.huanxung.cn

================================================================================
来源：http://zj.huanxung.cn

统计汇总
来源：http://zc.huixiangedu.cn

================================================================================
来源：http://ic.jianghongdianzi.cn

按语言统计（条）：
来源：http://ln.jianghongdianzi.cn

Python ......... 252
来源：http://dh.9csxet.cn

PHP ............ 252
来源：http://lv.muxihuayi.cn

JavaScript ..... 252
来源：http://sy.shxzskj.cn

TypeScript ..... 212
来源：http://yg.szxytkj.cn

Java ........... 212
来源：http://wd.lnxyls.cn

Go ............. 212
来源：http://ze.521024.cn

Ruby ........... 212
来源：http://kr.9csxet.cn

C# ............. 212
来源：http://ye.huanxung.cn

C .............. 30
来源：http://na.huixinmuqiang.cn

C++ ............ 30
来源：http://bl.wgjwhj.cn

SQL ............ 90
来源：http://um.newstarts.cn

Bash ........... 80
来源：http://rg.wgjwhj.cn

Kotlin ......... 15
来源：http://rz.huanxung.cn

Swift .......... 15
来源：http://so.bjjhwx.cn

Lua ............ 10
来源：http://ez.panjiajie.cn

Perl ........... 10
来源：http://el.huixiangedu.cn

Scala .......... 10
来源：http://dq.jctech888.com.cn

------------------------------------
来源：http://ks.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://ju.huanxung.cn

按章节统计：
来源：http://jd.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ug.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ik.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ym.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ai.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ii.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kc.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pq.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tn.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nb.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://an.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rk.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rl.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://na.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rq.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zd.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qu.szxytkj.cn

Q SQL 专题                              90
来源：http://yv.yuntaijiaju.cn

R Bash 专题                             80
来源：http://ws.521024.cn

S C / C++ 专题                          60
来源：http://pj.shxzskj.cn

T 其他语言补充                          60
来源：http://wo.jctech888.com.cn

U 高频实用片段                         120
来源：http://fn.szsharing.cn

------------------------------------
来源：http://kz.9csxet.cn

合计                                  2106 条
来源：http://oh.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://op.huixinmuqiang.cn

使用提醒
来源：http://vw.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://wb.shxzukj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://co.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://py.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eu.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sn.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bd.shxzukj.cn

—— 文件结束 ——
来源：http://uj.jctech888.com.cn

================================================================================
来源：http://pn.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://mg.asd995.cn

Common Programming Examples Cheat Book
来源：http://vc.nszjky.cn

================================================================================
来源：http://cu.shtwfgs.cn

【收录内容】
来源：http://xg.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ik.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oi.muxihuayi.cn

SQL · Bash · C · C++
来源：http://ge.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ux.haigaiapp.cn

【使用说明】
来源：http://nc.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ug.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ie.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yl.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cj.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ht.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oq.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vr.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ck.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lt.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rs.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://as.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eb.yuexingan06.cn

【文件统计】
来源：http://ai.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tv.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://zp.jianghongdianzi.cn

目  录
来源：http://ju.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ao.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uy.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sw.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hc.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zt.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xr.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rb.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://if.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tq.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aw.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tr.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mq.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ly.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fc.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bm.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sj.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nn.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gi.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ps.colortex.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ct.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yb.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fe.jianghongdianzi.cn

================================================================================
来源：http://zd.9csxet.cn

A. 基础语法与类型
来源：http://bs.haigaiapp.cn

================================================================================
来源：http://vd.shxzukj.cn

[A01] Hello World
来源：http://ra.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://qe.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://us.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://hj.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ui.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://im.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://tl.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://xa.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ra.nicolike.cn

[A02] 变量声明与赋值
来源：http://sx.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lt.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://px.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xw.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://im.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://qe.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://ws.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://am.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vy.wgjwhj.cn

[A03] 常量定义
来源：http://ze.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ku.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://tx.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://av.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://wy.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://zf.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://nm.wgjwhj.cn


<!-- 参考信息 -->