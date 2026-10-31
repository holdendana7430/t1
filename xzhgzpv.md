代发 wailian999

[U25] Py：CSV 按字典读
来源：http://bk.yuexingan06.cn

csv.DictReader(f)
来源：http://pj.hnjuh.cn

[U26] Py：并发下载
来源：http://uy.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mq.hahajie.cn

[U27] Py：异步 HTTP
来源：http://le.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://ry.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://em.asd995.cn

UserId = int
来源：http://vn.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://vf.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://pi.yuexingan06.cn

[U30] Py：数据类
来源：http://hp.szsharing.cn

@dataclass(slots=True)
来源：http://kd.hahajie.cn

[U31] Py：单测
来源：http://ht.hahajie.cn

python -m pytest -q
来源：http://tn.jctech888.com.cn

[U32] Py：代码格式化
来源：http://wu.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://ty.9csxet.cn

[U33] Py：打包发布
来源：http://ja.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://st.shtwfgs.cn

[U34] Py：判断编码
来源：http://lr.huanxung.cn

chardet.detect(raw)
来源：http://ug.huanxung.cn

[U35] Py：发送邮件
来源：http://ts.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yh.newstarts.cn

[U36] Py：定时任务
来源：http://hk.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://xn.huanxung.cn

[U37] Py：读写 Excel
来源：http://rx.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://td.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://hr.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://ko.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://dr.yuexingan06.cn

sys.stdout.isatty()
来源：http://of.huanxung.cn

[U40] Py：打印到标准错误
来源：http://sy.shxzskj.cn

print("err", file=sys.stderr)
来源：http://pv.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://ij.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yd.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://jk.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pk.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://aq.shxzskj.cn

namespace App\Http;
来源：http://go.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://ur.9csxet.cn

declare(strict_types=1);
来源：http://ae.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://lf.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://un.bjjhwx.cn

[U46] PHP：可空类型
来源：http://vi.9csxet.cn

?string $name = null
来源：http://pk.gzmigu.cn

[U47] PHP：联合类型
来源：http://vk.nicolike.cn

int|string $id
来源：http://kk.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://bo.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nd.shxzukj.cn

[U49] PHP：只读属性
来源：http://no.huanxung.cn

public readonly string $name
来源：http://aj.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://zn.asd995.cn

public function __construct(private int $id) {}
来源：http://co.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://ui.lnxyls.cn

[$a, $b] = $arr;
来源：http://pw.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://ub.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://pn.nszjky.cn

[U53] PHP：空合并运算符
来源：http://bs.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://qs.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://ln.muxihuayi.cn

$obj?->method()
来源：http://hk.szsharing.cn

[U55] PHP：match 表达式
来源：http://pk.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hd.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://vu.colortex.cn

f(a: 1, b: 2)
来源：http://id.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://qz.newstarts.cn

"值: {$a}"
来源：http://qg.newstarts.cn

[U58] PHP：数组三件套
来源：http://ta.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gv.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://xi.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://og.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://dd.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://km.huixinmuqiang.cn

[U61] PHP：正则
来源：http://rb.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xx.shtwfgs.cn

[U62] PHP：日期对象
来源：http://fz.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://di.szxytkj.cn

[U63] PHP：文件读写
来源：http://ro.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zb.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://ep.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ij.bjjhwx.cn

[U65] PHP：会话
来源：http://fk.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ui.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://jq.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fi.nszjky.cn

[U67] PHP：处理文件上传
来源：http://ad.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ys.huanxung.cn

[U68] PHP：PDO 连接
来源：http://zi.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://if.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://hv.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ju.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://nz.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wp.nszjky.cn

[U71] PHP：抛出异常
来源：http://ql.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://ea.nicolike.cn

[U72] PHP：写错误日志
来源：http://xu.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://lu.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://mn.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://zq.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://mo.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://wo.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://id.chemitech.net.cn

composer require psr/container
来源：http://xe.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://ib.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xi.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://rq.chemitech.net.cn

composer require twig/twig
来源：http://iw.newstarts.cn

[U78] PHP：单元测试
来源：http://yp.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://tc.521024.cn

[U79] PHP：静态分析
来源：http://qp.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://es.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://zb.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ty.gzmigu.cn

[U81] JS：初始化项目
来源：http://zy.asd995.cn

npm init -y;  npm i express
来源：http://qk.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://lg.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://in.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://mi.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xz.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://lu.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://my.shtwfgs.cn

[U85] JS：可选链
来源：http://zi.panjiajie.cn

a?.b?.c
来源：http://br.huanxung.cn

[U86] JS：空值合并
来源：http://ch.bjjhwx.cn

a ?? b
来源：http://pa.szxytkj.cn

[U87] JS：解构默认值
来源：http://ai.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://ex.szxytkj.cn

[U88] JS：对象展开合并
来源：http://zd.nicolike.cn

{ ...a, ...b }
来源：http://zw.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://jx.bookmarksfly.cn

[...new Set(arr)]
来源：http://pl.gzmigu.cn

[U90] JS：数字数组排序
来源：http://lc.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://yp.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://my.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zx.shtwfgs.cn

[U92] JS：深拷贝
来源：http://ie.bjjhwx.cn

structuredClone(obj)
来源：http://hy.newstarts.cn

[U93] JS：模板字符串
来源：http://dv.shxzskj.cn

`共 ${n} 条`
来源：http://cz.9csxet.cn

[U94] JS：箭头函数
来源：http://xl.shxzskj.cn

const double = x => x * 2;
来源：http://fn.gzmigu.cn

[U95] JS：Promise 包装
来源：http://ta.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://ky.colortex.cn

[U96] JS：async/await 与异常
来源：http://yh.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gq.521024.cn

[U97] JS：并发请求
来源：http://fq.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rj.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://vj.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://su.hahajie.cn

[U99] JS：事件监听
来源：http://dk.hahajie.cn

el.addEventListener("click", e => {})
来源：http://vg.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://ny.colortex.cn

document.querySelector(".item")
来源：http://wm.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://xp.lnxyls.cn

el.classList.toggle("active")
来源：http://oj.jctech888.com.cn

[U102] JS：本地存储
来源：http://qt.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://st.yuexingan06.cn

[U103] JS：定时器
来源：http://mc.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ol.gzmigu.cn

[U104] JS：防抖
来源：http://xr.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rb.wgjwhj.cn

[U105] JS：节流
来源：http://is.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fz.nszjky.cn

[U106] JS：日期格式化
来源：http://no.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://il.colortex.cn

[U107] JS：数字千分位
来源：http://mg.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://se.wgjwhj.cn

[U108] JS：随机整数
来源：http://bd.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fq.bookmarksfly.cn

[U109] JS：数组分组
来源：http://yl.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://da.lnxyls.cn

[U110] JS：数组分块
来源：http://ft.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ks.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://aq.gzmigu.cn

new Map(Object.entries(obj))
来源：http://eq.asd995.cn

[U112] JS：字符串补位
来源：http://av.jctech888.com.cn

"7".padStart(3, "0")
来源：http://km.shxzukj.cn

[U113] JS：正则替换全部
来源：http://xg.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://tg.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://fi.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mf.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://rn.haigaiapp.cn

crypto.randomUUID()
来源：http://jw.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://oq.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://ad.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://yv.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://nm.huanxung.cn

[U118] JS：开发服务器
来源：http://ae.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://ef.muxihuayi.cn

[U119] JS：生产构建
来源：http://fp.wgjwhj.cn

npx vite build
来源：http://sh.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://jg.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://nk.jianghongdianzi.cn

================================================================================
来源：http://ht.asd995.cn

统计汇总
来源：http://re.haigaiapp.cn

================================================================================
来源：http://sg.colortex.cn

按语言统计（条）：
来源：http://ze.szsharing.cn

Python ......... 252
来源：http://nl.newstarts.cn

PHP ............ 252
来源：http://rx.jianghongdianzi.cn

JavaScript ..... 252
来源：http://ok.lnxyls.cn

TypeScript ..... 212
来源：http://vs.bookmarksfly.cn

Java ........... 212
来源：http://dm.haigaiapp.cn

Go ............. 212
来源：http://gd.yuexingan06.cn

Ruby ........... 212
来源：http://rw.bjjhwx.cn

C# ............. 212
来源：http://jl.jctech888.com.cn

C .............. 30
来源：http://vc.szsharing.cn

C++ ............ 30
来源：http://ez.gzmigu.cn

SQL ............ 90
来源：http://ec.jctech888.com.cn

Bash ........... 80
来源：http://rd.muxihuayi.cn

Kotlin ......... 15
来源：http://ke.nszjky.cn

Swift .......... 15
来源：http://ms.lnxyls.cn

Lua ............ 10
来源：http://dw.haigaiapp.cn

Perl ........... 10
来源：http://rl.huixinmuqiang.cn

Scala .......... 10
来源：http://yu.newstarts.cn

------------------------------------
来源：http://ig.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://it.panjiajie.cn

按章节统计：
来源：http://gf.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ho.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dx.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dj.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nb.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jv.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bi.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ms.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bl.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ob.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qh.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ef.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tn.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ox.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xc.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nv.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kl.521024.cn

Q SQL 专题                              90
来源：http://xw.wgjwhj.cn

R Bash 专题                             80
来源：http://rt.shxzskj.cn

S C / C++ 专题                          60
来源：http://to.asd995.cn

T 其他语言补充                          60
来源：http://dv.hahajie.cn

U 高频实用片段                         120
来源：http://ak.haigaiapp.cn

------------------------------------
来源：http://mv.huixiangedu.cn

合计                                  2106 条
来源：http://wy.huanxung.cn

--------------------------------------------------------------------------------
来源：http://th.gzmigu.cn

使用提醒
来源：http://nx.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ja.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://du.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uv.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lo.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gw.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bi.9csxet.cn

—— 文件结束 ——
来源：http://ol.shxzukj.cn

================================================================================
来源：http://ed.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://tu.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://yp.panjiajie.cn

================================================================================
来源：http://re.panjiajie.cn

【收录内容】
来源：http://hz.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qm.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nl.szsharing.cn

SQL · Bash · C · C++
来源：http://at.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ln.chemitech.net.cn

【使用说明】
来源：http://so.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dz.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gw.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nj.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ol.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ma.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mw.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sq.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ro.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sr.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ly.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://md.nszjky.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dk.nicolike.cn

【文件统计】
来源：http://pz.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pa.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://he.9csxet.cn

目  录
来源：http://bq.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://mq.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oj.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mr.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vq.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wu.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ef.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://av.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gb.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ff.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bj.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ym.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gg.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ra.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mj.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bv.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://om.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ql.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ym.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bv.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rw.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bw.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hw.huixinmuqiang.cn

================================================================================
来源：http://dm.colortex.cn

A. 基础语法与类型
来源：http://yv.yuexingan06.cn

================================================================================
来源：http://sv.huixiangedu.cn

[A01] Hello World
来源：http://ow.gzmigu.cn


<!-- 参考信息 -->