代发 wailian999

[U35] Py：发送邮件
来源：http://sf.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://br.asd995.cn

[U36] Py：定时任务
来源：http://du.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://hh.hahajie.cn

[U37] Py：读写 Excel
来源：http://xs.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://de.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://us.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://oh.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://sh.huixiangedu.cn

sys.stdout.isatty()
来源：http://rl.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://ra.huanxung.cn

print("err", file=sys.stderr)
来源：http://so.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://rk.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rr.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://sq.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fe.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://tb.shxzskj.cn

namespace App\Http;
来源：http://fy.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://kj.gzmigu.cn

declare(strict_types=1);
来源：http://pg.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://xi.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mj.bjjhwx.cn

[U46] PHP：可空类型
来源：http://nl.shxzukj.cn

?string $name = null
来源：http://zx.colortex.cn

[U47] PHP：联合类型
来源：http://uj.nszjky.cn

int|string $id
来源：http://pd.szsharing.cn

[U48] PHP：纯枚举
来源：http://nv.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fb.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://br.hnjuh.cn

public readonly string $name
来源：http://pt.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://fw.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://fb.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://eu.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://gu.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://zv.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://xp.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://dv.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://tf.szsharing.cn

[U54] PHP：空安全调用
来源：http://sh.lnxyls.cn

$obj?->method()
来源：http://hp.panjiajie.cn

[U55] PHP：match 表达式
来源：http://db.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uv.shtwfgs.cn

[U56] PHP：命名参数
来源：http://ad.colortex.cn

f(a: 1, b: 2)
来源：http://da.nszjky.cn

[U57] PHP：字符串插值
来源：http://ph.szsharing.cn

"值: {$a}"
来源：http://iv.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://sg.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cy.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://ow.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bu.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://rk.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ll.yuntaijiaju.cn

[U61] PHP：正则
来源：http://sp.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jn.nszjky.cn

[U62] PHP：日期对象
来源：http://cx.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nr.nicolike.cn

[U63] PHP：文件读写
来源：http://rb.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kg.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://we.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://yi.521024.cn

[U65] PHP：会话
来源：http://if.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ng.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://ga.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aa.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://sz.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vy.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://gw.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sr.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://lm.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fd.hahajie.cn

[U70] PHP：PDO 事务
来源：http://wq.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://df.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://lj.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://qy.shxzskj.cn

[U72] PHP：写错误日志
来源：http://wo.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://hl.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://is.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://qp.szsharing.cn

[U74] PHP：读取环境变量
来源：http://cl.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://vv.huanxung.cn

[U75] PHP：依赖注入
来源：http://ca.9csxet.cn

composer require psr/container
来源：http://gu.asd995.cn

[U76] PHP：简单路由
来源：http://ry.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zg.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://df.shtwfgs.cn

composer require twig/twig
来源：http://oo.hahajie.cn

[U78] PHP：单元测试
来源：http://lx.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://oh.newstarts.cn

[U79] PHP：静态分析
来源：http://ue.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://sa.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://bw.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fx.wgjwhj.cn

[U81] JS：初始化项目
来源：http://gq.nszjky.cn

npm init -y;  npm i express
来源：http://fm.newstarts.cn

[U82] JS：package.json 脚本
来源：http://bd.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gt.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://tp.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vh.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://oh.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fg.chemitech.net.cn

[U85] JS：可选链
来源：http://hv.shtwfgs.cn

a?.b?.c
来源：http://kz.jctech888.com.cn

[U86] JS：空值合并
来源：http://cv.nicolike.cn

a ?? b
来源：http://ky.521024.cn

[U87] JS：解构默认值
来源：http://hb.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://ou.9csxet.cn

[U88] JS：对象展开合并
来源：http://wh.9csxet.cn

{ ...a, ...b }
来源：http://rg.panjiajie.cn

[U89] JS：数组去重
来源：http://ch.shxzukj.cn

[...new Set(arr)]
来源：http://sd.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://kx.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://oj.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://ya.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cw.szxytkj.cn

[U92] JS：深拷贝
来源：http://sj.huanxung.cn

structuredClone(obj)
来源：http://wg.gzmigu.cn

[U93] JS：模板字符串
来源：http://nt.521024.cn

`共 ${n} 条`
来源：http://bq.szsharing.cn

[U94] JS：箭头函数
来源：http://dt.newstarts.cn

const double = x => x * 2;
来源：http://to.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://yb.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://eb.asd995.cn

[U96] JS：async/await 与异常
来源：http://us.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://on.newstarts.cn

[U97] JS：并发请求
来源：http://ot.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hg.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://pd.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ga.szxytkj.cn

[U99] JS：事件监听
来源：http://um.nicolike.cn

el.addEventListener("click", e => {})
来源：http://rk.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://lu.nszjky.cn

document.querySelector(".item")
来源：http://kq.chemitech.net.cn

[U101] JS：classList 操作
来源：http://we.yuexingan06.cn

el.classList.toggle("active")
来源：http://rf.nicolike.cn

[U102] JS：本地存储
来源：http://um.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kw.lnxyls.cn

[U103] JS：定时器
来源：http://my.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pu.hahajie.cn

[U104] JS：防抖
来源：http://fj.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://km.521024.cn

[U105] JS：节流
来源：http://nw.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jy.bjjhwx.cn

[U106] JS：日期格式化
来源：http://tb.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xh.huixiangedu.cn

[U107] JS：数字千分位
来源：http://zs.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cc.haigaiapp.cn

[U108] JS：随机整数
来源：http://yv.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nx.shxzukj.cn

[U109] JS：数组分组
来源：http://xw.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://ie.szsharing.cn

[U110] JS：数组分块
来源：http://hp.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bn.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://qb.panjiajie.cn

new Map(Object.entries(obj))
来源：http://vf.newstarts.cn

[U112] JS：字符串补位
来源：http://ry.521024.cn

"7".padStart(3, "0")
来源：http://kd.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://fr.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://vy.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://kn.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wt.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://if.chemitech.net.cn

crypto.randomUUID()
来源：http://tq.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://dr.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://ip.haigaiapp.cn

[U117] JS：单元测试
来源：http://ui.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://pf.szsharing.cn

[U118] JS：开发服务器
来源：http://yi.huanxung.cn

npm i -D vite;  npx vite
来源：http://wx.521024.cn

[U119] JS：生产构建
来源：http://xc.lnxyls.cn

npx vite build
来源：http://nx.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://do.asd995.cn

import.meta.env.VITE_API_URL
来源：http://rs.bookmarksfly.cn

================================================================================
来源：http://bo.nszjky.cn

统计汇总
来源：http://fr.jctech888.com.cn

================================================================================
来源：http://ja.shxzskj.cn

按语言统计（条）：
来源：http://qn.chemitech.net.cn

Python ......... 252
来源：http://ve.521024.cn

PHP ............ 252
来源：http://fp.lnxyls.cn

JavaScript ..... 252
来源：http://vv.jctech888.com.cn

TypeScript ..... 212
来源：http://up.asd995.cn

Java ........... 212
来源：http://ha.jianghongdianzi.cn

Go ............. 212
来源：http://id.huixinmuqiang.cn

Ruby ........... 212
来源：http://sp.huixinmuqiang.cn

C# ............. 212
来源：http://op.huixinmuqiang.cn

C .............. 30
来源：http://hp.shxzukj.cn

C++ ............ 30
来源：http://hu.nicolike.cn

SQL ............ 90
来源：http://nd.hahajie.cn

Bash ........... 80
来源：http://no.yuexingan06.cn

Kotlin ......... 15
来源：http://qo.huixinmuqiang.cn

Swift .......... 15
来源：http://oa.newstarts.cn

Lua ............ 10
来源：http://vf.panjiajie.cn

Perl ........... 10
来源：http://jt.521024.cn

Scala .......... 10
来源：http://yh.shxzskj.cn

------------------------------------
来源：http://kl.shtwfgs.cn

合计 ........... 2106 条
来源：http://gl.bjjhwx.cn

按章节统计：
来源：http://fw.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xu.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rr.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://al.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jt.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ht.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yh.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://np.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://me.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yj.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eb.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gr.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mt.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://al.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cf.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ka.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://is.szxytkj.cn

Q SQL 专题                              90
来源：http://nh.szxytkj.cn

R Bash 专题                             80
来源：http://ma.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://dy.huixiangedu.cn

T 其他语言补充                          60
来源：http://bv.szsharing.cn

U 高频实用片段                         120
来源：http://ji.yuexingan06.cn

------------------------------------
来源：http://wl.bookmarksfly.cn

合计                                  2106 条
来源：http://et.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://oj.huixiangedu.cn

使用提醒
来源：http://ux.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://bj.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iq.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://er.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bg.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://aj.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ze.hnjuh.cn

—— 文件结束 ——
来源：http://sz.huanxung.cn

================================================================================
来源：http://en.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://ru.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://et.huanxung.cn

================================================================================
来源：http://jv.yuntaijiaju.cn

【收录内容】
来源：http://bs.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ik.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qy.szsharing.cn

SQL · Bash · C · C++
来源：http://pn.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wy.haigaiapp.cn

【使用说明】
来源：http://nk.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fm.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://px.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pg.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fi.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://in.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://up.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nl.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ev.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wn.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wr.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mg.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hh.wgjwhj.cn

【文件统计】
来源：http://kg.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sd.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://tj.newstarts.cn

目  录
来源：http://bw.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://gs.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gs.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://km.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sb.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zm.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ru.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fh.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uh.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qh.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pt.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eh.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rn.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vj.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dw.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yl.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sj.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ic.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ug.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://id.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ma.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kc.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qw.huixinmuqiang.cn

================================================================================
来源：http://pf.szxytkj.cn

A. 基础语法与类型
来源：http://ye.shxzukj.cn

================================================================================
来源：http://wm.shxzukj.cn

[A01] Hello World
来源：http://gi.panjiajie.cn

Py:   print("Hello, World!")
来源：http://pb.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://zf.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://rm.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tm.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://fg.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://gp.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://qx.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gx.hnjuh.cn

[A02] 变量声明与赋值
来源：http://us.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gr.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wu.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ke.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jn.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://mm.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://wf.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://fl.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ye.huanxung.cn

[A03] 常量定义
来源：http://ru.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uo.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://qh.colortex.cn


<!-- 参考信息 -->