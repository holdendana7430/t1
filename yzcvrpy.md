代发 wailian999

[U33] Py：打包发布
来源：http://vh.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://iw.521024.cn

[U34] Py：判断编码
来源：http://by.jctech888.com.cn

chardet.detect(raw)
来源：http://hg.yuexingan06.cn

[U35] Py：发送邮件
来源：http://oa.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://js.chemitech.net.cn

[U36] Py：定时任务
来源：http://ul.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://nq.newstarts.cn

[U37] Py：读写 Excel
来源：http://cp.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lq.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://fo.szsharing.cn

Path(__file__).resolve().parent
来源：http://hf.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://tx.wgjwhj.cn

sys.stdout.isatty()
来源：http://xp.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://oj.gzmigu.cn

print("err", file=sys.stderr)
来源：http://ol.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://up.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hf.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://ch.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mi.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://ml.nszjky.cn

namespace App\Http;
来源：http://aa.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://rz.szxytkj.cn

declare(strict_types=1);
来源：http://xq.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://xa.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vg.hnjuh.cn

[U46] PHP：可空类型
来源：http://nl.9csxet.cn

?string $name = null
来源：http://mh.lnxyls.cn

[U47] PHP：联合类型
来源：http://dz.jianghongdianzi.cn

int|string $id
来源：http://ah.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://ir.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fo.hnjuh.cn

[U49] PHP：只读属性
来源：http://af.9csxet.cn

public readonly string $name
来源：http://sv.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://mf.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://on.panjiajie.cn

[U51] PHP：数组解构
来源：http://yj.asd995.cn

[$a, $b] = $arr;
来源：http://ge.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://lk.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://kr.nicolike.cn

[U53] PHP：空合并运算符
来源：http://ex.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://tp.hahajie.cn

[U54] PHP：空安全调用
来源：http://as.panjiajie.cn

$obj?->method()
来源：http://np.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://gg.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sm.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://yj.hnjuh.cn

f(a: 1, b: 2)
来源：http://rf.shxzukj.cn

[U57] PHP：字符串插值
来源：http://ox.szsharing.cn

"值: {$a}"
来源：http://ck.9csxet.cn

[U58] PHP：数组三件套
来源：http://bu.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cc.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://hp.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ia.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://zs.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xe.panjiajie.cn

[U61] PHP：正则
来源：http://tb.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://za.9csxet.cn

[U62] PHP：日期对象
来源：http://lg.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://as.shxzukj.cn

[U63] PHP：文件读写
来源：http://jo.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gv.nszjky.cn

[U64] PHP：目录遍历
来源：http://yz.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://cd.hnjuh.cn

[U65] PHP：会话
来源：http://fq.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kj.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://in.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sy.9csxet.cn

[U67] PHP：处理文件上传
来源：http://at.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://im.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://ok.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qr.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://jd.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ur.asd995.cn

[U70] PHP：PDO 事务
来源：http://rr.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rb.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://lw.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://pe.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://zo.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://bz.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://hm.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://mb.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://cl.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://fg.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://oy.muxihuayi.cn

composer require psr/container
来源：http://sb.hnjuh.cn

[U76] PHP：简单路由
来源：http://cd.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://px.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://bp.huanxung.cn

composer require twig/twig
来源：http://tp.9csxet.cn

[U78] PHP：单元测试
来源：http://dg.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://oe.huanxung.cn

[U79] PHP：静态分析
来源：http://ut.asd995.cn

composer require --dev phpstan/phpstan
来源：http://xw.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://tk.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://of.shxzskj.cn

[U81] JS：初始化项目
来源：http://zl.jctech888.com.cn

npm init -y;  npm i express
来源：http://hm.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://pn.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://we.521024.cn

[U83] JS：ES Module 导入导出
来源：http://xn.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://om.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://vg.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://te.bjjhwx.cn

[U85] JS：可选链
来源：http://qb.muxihuayi.cn

a?.b?.c
来源：http://le.huixiangedu.cn

[U86] JS：空值合并
来源：http://xs.gzmigu.cn

a ?? b
来源：http://zi.jctech888.com.cn

[U87] JS：解构默认值
来源：http://rq.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://mu.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://do.lnxyls.cn

{ ...a, ...b }
来源：http://qa.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://kr.yuexingan06.cn

[...new Set(arr)]
来源：http://ii.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://bw.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://lk.hahajie.cn

[U91] JS：对象键值遍历
来源：http://ev.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fw.newstarts.cn

[U92] JS：深拷贝
来源：http://yu.9csxet.cn

structuredClone(obj)
来源：http://jq.nszjky.cn

[U93] JS：模板字符串
来源：http://hs.9csxet.cn

`共 ${n} 条`
来源：http://ip.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://em.jctech888.com.cn

const double = x => x * 2;
来源：http://yt.nszjky.cn

[U95] JS：Promise 包装
来源：http://er.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://my.szsharing.cn

[U96] JS：async/await 与异常
来源：http://sl.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ci.nicolike.cn

[U97] JS：并发请求
来源：http://dr.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bm.521024.cn

[U98] JS：fetch 带 JSON
来源：http://ck.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qk.huanxung.cn

[U99] JS：事件监听
来源：http://bq.colortex.cn

el.addEventListener("click", e => {})
来源：http://hd.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://pv.haigaiapp.cn

document.querySelector(".item")
来源：http://ku.shxzukj.cn

[U101] JS：classList 操作
来源：http://br.panjiajie.cn

el.classList.toggle("active")
来源：http://vc.hnjuh.cn

[U102] JS：本地存储
来源：http://zy.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qa.nicolike.cn

[U103] JS：定时器
来源：http://nm.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://al.9csxet.cn

[U104] JS：防抖
来源：http://ai.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rn.jianghongdianzi.cn

[U105] JS：节流
来源：http://do.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jj.hahajie.cn

[U106] JS：日期格式化
来源：http://tz.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xs.haigaiapp.cn

[U107] JS：数字千分位
来源：http://rq.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zg.haigaiapp.cn

[U108] JS：随机整数
来源：http://fm.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nn.newstarts.cn

[U109] JS：数组分组
来源：http://si.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://oh.panjiajie.cn

[U110] JS：数组分块
来源：http://ir.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xu.nicolike.cn

[U111] JS：对象转 Map
来源：http://ju.szxytkj.cn

new Map(Object.entries(obj))
来源：http://pv.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://nd.huixiangedu.cn

"7".padStart(3, "0")
来源：http://li.newstarts.cn

[U113] JS：正则替换全部
来源：http://kc.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://ip.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://so.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bq.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://qg.nicolike.cn

crypto.randomUUID()
来源：http://nt.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://pg.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://nd.bjjhwx.cn

[U117] JS：单元测试
来源：http://ry.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://dq.shxzskj.cn

[U118] JS：开发服务器
来源：http://tz.huanxung.cn

npm i -D vite;  npx vite
来源：http://id.colortex.cn

[U119] JS：生产构建
来源：http://wp.chemitech.net.cn

npx vite build
来源：http://lr.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://xn.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://vv.wgjwhj.cn

================================================================================
来源：http://tm.jianghongdianzi.cn

统计汇总
来源：http://vt.hnjuh.cn

================================================================================
来源：http://nl.521024.cn

按语言统计（条）：
来源：http://cj.colortex.cn

Python ......... 252
来源：http://xm.yuntaijiaju.cn

PHP ............ 252
来源：http://lp.shtwfgs.cn

JavaScript ..... 252
来源：http://tw.colortex.cn

TypeScript ..... 212
来源：http://mu.bookmarksfly.cn

Java ........... 212
来源：http://gd.wgjwhj.cn

Go ............. 212
来源：http://iq.huixiangedu.cn

Ruby ........... 212
来源：http://dn.nicolike.cn

C# ............. 212
来源：http://gz.9csxet.cn

C .............. 30
来源：http://nt.asd995.cn

C++ ............ 30
来源：http://qo.huixinmuqiang.cn

SQL ............ 90
来源：http://ci.nicolike.cn

Bash ........... 80
来源：http://zf.wgjwhj.cn

Kotlin ......... 15
来源：http://wx.asd995.cn

Swift .......... 15
来源：http://wf.gzmigu.cn

Lua ............ 10
来源：http://hf.newstarts.cn

Perl ........... 10
来源：http://iz.shtwfgs.cn

Scala .......... 10
来源：http://ql.jctech888.com.cn

------------------------------------
来源：http://ao.hnjuh.cn

合计 ........... 2106 条
来源：http://bh.szxytkj.cn

按章节统计：
来源：http://tc.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ki.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yn.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cq.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xv.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qe.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gd.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gz.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fu.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xe.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ow.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rz.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cx.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dq.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://md.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oj.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cv.newstarts.cn

Q SQL 专题                              90
来源：http://ym.lnxyls.cn

R Bash 专题                             80
来源：http://wl.gzmigu.cn

S C / C++ 专题                          60
来源：http://cw.521024.cn

T 其他语言补充                          60
来源：http://pc.haigaiapp.cn

U 高频实用片段                         120
来源：http://xm.yuexingan06.cn

------------------------------------
来源：http://tr.chemitech.net.cn

合计                                  2106 条
来源：http://oy.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://gy.nszjky.cn

使用提醒
来源：http://pp.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://yc.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yz.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gw.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qa.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://aj.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rd.huanxung.cn

—— 文件结束 ——
来源：http://qh.huixiangedu.cn

================================================================================
来源：http://wr.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://mt.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://zq.huanxung.cn

================================================================================
来源：http://lc.nszjky.cn

【收录内容】
来源：http://xe.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://he.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xx.colortex.cn

SQL · Bash · C · C++
来源：http://qk.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ke.wgjwhj.cn

【使用说明】
来源：http://xb.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cq.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://my.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kb.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yi.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xz.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tn.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ub.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ug.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dl.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vz.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nb.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://le.muxihuayi.cn

【文件统计】
来源：http://ga.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ex.szsharing.cn

--------------------------------------------------------------------------------
来源：http://ux.bookmarksfly.cn

目  录
来源：http://qy.9csxet.cn

--------------------------------------------------------------------------------
来源：http://vj.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rw.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kx.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ka.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ca.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oe.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ok.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rr.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hx.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sb.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rp.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xe.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nw.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gc.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ef.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://or.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vy.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hn.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ys.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hr.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cz.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ym.yuexingan06.cn

================================================================================
来源：http://bz.shxzskj.cn

A. 基础语法与类型
来源：http://vp.bjjhwx.cn

================================================================================
来源：http://li.lnxyls.cn

[A01] Hello World
来源：http://db.shxzskj.cn

Py:   print("Hello, World!")
来源：http://jl.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://ms.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://yv.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qx.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://oc.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://eh.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://oz.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wc.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://mo.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bg.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pf.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dn.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ig.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://qd.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://qr.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://gv.yuntaijiaju.cn


<!-- 参考信息 -->