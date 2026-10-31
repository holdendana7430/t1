代发 wailian999

[U35] Py：发送邮件
来源：http://du.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rg.asd995.cn

[U36] Py：定时任务
来源：http://gs.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://qi.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://lh.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hl.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://ak.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://nm.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://fb.szxytkj.cn

sys.stdout.isatty()
来源：http://bx.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://lu.hahajie.cn

print("err", file=sys.stderr)
来源：http://jb.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://kw.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lg.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://gr.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sw.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://pv.jianghongdianzi.cn

namespace App\Http;
来源：http://yh.szsharing.cn

[U44] PHP：开启严格类型
来源：http://mb.521024.cn

declare(strict_types=1);
来源：http://hg.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://dr.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yp.hahajie.cn

[U46] PHP：可空类型
来源：http://nh.bjjhwx.cn

?string $name = null
来源：http://su.nicolike.cn

[U47] PHP：联合类型
来源：http://cc.nszjky.cn

int|string $id
来源：http://bq.gzmigu.cn

[U48] PHP：纯枚举
来源：http://hx.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aa.yuexingan06.cn

[U49] PHP：只读属性
来源：http://te.huanxung.cn

public readonly string $name
来源：http://uj.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://xw.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://as.shxzukj.cn

[U51] PHP：数组解构
来源：http://vu.9csxet.cn

[$a, $b] = $arr;
来源：http://tt.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://xp.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://qr.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://sa.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://ab.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://zm.gzmigu.cn

$obj?->method()
来源：http://oh.newstarts.cn

[U55] PHP：match 表达式
来源：http://wc.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ns.shxzskj.cn

[U56] PHP：命名参数
来源：http://fs.nicolike.cn

f(a: 1, b: 2)
来源：http://ra.521024.cn

[U57] PHP：字符串插值
来源：http://tm.jctech888.com.cn

"值: {$a}"
来源：http://ct.colortex.cn

[U58] PHP：数组三件套
来源：http://ow.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xr.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://nh.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ma.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://wh.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://de.yuexingan06.cn

[U61] PHP：正则
来源：http://df.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://st.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://yu.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tn.lnxyls.cn

[U63] PHP：文件读写
来源：http://zf.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ky.521024.cn

[U64] PHP：目录遍历
来源：http://nl.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://sv.nszjky.cn

[U65] PHP：会话
来源：http://ah.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://my.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://kb.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ek.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://mf.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://in.nicolike.cn

[U68] PHP：PDO 连接
来源：http://zt.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ck.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://wj.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://it.nszjky.cn

[U70] PHP：PDO 事务
来源：http://mi.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fn.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://kd.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://za.hnjuh.cn

[U72] PHP：写错误日志
来源：http://hd.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://uq.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://id.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://qq.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://rt.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://df.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://lr.szsharing.cn

composer require psr/container
来源：http://wn.panjiajie.cn

[U76] PHP：简单路由
来源：http://hs.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uv.asd995.cn

[U77] PHP：模板渲染
来源：http://mo.wgjwhj.cn

composer require twig/twig
来源：http://jk.bjjhwx.cn

[U78] PHP：单元测试
来源：http://he.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://qo.jctech888.com.cn

[U79] PHP：静态分析
来源：http://oo.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://bq.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://nx.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ec.gzmigu.cn

[U81] JS：初始化项目
来源：http://ct.hnjuh.cn

npm init -y;  npm i express
来源：http://gu.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://ai.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://af.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://tx.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gc.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://pp.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fi.panjiajie.cn

[U85] JS：可选链
来源：http://xk.newstarts.cn

a?.b?.c
来源：http://do.9csxet.cn

[U86] JS：空值合并
来源：http://lg.jianghongdianzi.cn

a ?? b
来源：http://zn.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://gd.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://so.521024.cn

[U88] JS：对象展开合并
来源：http://vt.colortex.cn

{ ...a, ...b }
来源：http://pc.muxihuayi.cn

[U89] JS：数组去重
来源：http://ny.haigaiapp.cn

[...new Set(arr)]
来源：http://pm.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://vx.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://ux.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://xu.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://de.hahajie.cn

[U92] JS：深拷贝
来源：http://sy.huixiangedu.cn

structuredClone(obj)
来源：http://bz.bjjhwx.cn

[U93] JS：模板字符串
来源：http://sx.haigaiapp.cn

`共 ${n} 条`
来源：http://jz.nszjky.cn

[U94] JS：箭头函数
来源：http://vl.jianghongdianzi.cn

const double = x => x * 2;
来源：http://zm.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://oc.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://rh.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://kc.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nd.bookmarksfly.cn

[U97] JS：并发请求
来源：http://oq.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gw.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://dy.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ym.gzmigu.cn

[U99] JS：事件监听
来源：http://gc.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://zf.panjiajie.cn

[U100] JS：DOM 查询
来源：http://cp.jctech888.com.cn

document.querySelector(".item")
来源：http://ws.colortex.cn

[U101] JS：classList 操作
来源：http://af.muxihuayi.cn

el.classList.toggle("active")
来源：http://gx.panjiajie.cn

[U102] JS：本地存储
来源：http://wi.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xg.nicolike.cn

[U103] JS：定时器
来源：http://kd.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tv.jianghongdianzi.cn

[U104] JS：防抖
来源：http://op.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mq.gzmigu.cn

[U105] JS：节流
来源：http://rt.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lx.muxihuayi.cn

[U106] JS：日期格式化
来源：http://et.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://je.lnxyls.cn

[U107] JS：数字千分位
来源：http://ki.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://on.szsharing.cn

[U108] JS：随机整数
来源：http://cv.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qj.lnxyls.cn

[U109] JS：数组分组
来源：http://hu.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://xe.szxytkj.cn

[U110] JS：数组分块
来源：http://ox.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pv.nicolike.cn

[U111] JS：对象转 Map
来源：http://ft.hahajie.cn

new Map(Object.entries(obj))
来源：http://ly.haigaiapp.cn

[U112] JS：字符串补位
来源：http://tb.yuexingan06.cn

"7".padStart(3, "0")
来源：http://jy.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://di.hahajie.cn

s.replaceAll("a", "b")
来源：http://tf.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://qy.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sk.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://qv.bookmarksfly.cn

crypto.randomUUID()
来源：http://vb.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://st.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://hl.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://ja.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://id.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://mx.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://be.colortex.cn

[U119] JS：生产构建
来源：http://iy.bookmarksfly.cn

npx vite build
来源：http://ad.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://do.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://xb.9csxet.cn

================================================================================
来源：http://sf.gzmigu.cn

统计汇总
来源：http://yg.chemitech.net.cn

================================================================================
来源：http://ut.jctech888.com.cn

按语言统计（条）：
来源：http://rr.gzmigu.cn

Python ......... 252
来源：http://dd.asd995.cn

PHP ............ 252
来源：http://ff.gzmigu.cn

JavaScript ..... 252
来源：http://sy.521024.cn

TypeScript ..... 212
来源：http://dw.colortex.cn

Java ........... 212
来源：http://rn.bjjhwx.cn

Go ............. 212
来源：http://to.shxzukj.cn

Ruby ........... 212
来源：http://eo.panjiajie.cn

C# ............. 212
来源：http://wj.szxytkj.cn

C .............. 30
来源：http://um.9csxet.cn

C++ ............ 30
来源：http://py.gzmigu.cn

SQL ............ 90
来源：http://fe.colortex.cn

Bash ........... 80
来源：http://jc.chemitech.net.cn

Kotlin ......... 15
来源：http://tm.panjiajie.cn

Swift .......... 15
来源：http://li.huanxung.cn

Lua ............ 10
来源：http://an.newstarts.cn

Perl ........... 10
来源：http://zq.wgjwhj.cn

Scala .......... 10
来源：http://qp.panjiajie.cn

------------------------------------
来源：http://lq.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://nt.jianghongdianzi.cn

按章节统计：
来源：http://gv.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ol.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ew.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wh.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pt.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jf.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vw.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kp.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mj.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://co.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rr.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ez.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://we.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zd.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://up.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ed.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ae.jctech888.com.cn

Q SQL 专题                              90
来源：http://il.bookmarksfly.cn

R Bash 专题                             80
来源：http://ck.huixiangedu.cn

S C / C++ 专题                          60
来源：http://fi.szxytkj.cn

T 其他语言补充                          60
来源：http://zg.haigaiapp.cn

U 高频实用片段                         120
来源：http://xo.huixinmuqiang.cn

------------------------------------
来源：http://ya.szsharing.cn

合计                                  2106 条
来源：http://ba.asd995.cn

--------------------------------------------------------------------------------
来源：http://fa.hahajie.cn

使用提醒
来源：http://hp.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://yt.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ol.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qj.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zu.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sn.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cq.shxzskj.cn

—— 文件结束 ——
来源：http://vg.nszjky.cn

================================================================================
来源：http://zo.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://hd.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://sd.nicolike.cn

================================================================================
来源：http://ds.hahajie.cn

【收录内容】
来源：http://ax.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dc.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pz.newstarts.cn

SQL · Bash · C · C++
来源：http://fb.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pd.bjjhwx.cn

【使用说明】
来源：http://qu.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vz.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mz.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mp.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eg.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://or.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bi.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://is.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sm.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sd.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://so.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nx.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hc.gzmigu.cn

【文件统计】
来源：http://jj.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zy.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://xk.huixinmuqiang.cn

目  录
来源：http://ou.521024.cn

--------------------------------------------------------------------------------
来源：http://uz.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lt.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bv.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yk.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uo.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rd.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dk.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wi.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://az.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mi.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mn.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zp.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vj.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rz.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fm.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mg.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yl.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ea.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zn.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yr.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qj.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://du.yuexingan06.cn

================================================================================
来源：http://yh.bjjhwx.cn

A. 基础语法与类型
来源：http://bo.chemitech.net.cn

================================================================================
来源：http://pf.yuntaijiaju.cn

[A01] Hello World
来源：http://xi.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://ol.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://hf.521024.cn

JS:   console.log("Hello, World!");
来源：http://pp.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ho.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://tj.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://fc.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://bk.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nt.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://vr.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kl.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ov.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://er.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bi.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ox.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://yr.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://lj.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hf.muxihuayi.cn

[A03] 常量定义
来源：http://zo.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gx.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://yz.bookmarksfly.cn


<!-- 参考信息 -->