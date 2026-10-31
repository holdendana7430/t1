代发 wailian999

[U33] Py：打包发布
来源：http://mz.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://tl.jctech888.com.cn

[U34] Py：判断编码
来源：http://ou.szsharing.cn

chardet.detect(raw)
来源：http://pg.bjjhwx.cn

[U35] Py：发送邮件
来源：http://qq.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://id.huanxung.cn

[U36] Py：定时任务
来源：http://tn.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://vx.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://nx.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zg.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://pw.gzmigu.cn

Path(__file__).resolve().parent
来源：http://uf.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://cw.asd995.cn

sys.stdout.isatty()
来源：http://mc.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://ri.newstarts.cn

print("err", file=sys.stderr)
来源：http://wj.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://wr.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dq.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://me.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gf.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://wh.bjjhwx.cn

namespace App\Http;
来源：http://ak.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://aj.yuexingan06.cn

declare(strict_types=1);
来源：http://bh.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://tb.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ir.panjiajie.cn

[U46] PHP：可空类型
来源：http://nz.haigaiapp.cn

?string $name = null
来源：http://ro.9csxet.cn

[U47] PHP：联合类型
来源：http://bg.szsharing.cn

int|string $id
来源：http://th.shxzskj.cn

[U48] PHP：纯枚举
来源：http://kw.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pk.yuexingan06.cn

[U49] PHP：只读属性
来源：http://kc.9csxet.cn

public readonly string $name
来源：http://an.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://sq.hahajie.cn

public function __construct(private int $id) {}
来源：http://bx.huixiangedu.cn

[U51] PHP：数组解构
来源：http://nj.9csxet.cn

[$a, $b] = $arr;
来源：http://hr.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://ti.asd995.cn

$double = fn($x) => $x * 2;
来源：http://ht.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://jm.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://lb.521024.cn

[U54] PHP：空安全调用
来源：http://dd.huixinmuqiang.cn

$obj?->method()
来源：http://rp.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://tc.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ue.haigaiapp.cn

[U56] PHP：命名参数
来源：http://ha.hahajie.cn

f(a: 1, b: 2)
来源：http://un.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://hn.hnjuh.cn

"值: {$a}"
来源：http://nt.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://vv.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ed.szsharing.cn

[U59] PHP：自定义排序
来源：http://qz.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wc.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://lc.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sb.asd995.cn

[U61] PHP：正则
来源：http://et.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yc.chemitech.net.cn

[U62] PHP：日期对象
来源：http://em.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hv.yuexingan06.cn

[U63] PHP：文件读写
来源：http://tm.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dv.panjiajie.cn

[U64] PHP：目录遍历
来源：http://bu.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://jo.szxytkj.cn

[U65] PHP：会话
来源：http://xr.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hp.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://jc.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yv.521024.cn

[U67] PHP：处理文件上传
来源：http://rr.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sr.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://nk.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xr.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://uo.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yr.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://aq.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qo.colortex.cn

[U71] PHP：抛出异常
来源：http://bo.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://wk.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://qk.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://yd.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://dx.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://bi.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://tw.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://lm.nszjky.cn

[U75] PHP：依赖注入
来源：http://gd.yuexingan06.cn

composer require psr/container
来源：http://qm.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://jd.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ls.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://hl.newstarts.cn

composer require twig/twig
来源：http://hr.wgjwhj.cn

[U78] PHP：单元测试
来源：http://fj.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://sf.huanxung.cn

[U79] PHP：静态分析
来源：http://gb.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://nu.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://zk.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yx.szsharing.cn

[U81] JS：初始化项目
来源：http://mg.bjjhwx.cn

npm init -y;  npm i express
来源：http://ss.asd995.cn

[U82] JS：package.json 脚本
来源：http://ks.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wt.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://zk.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hr.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://bn.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nw.hahajie.cn

[U85] JS：可选链
来源：http://vd.lnxyls.cn

a?.b?.c
来源：http://xz.bjjhwx.cn

[U86] JS：空值合并
来源：http://yp.muxihuayi.cn

a ?? b
来源：http://op.huanxung.cn

[U87] JS：解构默认值
来源：http://dq.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://ml.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://wd.9csxet.cn

{ ...a, ...b }
来源：http://zc.gzmigu.cn

[U89] JS：数组去重
来源：http://ni.9csxet.cn

[...new Set(arr)]
来源：http://jj.szxytkj.cn

[U90] JS：数字数组排序
来源：http://tm.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://iv.nicolike.cn

[U91] JS：对象键值遍历
来源：http://ua.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xj.bjjhwx.cn

[U92] JS：深拷贝
来源：http://ny.shxzskj.cn

structuredClone(obj)
来源：http://ug.wgjwhj.cn

[U93] JS：模板字符串
来源：http://wy.asd995.cn

`共 ${n} 条`
来源：http://ha.chemitech.net.cn

[U94] JS：箭头函数
来源：http://at.lnxyls.cn

const double = x => x * 2;
来源：http://gu.newstarts.cn

[U95] JS：Promise 包装
来源：http://tu.521024.cn

new Promise((resolve, reject) => {})
来源：http://ow.hahajie.cn

[U96] JS：async/await 与异常
来源：http://oo.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rc.bjjhwx.cn

[U97] JS：并发请求
来源：http://pv.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ig.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://kg.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mm.shxzukj.cn

[U99] JS：事件监听
来源：http://pc.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://qn.asd995.cn

[U100] JS：DOM 查询
来源：http://pt.szxytkj.cn

document.querySelector(".item")
来源：http://jb.521024.cn

[U101] JS：classList 操作
来源：http://jn.nicolike.cn

el.classList.toggle("active")
来源：http://dt.lnxyls.cn

[U102] JS：本地存储
来源：http://rw.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://au.chemitech.net.cn

[U103] JS：定时器
来源：http://yd.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uo.huixiangedu.cn

[U104] JS：防抖
来源：http://hr.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nc.hahajie.cn

[U105] JS：节流
来源：http://uz.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ny.szxytkj.cn

[U106] JS：日期格式化
来源：http://lp.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bg.colortex.cn

[U107] JS：数字千分位
来源：http://za.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zr.szsharing.cn

[U108] JS：随机整数
来源：http://mw.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cx.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://oq.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://xr.shtwfgs.cn

[U110] JS：数组分块
来源：http://nl.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ne.shxzskj.cn

[U111] JS：对象转 Map
来源：http://ui.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://sl.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://sy.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://ev.szsharing.cn

[U113] JS：正则替换全部
来源：http://nm.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://lp.newstarts.cn

[U114] JS：JSON 深比较
来源：http://wv.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hv.shxzukj.cn

[U115] JS：生成 UUID
来源：http://ba.bookmarksfly.cn

crypto.randomUUID()
来源：http://sv.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://ei.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://dr.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://xb.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://dm.shtwfgs.cn

[U118] JS：开发服务器
来源：http://gf.nszjky.cn

npm i -D vite;  npx vite
来源：http://li.wgjwhj.cn

[U119] JS：生产构建
来源：http://ea.nszjky.cn

npx vite build
来源：http://ez.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://zi.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://mi.9csxet.cn

================================================================================
来源：http://ea.haigaiapp.cn

统计汇总
来源：http://sk.nszjky.cn

================================================================================
来源：http://vv.shtwfgs.cn

按语言统计（条）：
来源：http://jo.shxzskj.cn

Python ......... 252
来源：http://gc.jctech888.com.cn

PHP ............ 252
来源：http://qe.asd995.cn

JavaScript ..... 252
来源：http://qp.yuntaijiaju.cn

TypeScript ..... 212
来源：http://jb.yuexingan06.cn

Java ........... 212
来源：http://bg.haigaiapp.cn

Go ............. 212
来源：http://mx.jianghongdianzi.cn

Ruby ........... 212
来源：http://ep.nicolike.cn

C# ............. 212
来源：http://dd.huixiangedu.cn

C .............. 30
来源：http://xj.gzmigu.cn

C++ ............ 30
来源：http://oe.muxihuayi.cn

SQL ............ 90
来源：http://ij.gzmigu.cn

Bash ........... 80
来源：http://vo.haigaiapp.cn

Kotlin ......... 15
来源：http://bm.huixinmuqiang.cn

Swift .......... 15
来源：http://sw.newstarts.cn

Lua ............ 10
来源：http://od.huixiangedu.cn

Perl ........... 10
来源：http://cl.jianghongdianzi.cn

Scala .......... 10
来源：http://cz.szxytkj.cn

------------------------------------
来源：http://oo.shtwfgs.cn

合计 ........... 2106 条
来源：http://uo.bjjhwx.cn

按章节统计：
来源：http://uc.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qu.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cp.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rd.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kb.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kb.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fr.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xh.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jb.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oq.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uk.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hl.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mr.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rq.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hd.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ll.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qn.wgjwhj.cn

Q SQL 专题                              90
来源：http://wf.nicolike.cn

R Bash 专题                             80
来源：http://gn.hnjuh.cn

S C / C++ 专题                          60
来源：http://vq.hnjuh.cn

T 其他语言补充                          60
来源：http://fg.newstarts.cn

U 高频实用片段                         120
来源：http://ga.hnjuh.cn

------------------------------------
来源：http://as.szxytkj.cn

合计                                  2106 条
来源：http://yp.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://zy.yuntaijiaju.cn

使用提醒
来源：http://fu.nicolike.cn

--------------------------------------------------------------------------------
来源：http://yo.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xm.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bw.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://te.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://re.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vq.chemitech.net.cn

—— 文件结束 ——
来源：http://xc.shxzukj.cn

================================================================================
来源：http://ez.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://gz.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://ab.szsharing.cn

================================================================================
来源：http://ft.yuntaijiaju.cn

【收录内容】
来源：http://ms.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gp.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tt.wgjwhj.cn

SQL · Bash · C · C++
来源：http://bc.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wo.colortex.cn

【使用说明】
来源：http://gx.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tl.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ei.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fo.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://th.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ah.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pk.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://op.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mb.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://df.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ow.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ry.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mf.yuntaijiaju.cn

【文件统计】
来源：http://hz.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xc.521024.cn

--------------------------------------------------------------------------------
来源：http://lh.shxzukj.cn

目  录
来源：http://ae.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://tb.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ge.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wu.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pc.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gn.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hl.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mo.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xm.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vq.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eu.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bn.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mt.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://py.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wk.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kw.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cc.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qq.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zz.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mr.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ew.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://da.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nz.nszjky.cn

================================================================================
来源：http://fa.nicolike.cn

A. 基础语法与类型
来源：http://bh.hahajie.cn

================================================================================
来源：http://jr.521024.cn

[A01] Hello World
来源：http://vb.shxzukj.cn

Py:   print("Hello, World!")
来源：http://ll.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://oj.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://ho.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://za.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://ut.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://vb.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://vk.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mg.nszjky.cn

[A02] 变量声明与赋值
来源：http://kj.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mv.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://om.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qw.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eo.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://wr.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://iy.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://fe.hnjuh.cn


<!-- 参考信息 -->