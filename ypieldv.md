代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://sh.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vh.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://sh.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fr.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://dv.newstarts.cn

namespace App\Http;
来源：http://gx.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://ai.bjjhwx.cn

declare(strict_types=1);
来源：http://vl.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://il.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://br.hnjuh.cn

[U46] PHP：可空类型
来源：http://pl.521024.cn

?string $name = null
来源：http://dj.wgjwhj.cn

[U47] PHP：联合类型
来源：http://dp.hnjuh.cn

int|string $id
来源：http://ay.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://nf.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zt.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://wk.huixinmuqiang.cn

public readonly string $name
来源：http://ov.521024.cn

[U50] PHP：构造器属性提升
来源：http://ax.panjiajie.cn

public function __construct(private int $id) {}
来源：http://jp.asd995.cn

[U51] PHP：数组解构
来源：http://sn.9csxet.cn

[$a, $b] = $arr;
来源：http://bg.colortex.cn

[U52] PHP：箭头函数
来源：http://lj.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://ez.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://du.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://xt.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://ay.jctech888.com.cn

$obj?->method()
来源：http://xv.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://lz.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iq.huanxung.cn

[U56] PHP：命名参数
来源：http://wz.asd995.cn

f(a: 1, b: 2)
来源：http://ie.521024.cn

[U57] PHP：字符串插值
来源：http://rj.lnxyls.cn

"值: {$a}"
来源：http://ts.lnxyls.cn

[U58] PHP：数组三件套
来源：http://st.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://my.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://hs.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zs.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://ms.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dq.huanxung.cn

[U61] PHP：正则
来源：http://up.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kh.haigaiapp.cn

[U62] PHP：日期对象
来源：http://wn.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qm.huanxung.cn

[U63] PHP：文件读写
来源：http://kb.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cz.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://pf.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://pr.panjiajie.cn

[U65] PHP：会话
来源：http://bt.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aq.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://sw.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ft.521024.cn

[U67] PHP：处理文件上传
来源：http://uu.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dd.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://by.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://si.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://hb.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yy.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://ra.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cn.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://xn.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://vi.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://rq.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://cy.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://lx.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://eh.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://xs.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://kv.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://wc.huixinmuqiang.cn

composer require psr/container
来源：http://xs.521024.cn

[U76] PHP：简单路由
来源：http://gf.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tk.9csxet.cn

[U77] PHP：模板渲染
来源：http://yc.szsharing.cn

composer require twig/twig
来源：http://vv.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://jl.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://zf.shxzukj.cn

[U79] PHP：静态分析
来源：http://pv.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://uh.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://as.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xe.panjiajie.cn

[U81] JS：初始化项目
来源：http://cq.muxihuayi.cn

npm init -y;  npm i express
来源：http://vx.nszjky.cn

[U82] JS：package.json 脚本
来源：http://dj.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ij.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://yv.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jr.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://dl.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cu.huixinmuqiang.cn

[U85] JS：可选链
来源：http://ie.gzmigu.cn

a?.b?.c
来源：http://cl.shtwfgs.cn

[U86] JS：空值合并
来源：http://lz.shxzskj.cn

a ?? b
来源：http://tn.chemitech.net.cn

[U87] JS：解构默认值
来源：http://gy.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://xu.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://eq.panjiajie.cn

{ ...a, ...b }
来源：http://aq.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://nx.hahajie.cn

[...new Set(arr)]
来源：http://sz.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://gl.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://ll.colortex.cn

[U91] JS：对象键值遍历
来源：http://kn.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hs.lnxyls.cn

[U92] JS：深拷贝
来源：http://ug.bookmarksfly.cn

structuredClone(obj)
来源：http://px.shtwfgs.cn

[U93] JS：模板字符串
来源：http://sa.chemitech.net.cn

`共 ${n} 条`
来源：http://sb.shxzskj.cn

[U94] JS：箭头函数
来源：http://cw.hahajie.cn

const double = x => x * 2;
来源：http://gy.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://cz.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://jz.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://gd.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pw.asd995.cn

[U97] JS：并发请求
来源：http://fh.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ug.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://nc.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xv.chemitech.net.cn

[U99] JS：事件监听
来源：http://st.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://ft.shxzskj.cn

[U100] JS：DOM 查询
来源：http://dp.jctech888.com.cn

document.querySelector(".item")
来源：http://yc.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://gn.asd995.cn

el.classList.toggle("active")
来源：http://ok.szsharing.cn

[U102] JS：本地存储
来源：http://ct.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ke.colortex.cn

[U103] JS：定时器
来源：http://tx.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uj.lnxyls.cn

[U104] JS：防抖
来源：http://sw.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hc.yuntaijiaju.cn

[U105] JS：节流
来源：http://mk.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nk.szsharing.cn

[U106] JS：日期格式化
来源：http://uy.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eb.asd995.cn

[U107] JS：数字千分位
来源：http://wh.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ej.haigaiapp.cn

[U108] JS：随机整数
来源：http://ab.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cu.nicolike.cn

[U109] JS：数组分组
来源：http://ab.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://nq.huanxung.cn

[U110] JS：数组分块
来源：http://zx.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jk.521024.cn

[U111] JS：对象转 Map
来源：http://pv.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://bu.colortex.cn

[U112] JS：字符串补位
来源：http://cn.lnxyls.cn

"7".padStart(3, "0")
来源：http://bf.asd995.cn

[U113] JS：正则替换全部
来源：http://tm.szxytkj.cn

s.replaceAll("a", "b")
来源：http://pi.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://az.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pn.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://jt.asd995.cn

crypto.randomUUID()
来源：http://qb.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://oq.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://hf.huixiangedu.cn

[U117] JS：单元测试
来源：http://ug.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://ch.muxihuayi.cn

[U118] JS：开发服务器
来源：http://gl.hahajie.cn

npm i -D vite;  npx vite
来源：http://dn.jctech888.com.cn

[U119] JS：生产构建
来源：http://qy.huixiangedu.cn

npx vite build
来源：http://or.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://se.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://oo.521024.cn

================================================================================
来源：http://gd.hnjuh.cn

统计汇总
来源：http://jr.9csxet.cn

================================================================================
来源：http://ld.jctech888.com.cn

按语言统计（条）：
来源：http://fw.wgjwhj.cn

Python ......... 252
来源：http://vs.chemitech.net.cn

PHP ............ 252
来源：http://sz.haigaiapp.cn

JavaScript ..... 252
来源：http://vn.hnjuh.cn

TypeScript ..... 212
来源：http://jy.shtwfgs.cn

Java ........... 212
来源：http://xh.bookmarksfly.cn

Go ............. 212
来源：http://th.shxzskj.cn

Ruby ........... 212
来源：http://ta.shxzskj.cn

C# ............. 212
来源：http://df.yuntaijiaju.cn

C .............. 30
来源：http://cq.jianghongdianzi.cn

C++ ............ 30
来源：http://ka.colortex.cn

SQL ............ 90
来源：http://tu.huanxung.cn

Bash ........... 80
来源：http://pz.hnjuh.cn

Kotlin ......... 15
来源：http://us.wgjwhj.cn

Swift .......... 15
来源：http://wq.muxihuayi.cn

Lua ............ 10
来源：http://sk.colortex.cn

Perl ........... 10
来源：http://eg.shxzskj.cn

Scala .......... 10
来源：http://hk.bjjhwx.cn

------------------------------------
来源：http://mn.9csxet.cn

合计 ........... 2106 条
来源：http://vj.chemitech.net.cn

按章节统计：
来源：http://tf.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hg.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vf.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uy.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rv.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bg.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://os.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mu.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vb.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sd.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ml.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wk.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ch.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://up.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lm.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://is.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jj.yuexingan06.cn

Q SQL 专题                              90
来源：http://xq.hnjuh.cn

R Bash 专题                             80
来源：http://hu.hnjuh.cn

S C / C++ 专题                          60
来源：http://kx.jctech888.com.cn

T 其他语言补充                          60
来源：http://ie.hahajie.cn

U 高频实用片段                         120
来源：http://ng.wgjwhj.cn

------------------------------------
来源：http://dm.shxzskj.cn

合计                                  2106 条
来源：http://vw.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://pn.colortex.cn

使用提醒
来源：http://tq.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://xo.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dq.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cu.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qk.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cf.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gq.yuntaijiaju.cn

—— 文件结束 ——
来源：http://hc.nszjky.cn

================================================================================
来源：http://hl.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://yk.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://pu.lnxyls.cn

================================================================================
来源：http://yt.huixiangedu.cn

【收录内容】
来源：http://lf.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://am.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jk.jctech888.com.cn

SQL · Bash · C · C++
来源：http://xb.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vo.newstarts.cn

【使用说明】
来源：http://fc.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://du.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lc.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zf.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yl.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://eh.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://da.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ym.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oi.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vs.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uw.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xj.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eh.shxzskj.cn

【文件统计】
来源：http://dx.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zc.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://tw.huanxung.cn

目  录
来源：http://ec.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://qr.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yr.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lk.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wm.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vb.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jc.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://at.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gm.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vi.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dq.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wd.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sz.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ou.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://th.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ox.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pe.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gl.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pt.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vg.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hb.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cw.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lj.huixiangedu.cn

================================================================================
来源：http://ep.colortex.cn

A. 基础语法与类型
来源：http://ed.shtwfgs.cn

================================================================================
来源：http://fi.asd995.cn

[A01] Hello World
来源：http://rc.nszjky.cn

Py:   print("Hello, World!")
来源：http://sz.colortex.cn

PHP:  echo "Hello, World!";
来源：http://ej.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://dg.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rf.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://ud.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://rq.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://dm.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sw.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://gj.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dk.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nq.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dp.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bi.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://li.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://el.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://ww.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eu.chemitech.net.cn

[A03] 常量定义
来源：http://wf.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ht.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://re.asd995.cn

JS:   const PI = 3.14159;
来源：http://ai.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://ri.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://gb.lnxyls.cn

Go:   const PI = 3.14159
来源：http://ui.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://xu.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://dw.nicolike.cn

[A04] 判断变量类型
来源：http://mk.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qu.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ng.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qy.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://no.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cn.bookmarksfly.cn


<!-- 参考信息 -->