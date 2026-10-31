代发 wailian999

[U37] Py：读写 Excel
来源：http://ds.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tw.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://co.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://wt.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://cd.haigaiapp.cn

sys.stdout.isatty()
来源：http://jp.9csxet.cn

[U40] Py：打印到标准错误
来源：http://cc.hahajie.cn

print("err", file=sys.stderr)
来源：http://zv.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://jb.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eh.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://qy.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xn.newstarts.cn

[U43] PHP：声明命名空间
来源：http://fg.nszjky.cn

namespace App\Http;
来源：http://pf.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://wh.521024.cn

declare(strict_types=1);
来源：http://ef.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://to.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lu.hnjuh.cn

[U46] PHP：可空类型
来源：http://xo.huixiangedu.cn

?string $name = null
来源：http://cw.colortex.cn

[U47] PHP：联合类型
来源：http://yr.521024.cn

int|string $id
来源：http://uv.szsharing.cn

[U48] PHP：纯枚举
来源：http://jc.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wo.newstarts.cn

[U49] PHP：只读属性
来源：http://by.nszjky.cn

public readonly string $name
来源：http://to.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://xo.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://uy.shtwfgs.cn

[U51] PHP：数组解构
来源：http://kb.asd995.cn

[$a, $b] = $arr;
来源：http://da.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://yp.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://pn.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://rw.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://ug.9csxet.cn

[U54] PHP：空安全调用
来源：http://gr.shxzukj.cn

$obj?->method()
来源：http://to.hnjuh.cn

[U55] PHP：match 表达式
来源：http://ye.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rj.nszjky.cn

[U56] PHP：命名参数
来源：http://bj.szsharing.cn

f(a: 1, b: 2)
来源：http://xc.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://ar.huanxung.cn

"值: {$a}"
来源：http://pu.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://bb.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ly.colortex.cn

[U59] PHP：自定义排序
来源：http://kp.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pq.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://cw.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://id.chemitech.net.cn

[U61] PHP：正则
来源：http://gt.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ko.huanxung.cn

[U62] PHP：日期对象
来源：http://xk.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ru.nszjky.cn

[U63] PHP：文件读写
来源：http://vf.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ab.szxytkj.cn

[U64] PHP：目录遍历
来源：http://ei.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://np.9csxet.cn

[U65] PHP：会话
来源：http://pt.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qb.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://gj.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tv.521024.cn

[U67] PHP：处理文件上传
来源：http://je.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ao.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://zo.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bc.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://ct.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hn.colortex.cn

[U70] PHP：PDO 事务
来源：http://so.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ft.hahajie.cn

[U71] PHP：抛出异常
来源：http://eb.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://wz.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://wv.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://wp.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://hi.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://jl.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://zq.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://gd.shxzukj.cn

[U75] PHP：依赖注入
来源：http://pd.bjjhwx.cn

composer require psr/container
来源：http://fk.muxihuayi.cn

[U76] PHP：简单路由
来源：http://ev.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eb.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://ry.colortex.cn

composer require twig/twig
来源：http://im.shxzskj.cn

[U78] PHP：单元测试
来源：http://bb.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://yx.muxihuayi.cn

[U79] PHP：静态分析
来源：http://bb.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://nz.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://ul.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xy.huanxung.cn

[U81] JS：初始化项目
来源：http://we.haigaiapp.cn

npm init -y;  npm i express
来源：http://ul.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://ny.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ra.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://uo.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ru.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://gg.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yv.9csxet.cn

[U85] JS：可选链
来源：http://qo.9csxet.cn

a?.b?.c
来源：http://ca.lnxyls.cn

[U86] JS：空值合并
来源：http://de.hahajie.cn

a ?? b
来源：http://jj.nszjky.cn

[U87] JS：解构默认值
来源：http://tz.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ij.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://io.jianghongdianzi.cn

{ ...a, ...b }
来源：http://kt.szsharing.cn

[U89] JS：数组去重
来源：http://za.panjiajie.cn

[...new Set(arr)]
来源：http://gi.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://tz.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://yz.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://pc.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bt.asd995.cn

[U92] JS：深拷贝
来源：http://le.huanxung.cn

structuredClone(obj)
来源：http://mi.colortex.cn

[U93] JS：模板字符串
来源：http://nv.jctech888.com.cn

`共 ${n} 条`
来源：http://kp.shxzukj.cn

[U94] JS：箭头函数
来源：http://bp.muxihuayi.cn

const double = x => x * 2;
来源：http://vy.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://nm.asd995.cn

new Promise((resolve, reject) => {})
来源：http://th.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://nz.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pm.9csxet.cn

[U97] JS：并发请求
来源：http://ge.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ck.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://as.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bd.szsharing.cn

[U99] JS：事件监听
来源：http://lc.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://zx.nicolike.cn

[U100] JS：DOM 查询
来源：http://fp.muxihuayi.cn

document.querySelector(".item")
来源：http://yu.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://oq.huanxung.cn

el.classList.toggle("active")
来源：http://mp.yuexingan06.cn

[U102] JS：本地存储
来源：http://cg.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oh.shxzukj.cn

[U103] JS：定时器
来源：http://ff.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nn.huanxung.cn

[U104] JS：防抖
来源：http://xi.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nd.hnjuh.cn

[U105] JS：节流
来源：http://yj.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gb.jctech888.com.cn

[U106] JS：日期格式化
来源：http://jf.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://li.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://gd.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cs.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://ok.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wv.gzmigu.cn

[U109] JS：数组分组
来源：http://yc.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://sf.szxytkj.cn

[U110] JS：数组分块
来源：http://bm.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ta.szxytkj.cn

[U111] JS：对象转 Map
来源：http://jx.panjiajie.cn

new Map(Object.entries(obj))
来源：http://ut.nicolike.cn

[U112] JS：字符串补位
来源：http://tz.chemitech.net.cn

"7".padStart(3, "0")
来源：http://ok.shxzukj.cn

[U113] JS：正则替换全部
来源：http://qq.szxytkj.cn

s.replaceAll("a", "b")
来源：http://kr.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://cn.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dn.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://tj.shtwfgs.cn

crypto.randomUUID()
来源：http://eb.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://yb.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://ws.haigaiapp.cn

[U117] JS：单元测试
来源：http://dk.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://jn.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://bz.521024.cn

npm i -D vite;  npx vite
来源：http://yu.wgjwhj.cn

[U119] JS：生产构建
来源：http://bb.jianghongdianzi.cn

npx vite build
来源：http://ix.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://bb.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://mc.yuexingan06.cn

================================================================================
来源：http://td.panjiajie.cn

统计汇总
来源：http://ll.nszjky.cn

================================================================================
来源：http://iv.shtwfgs.cn

按语言统计（条）：
来源：http://ug.wgjwhj.cn

Python ......... 252
来源：http://ok.shtwfgs.cn

PHP ............ 252
来源：http://bf.9csxet.cn

JavaScript ..... 252
来源：http://ao.colortex.cn

TypeScript ..... 212
来源：http://qm.yuexingan06.cn

Java ........... 212
来源：http://nl.9csxet.cn

Go ............. 212
来源：http://cg.gzmigu.cn

Ruby ........... 212
来源：http://sb.yuexingan06.cn

C# ............. 212
来源：http://hw.bookmarksfly.cn

C .............. 30
来源：http://nk.yuntaijiaju.cn

C++ ............ 30
来源：http://qi.wgjwhj.cn

SQL ............ 90
来源：http://es.hnjuh.cn

Bash ........... 80
来源：http://zg.szsharing.cn

Kotlin ......... 15
来源：http://ev.521024.cn

Swift .......... 15
来源：http://oo.haigaiapp.cn

Lua ............ 10
来源：http://wr.huixiangedu.cn

Perl ........... 10
来源：http://bl.yuexingan06.cn

Scala .......... 10
来源：http://jk.colortex.cn

------------------------------------
来源：http://pg.colortex.cn

合计 ........... 2106 条
来源：http://gw.chemitech.net.cn

按章节统计：
来源：http://ws.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cs.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://de.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dd.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://up.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gx.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lp.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tm.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ns.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yz.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zw.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rd.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ul.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ke.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fu.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yt.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jq.bjjhwx.cn

Q SQL 专题                              90
来源：http://jy.nszjky.cn

R Bash 专题                             80
来源：http://qy.nicolike.cn

S C / C++ 专题                          60
来源：http://is.hnjuh.cn

T 其他语言补充                          60
来源：http://qg.panjiajie.cn

U 高频实用片段                         120
来源：http://jz.shxzskj.cn

------------------------------------
来源：http://qd.wgjwhj.cn

合计                                  2106 条
来源：http://km.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://np.gzmigu.cn

使用提醒
来源：http://eh.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://ys.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mn.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://av.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xi.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://so.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://js.colortex.cn

—— 文件结束 ——
来源：http://kq.jctech888.com.cn

================================================================================
来源：http://mq.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://hl.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://bb.hahajie.cn

================================================================================
来源：http://se.bookmarksfly.cn

【收录内容】
来源：http://ym.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rv.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mj.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://th.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ub.jianghongdianzi.cn

【使用说明】
来源：http://zz.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sa.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hu.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tm.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ns.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sj.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://au.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pa.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jp.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lc.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wv.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sl.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mp.asd995.cn

【文件统计】
来源：http://xo.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fe.asd995.cn

--------------------------------------------------------------------------------
来源：http://ja.9csxet.cn

目  录
来源：http://fu.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://qy.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xa.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fh.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://po.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xb.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qi.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bz.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jy.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://er.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yg.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wn.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yv.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://co.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ty.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lx.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rj.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kd.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hq.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://em.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mi.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zk.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xz.panjiajie.cn

================================================================================
来源：http://fz.newstarts.cn

A. 基础语法与类型
来源：http://ux.wgjwhj.cn

================================================================================
来源：http://vg.jctech888.com.cn

[A01] Hello World
来源：http://dp.hahajie.cn

Py:   print("Hello, World!")
来源：http://hf.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://wt.521024.cn

JS:   console.log("Hello, World!");
来源：http://du.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vv.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://ah.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://ep.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://gf.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rh.asd995.cn

[A02] 变量声明与赋值
来源：http://ev.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ci.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bf.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kj.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kw.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://ty.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://mc.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://jm.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://as.hnjuh.cn

[A03] 常量定义
来源：http://ii.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oh.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://cu.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://yt.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://nt.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://jc.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://ya.colortex.cn


<!-- 参考信息 -->