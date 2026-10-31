代发 wailian999

[U27] Py：异步 HTTP
来源：http://qs.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://vu.szxytkj.cn

[U28] Py：类型别名
来源：http://qe.shtwfgs.cn

UserId = int
来源：http://tv.nicolike.cn

[U29] Py：属性校验
来源：http://ye.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://bq.hahajie.cn

[U30] Py：数据类
来源：http://la.huixiangedu.cn

@dataclass(slots=True)
来源：http://yl.nszjky.cn

[U31] Py：单测
来源：http://po.9csxet.cn

python -m pytest -q
来源：http://su.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://bm.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://gb.szxytkj.cn

[U33] Py：打包发布
来源：http://jd.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://fe.haigaiapp.cn

[U34] Py：判断编码
来源：http://ge.yuexingan06.cn

chardet.detect(raw)
来源：http://mw.newstarts.cn

[U35] Py：发送邮件
来源：http://ij.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ou.wgjwhj.cn

[U36] Py：定时任务
来源：http://cm.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://eq.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://nu.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://de.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://sv.521024.cn

Path(__file__).resolve().parent
来源：http://yz.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://ju.9csxet.cn

sys.stdout.isatty()
来源：http://gt.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://nl.szsharing.cn

print("err", file=sys.stderr)
来源：http://af.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://gt.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://di.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://su.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aa.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://cz.huixiangedu.cn

namespace App\Http;
来源：http://ol.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://ik.gzmigu.cn

declare(strict_types=1);
来源：http://hv.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://om.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rw.chemitech.net.cn

[U46] PHP：可空类型
来源：http://ne.jctech888.com.cn

?string $name = null
来源：http://jw.asd995.cn

[U47] PHP：联合类型
来源：http://je.hahajie.cn

int|string $id
来源：http://by.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://jq.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ra.9csxet.cn

[U49] PHP：只读属性
来源：http://lz.bookmarksfly.cn

public readonly string $name
来源：http://de.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://sf.hahajie.cn

public function __construct(private int $id) {}
来源：http://co.huixiangedu.cn

[U51] PHP：数组解构
来源：http://tp.huixiangedu.cn

[$a, $b] = $arr;
来源：http://lm.hnjuh.cn

[U52] PHP：箭头函数
来源：http://jf.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://mb.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://nj.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://ke.gzmigu.cn

[U54] PHP：空安全调用
来源：http://bd.colortex.cn

$obj?->method()
来源：http://hi.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://eq.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cl.gzmigu.cn

[U56] PHP：命名参数
来源：http://md.muxihuayi.cn

f(a: 1, b: 2)
来源：http://fo.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://ae.521024.cn

"值: {$a}"
来源：http://ol.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://sp.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zh.asd995.cn

[U59] PHP：自定义排序
来源：http://yl.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ku.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://rg.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ex.shxzukj.cn

[U61] PHP：正则
来源：http://ju.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tc.hahajie.cn

[U62] PHP：日期对象
来源：http://sn.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ko.bjjhwx.cn

[U63] PHP：文件读写
来源：http://uj.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jk.panjiajie.cn

[U64] PHP：目录遍历
来源：http://ba.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://ni.chemitech.net.cn

[U65] PHP：会话
来源：http://lr.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pe.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://by.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bu.9csxet.cn

[U67] PHP：处理文件上传
来源：http://rg.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wy.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://pa.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gb.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://iy.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://au.szsharing.cn

[U70] PHP：PDO 事务
来源：http://cx.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tx.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://gf.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://jz.9csxet.cn

[U72] PHP：写错误日志
来源：http://rc.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://hw.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://by.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://az.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://um.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://yg.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://hl.haigaiapp.cn

composer require psr/container
来源：http://ct.wgjwhj.cn

[U76] PHP：简单路由
来源：http://yx.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mt.nicolike.cn

[U77] PHP：模板渲染
来源：http://zd.wgjwhj.cn

composer require twig/twig
来源：http://pv.hahajie.cn

[U78] PHP：单元测试
来源：http://ji.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://wd.shxzukj.cn

[U79] PHP：静态分析
来源：http://af.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://ax.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://xz.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hq.hahajie.cn

[U81] JS：初始化项目
来源：http://ep.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://kp.szsharing.cn

[U82] JS：package.json 脚本
来源：http://qj.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yr.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://mw.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dp.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://ju.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xf.colortex.cn

[U85] JS：可选链
来源：http://fy.bjjhwx.cn

a?.b?.c
来源：http://yo.9csxet.cn

[U86] JS：空值合并
来源：http://lz.lnxyls.cn

a ?? b
来源：http://lg.chemitech.net.cn

[U87] JS：解构默认值
来源：http://nr.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://ux.asd995.cn

[U88] JS：对象展开合并
来源：http://xq.huixinmuqiang.cn

{ ...a, ...b }
来源：http://jj.shxzukj.cn

[U89] JS：数组去重
来源：http://dk.chemitech.net.cn

[...new Set(arr)]
来源：http://ql.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ao.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://ui.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://ca.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qo.gzmigu.cn

[U92] JS：深拷贝
来源：http://bk.shxzskj.cn

structuredClone(obj)
来源：http://wq.nszjky.cn

[U93] JS：模板字符串
来源：http://if.shxzskj.cn

`共 ${n} 条`
来源：http://pq.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://mx.haigaiapp.cn

const double = x => x * 2;
来源：http://et.hahajie.cn

[U95] JS：Promise 包装
来源：http://dm.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://lk.szsharing.cn

[U96] JS：async/await 与异常
来源：http://vk.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xy.shxzukj.cn

[U97] JS：并发请求
来源：http://od.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kh.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://hd.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zf.huanxung.cn

[U99] JS：事件监听
来源：http://vf.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://sq.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://jt.newstarts.cn

document.querySelector(".item")
来源：http://ao.shxzukj.cn

[U101] JS：classList 操作
来源：http://jo.9csxet.cn

el.classList.toggle("active")
来源：http://lc.szxytkj.cn

[U102] JS：本地存储
来源：http://br.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ew.haigaiapp.cn

[U103] JS：定时器
来源：http://cx.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oe.jctech888.com.cn

[U104] JS：防抖
来源：http://um.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eg.shxzskj.cn

[U105] JS：节流
来源：http://qc.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hv.bjjhwx.cn

[U106] JS：日期格式化
来源：http://rq.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nh.shxzukj.cn

[U107] JS：数字千分位
来源：http://ye.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bw.shtwfgs.cn

[U108] JS：随机整数
来源：http://df.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pl.panjiajie.cn

[U109] JS：数组分组
来源：http://bb.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://nc.shtwfgs.cn

[U110] JS：数组分块
来源：http://gm.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bs.szxytkj.cn

[U111] JS：对象转 Map
来源：http://ru.szxytkj.cn

new Map(Object.entries(obj))
来源：http://tn.shtwfgs.cn

[U112] JS：字符串补位
来源：http://mu.shtwfgs.cn

"7".padStart(3, "0")
来源：http://gk.hahajie.cn

[U113] JS：正则替换全部
来源：http://oz.huanxung.cn

s.replaceAll("a", "b")
来源：http://hf.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://bm.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fz.panjiajie.cn

[U115] JS：生成 UUID
来源：http://wz.9csxet.cn

crypto.randomUUID()
来源：http://qp.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://lo.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://yo.shtwfgs.cn

[U117] JS：单元测试
来源：http://jk.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://xs.wgjwhj.cn

[U118] JS：开发服务器
来源：http://wy.hahajie.cn

npm i -D vite;  npx vite
来源：http://jz.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://qg.asd995.cn

npx vite build
来源：http://uo.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://cb.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://ip.asd995.cn

================================================================================
来源：http://gi.haigaiapp.cn

统计汇总
来源：http://pw.newstarts.cn

================================================================================
来源：http://xe.hahajie.cn

按语言统计（条）：
来源：http://sv.asd995.cn

Python ......... 252
来源：http://nz.shtwfgs.cn

PHP ............ 252
来源：http://ut.shxzukj.cn

JavaScript ..... 252
来源：http://qd.muxihuayi.cn

TypeScript ..... 212
来源：http://lc.yuexingan06.cn

Java ........... 212
来源：http://ri.panjiajie.cn

Go ............. 212
来源：http://ga.yuexingan06.cn

Ruby ........... 212
来源：http://bo.shxzskj.cn

C# ............. 212
来源：http://rt.nicolike.cn

C .............. 30
来源：http://jc.yuntaijiaju.cn

C++ ............ 30
来源：http://gs.shxzukj.cn

SQL ............ 90
来源：http://om.huixiangedu.cn

Bash ........... 80
来源：http://nc.panjiajie.cn

Kotlin ......... 15
来源：http://dr.shxzukj.cn

Swift .......... 15
来源：http://zg.hahajie.cn

Lua ............ 10
来源：http://bb.nicolike.cn

Perl ........... 10
来源：http://kr.hahajie.cn

Scala .......... 10
来源：http://uk.bookmarksfly.cn

------------------------------------
来源：http://ek.9csxet.cn

合计 ........... 2106 条
来源：http://iw.szxytkj.cn

按章节统计：
来源：http://ul.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bm.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oa.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://je.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mh.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kt.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bg.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vj.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mn.shtwfgs.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qu.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lv.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gp.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://az.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yl.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://it.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wk.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ny.huanxung.cn

Q SQL 专题                              90
来源：http://nu.yuexingan06.cn

R Bash 专题                             80
来源：http://ko.shxzskj.cn

S C / C++ 专题                          60
来源：http://bp.huanxung.cn

T 其他语言补充                          60
来源：http://uy.colortex.cn

U 高频实用片段                         120
来源：http://xr.newstarts.cn

------------------------------------
来源：http://nz.asd995.cn

合计                                  2106 条
来源：http://fa.colortex.cn

--------------------------------------------------------------------------------
来源：http://bs.haigaiapp.cn

使用提醒
来源：http://bi.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://lt.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xq.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rj.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bn.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wn.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oi.hahajie.cn

—— 文件结束 ——
来源：http://kp.wgjwhj.cn

================================================================================
来源：http://vs.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://ze.newstarts.cn

Common Programming Examples Cheat Book
来源：http://kj.gzmigu.cn

================================================================================
来源：http://gu.panjiajie.cn

【收录内容】
来源：http://rl.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lq.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zd.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://dj.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eu.huanxung.cn

【使用说明】
来源：http://zr.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jg.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ki.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gm.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ao.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cv.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xo.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jk.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://od.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tf.gzmigu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ba.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gg.yuntaijiaju.cn

【文件统计】
来源：http://lk.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yh.nicolike.cn

--------------------------------------------------------------------------------
来源：http://mm.gzmigu.cn

目  录
来源：http://mf.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://hq.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lp.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bd.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kr.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://om.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fc.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fb.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kl.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xh.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mq.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://su.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zz.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bi.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hu.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yd.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kd.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fb.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cz.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yd.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nx.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rk.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kj.hahajie.cn

================================================================================
来源：http://zy.bjjhwx.cn

A. 基础语法与类型
来源：http://ps.jianghongdianzi.cn

================================================================================
来源：http://uv.colortex.cn

[A01] Hello World
来源：http://xa.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://cd.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://vt.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://lx.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fz.wgjwhj.cn


<!-- 参考信息 -->