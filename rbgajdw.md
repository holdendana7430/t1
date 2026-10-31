代发 wailian999

[U31] Py：单测
来源：http://vl.nicolike.cn

python -m pytest -q
来源：http://ne.colortex.cn

[U32] Py：代码格式化
来源：http://rj.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://ic.nszjky.cn

[U33] Py：打包发布
来源：http://uv.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://mz.jctech888.com.cn

[U34] Py：判断编码
来源：http://pl.huixiangedu.cn

chardet.detect(raw)
来源：http://ec.hahajie.cn

[U35] Py：发送邮件
来源：http://mw.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hd.nicolike.cn

[U36] Py：定时任务
来源：http://df.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://nj.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://wl.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://na.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://ts.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://kc.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://qp.muxihuayi.cn

sys.stdout.isatty()
来源：http://yi.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://mm.panjiajie.cn

print("err", file=sys.stderr)
来源：http://sn.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://qf.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://by.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://vo.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kr.asd995.cn

[U43] PHP：声明命名空间
来源：http://lu.521024.cn

namespace App\Http;
来源：http://ww.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://zk.bjjhwx.cn

declare(strict_types=1);
来源：http://xc.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://zg.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yh.yuexingan06.cn

[U46] PHP：可空类型
来源：http://pt.huanxung.cn

?string $name = null
来源：http://pk.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://zf.szxytkj.cn

int|string $id
来源：http://kd.panjiajie.cn

[U48] PHP：纯枚举
来源：http://we.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zv.shxzskj.cn

[U49] PHP：只读属性
来源：http://bz.huanxung.cn

public readonly string $name
来源：http://tt.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://tf.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://jt.newstarts.cn

[U51] PHP：数组解构
来源：http://ma.asd995.cn

[$a, $b] = $arr;
来源：http://dn.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://xz.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://sf.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://yj.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ak.gzmigu.cn

[U54] PHP：空安全调用
来源：http://yt.hnjuh.cn

$obj?->method()
来源：http://pb.lnxyls.cn

[U55] PHP：match 表达式
来源：http://fr.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nm.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://ep.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://hz.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://aq.521024.cn

"值: {$a}"
来源：http://yi.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://qy.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oh.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://aj.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tw.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://dq.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://te.hahajie.cn

[U61] PHP：正则
来源：http://wv.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pa.haigaiapp.cn

[U62] PHP：日期对象
来源：http://vq.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pu.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://xe.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://fn.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://aj.shxzukj.cn

[U65] PHP：会话
来源：http://yy.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://we.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://re.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wx.hahajie.cn

[U67] PHP：处理文件上传
来源：http://kw.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rk.szsharing.cn

[U68] PHP：PDO 连接
来源：http://mw.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kg.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://ir.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zs.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://hu.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fp.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://in.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://fu.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://bf.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://bv.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://ij.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://zt.521024.cn

[U74] PHP：读取环境变量
来源：http://st.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://co.huanxung.cn

[U75] PHP：依赖注入
来源：http://bw.haigaiapp.cn

composer require psr/container
来源：http://sp.nicolike.cn

[U76] PHP：简单路由
来源：http://xx.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fc.huanxung.cn

[U77] PHP：模板渲染
来源：http://qj.shxzukj.cn

composer require twig/twig
来源：http://nd.szxytkj.cn

[U78] PHP：单元测试
来源：http://ka.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://dr.nicolike.cn

[U79] PHP：静态分析
来源：http://ps.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://bw.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://ms.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nq.yuexingan06.cn

[U81] JS：初始化项目
来源：http://ru.szxytkj.cn

npm init -y;  npm i express
来源：http://vq.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://om.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ph.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://pm.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zl.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://ak.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://et.wgjwhj.cn

[U85] JS：可选链
来源：http://gm.yuntaijiaju.cn

a?.b?.c
来源：http://sz.521024.cn

[U86] JS：空值合并
来源：http://bd.shxzskj.cn

a ?? b
来源：http://yc.nicolike.cn

[U87] JS：解构默认值
来源：http://ir.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://ig.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://td.asd995.cn

{ ...a, ...b }
来源：http://qe.panjiajie.cn

[U89] JS：数组去重
来源：http://ao.hnjuh.cn

[...new Set(arr)]
来源：http://un.nszjky.cn

[U90] JS：数字数组排序
来源：http://nf.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://fw.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://hg.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ir.shtwfgs.cn

[U92] JS：深拷贝
来源：http://na.gzmigu.cn

structuredClone(obj)
来源：http://kb.lnxyls.cn

[U93] JS：模板字符串
来源：http://hv.shtwfgs.cn

`共 ${n} 条`
来源：http://hh.jctech888.com.cn

[U94] JS：箭头函数
来源：http://wf.colortex.cn

const double = x => x * 2;
来源：http://jd.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://aj.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://ae.colortex.cn

[U96] JS：async/await 与异常
来源：http://no.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hf.nszjky.cn

[U97] JS：并发请求
来源：http://zb.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fj.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://nr.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hp.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://bd.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://kb.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://hq.9csxet.cn

document.querySelector(".item")
来源：http://qw.huanxung.cn

[U101] JS：classList 操作
来源：http://pb.lnxyls.cn

el.classList.toggle("active")
来源：http://it.nszjky.cn

[U102] JS：本地存储
来源：http://ev.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gl.yuexingan06.cn

[U103] JS：定时器
来源：http://ig.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yv.nszjky.cn

[U104] JS：防抖
来源：http://uf.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iu.521024.cn

[U105] JS：节流
来源：http://au.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ax.szxytkj.cn

[U106] JS：日期格式化
来源：http://ai.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yz.huanxung.cn

[U107] JS：数字千分位
来源：http://af.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nw.panjiajie.cn

[U108] JS：随机整数
来源：http://vc.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wf.lnxyls.cn

[U109] JS：数组分组
来源：http://qh.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://ir.hnjuh.cn

[U110] JS：数组分块
来源：http://cl.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://we.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://zz.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://cy.chemitech.net.cn

[U112] JS：字符串补位
来源：http://av.hnjuh.cn

"7".padStart(3, "0")
来源：http://jd.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://uq.shxzskj.cn

s.replaceAll("a", "b")
来源：http://zd.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://ie.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aj.asd995.cn

[U115] JS：生成 UUID
来源：http://rg.colortex.cn

crypto.randomUUID()
来源：http://zx.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://op.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://nl.chemitech.net.cn

[U117] JS：单元测试
来源：http://pt.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://hr.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://zv.hahajie.cn

npm i -D vite;  npx vite
来源：http://gu.9csxet.cn

[U119] JS：生产构建
来源：http://ob.jianghongdianzi.cn

npx vite build
来源：http://ws.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://dx.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://sl.huixinmuqiang.cn

================================================================================
来源：http://gp.bjjhwx.cn

统计汇总
来源：http://fj.panjiajie.cn

================================================================================
来源：http://ds.asd995.cn

按语言统计（条）：
来源：http://qs.muxihuayi.cn

Python ......... 252
来源：http://tn.lnxyls.cn

PHP ............ 252
来源：http://io.hahajie.cn

JavaScript ..... 252
来源：http://qg.yuexingan06.cn

TypeScript ..... 212
来源：http://nu.9csxet.cn

Java ........... 212
来源：http://fz.bjjhwx.cn

Go ............. 212
来源：http://qp.shtwfgs.cn

Ruby ........... 212
来源：http://pu.panjiajie.cn

C# ............. 212
来源：http://ee.9csxet.cn

C .............. 30
来源：http://xa.chemitech.net.cn

C++ ............ 30
来源：http://ah.9csxet.cn

SQL ............ 90
来源：http://ye.newstarts.cn

Bash ........... 80
来源：http://kr.bookmarksfly.cn

Kotlin ......... 15
来源：http://lw.muxihuayi.cn

Swift .......... 15
来源：http://mq.huixinmuqiang.cn

Lua ............ 10
来源：http://rr.chemitech.net.cn

Perl ........... 10
来源：http://nb.shtwfgs.cn

Scala .......... 10
来源：http://fl.wgjwhj.cn

------------------------------------
来源：http://fv.shxzskj.cn

合计 ........... 2106 条
来源：http://me.bookmarksfly.cn

按章节统计：
来源：http://kx.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tf.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vw.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gy.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lq.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yp.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lu.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pc.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zv.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qu.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ts.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dt.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bh.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pe.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lq.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ck.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tz.nszjky.cn

Q SQL 专题                              90
来源：http://fz.gzmigu.cn

R Bash 专题                             80
来源：http://sm.huanxung.cn

S C / C++ 专题                          60
来源：http://sx.nszjky.cn

T 其他语言补充                          60
来源：http://ay.huanxung.cn

U 高频实用片段                         120
来源：http://uu.bjjhwx.cn

------------------------------------
来源：http://fl.lnxyls.cn

合计                                  2106 条
来源：http://na.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://df.haigaiapp.cn

使用提醒
来源：http://tc.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://sy.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qn.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zf.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uo.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qs.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gv.jianghongdianzi.cn

—— 文件结束 ——
来源：http://sp.hnjuh.cn

================================================================================
来源：http://qz.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://ss.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://wg.9csxet.cn

================================================================================
来源：http://kw.nicolike.cn

【收录内容】
来源：http://lv.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cy.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ed.szsharing.cn

SQL · Bash · C · C++
来源：http://cv.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rm.wgjwhj.cn

【使用说明】
来源：http://iz.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sg.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yu.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dj.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iw.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ke.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qt.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zj.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://on.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hg.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rf.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vh.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ua.huanxung.cn

【文件统计】
来源：http://lg.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://un.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://je.shxzskj.cn

目  录
来源：http://fp.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://tj.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qy.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ht.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fa.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://um.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bo.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ql.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ha.nicolike.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ra.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sp.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xw.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yg.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ht.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://do.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ux.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kr.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yp.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tf.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xy.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ce.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://po.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ji.nszjky.cn

================================================================================
来源：http://yv.szsharing.cn

A. 基础语法与类型
来源：http://cl.colortex.cn

================================================================================
来源：http://mj.yuntaijiaju.cn

[A01] Hello World
来源：http://ou.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://bc.asd995.cn

PHP:  echo "Hello, World!";
来源：http://ht.asd995.cn

JS:   console.log("Hello, World!");
来源：http://yg.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yl.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://up.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://nj.521024.cn

Ruby: puts "Hello, World!"
来源：http://ph.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dm.newstarts.cn

[A02] 变量声明与赋值
来源：http://yk.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wg.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ye.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zt.shxzskj.cn


<!-- 参考信息 -->