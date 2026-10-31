代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://be.bookmarksfly.cn

@contextlib.contextmanager
来源：http://zj.hahajie.cn

[U22] Py：矩阵转置
来源：http://lq.gzmigu.cn

list(zip(*m))
来源：http://kq.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://ig.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vx.jctech888.com.cn

[U24] Py：路径操作
来源：http://uf.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vy.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://qx.jianghongdianzi.cn

csv.DictReader(f)
来源：http://pj.9csxet.cn

[U26] Py：并发下载
来源：http://wc.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rq.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://fl.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://uu.yuexingan06.cn

[U28] Py：类型别名
来源：http://ex.huixinmuqiang.cn

UserId = int
来源：http://uj.yuexingan06.cn

[U29] Py：属性校验
来源：http://tk.gzmigu.cn

@property 与 @x.setter 配合
来源：http://ce.nicolike.cn

[U30] Py：数据类
来源：http://jc.wgjwhj.cn

@dataclass(slots=True)
来源：http://ue.hnjuh.cn

[U31] Py：单测
来源：http://bz.shtwfgs.cn

python -m pytest -q
来源：http://vw.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://qt.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://zg.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://kc.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ho.hnjuh.cn

[U34] Py：判断编码
来源：http://iy.nszjky.cn

chardet.detect(raw)
来源：http://hs.9csxet.cn

[U35] Py：发送邮件
来源：http://ps.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ij.asd995.cn

[U36] Py：定时任务
来源：http://qh.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://by.hnjuh.cn

[U37] Py：读写 Excel
来源：http://fd.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gv.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://jv.colortex.cn

Path(__file__).resolve().parent
来源：http://bg.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://bj.yuexingan06.cn

sys.stdout.isatty()
来源：http://nt.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://zr.szsharing.cn

print("err", file=sys.stderr)
来源：http://od.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://va.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rg.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://xq.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xf.colortex.cn

[U43] PHP：声明命名空间
来源：http://wg.szsharing.cn

namespace App\Http;
来源：http://gf.huanxung.cn

[U44] PHP：开启严格类型
来源：http://jp.huixinmuqiang.cn

declare(strict_types=1);
来源：http://bw.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://fx.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mu.shxzukj.cn

[U46] PHP：可空类型
来源：http://ov.wgjwhj.cn

?string $name = null
来源：http://bx.nszjky.cn

[U47] PHP：联合类型
来源：http://hm.huixiangedu.cn

int|string $id
来源：http://zf.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://kv.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fx.muxihuayi.cn

[U49] PHP：只读属性
来源：http://hw.bookmarksfly.cn

public readonly string $name
来源：http://pr.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://hu.shxzskj.cn

public function __construct(private int $id) {}
来源：http://ji.szsharing.cn

[U51] PHP：数组解构
来源：http://jo.chemitech.net.cn

[$a, $b] = $arr;
来源：http://zc.nicolike.cn

[U52] PHP：箭头函数
来源：http://jp.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://bu.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://ht.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://wy.asd995.cn

[U54] PHP：空安全调用
来源：http://na.shtwfgs.cn

$obj?->method()
来源：http://wg.9csxet.cn

[U55] PHP：match 表达式
来源：http://ri.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gn.hahajie.cn

[U56] PHP：命名参数
来源：http://ez.bjjhwx.cn

f(a: 1, b: 2)
来源：http://jv.panjiajie.cn

[U57] PHP：字符串插值
来源：http://pk.jctech888.com.cn

"值: {$a}"
来源：http://el.szxytkj.cn

[U58] PHP：数组三件套
来源：http://mq.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pm.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://rg.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ny.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://su.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xk.huixiangedu.cn

[U61] PHP：正则
来源：http://yd.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vl.hnjuh.cn

[U62] PHP：日期对象
来源：http://ns.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ku.521024.cn

[U63] PHP：文件读写
来源：http://cc.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://be.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://jy.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://rj.521024.cn

[U65] PHP：会话
来源：http://ht.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://na.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://ct.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tg.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://zi.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mp.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://bd.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ka.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://et.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jo.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://fm.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yo.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://sx.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://ug.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://fy.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://ao.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://qp.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://fv.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://ax.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://dj.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://lk.nszjky.cn

composer require psr/container
来源：http://qc.muxihuayi.cn

[U76] PHP：简单路由
来源：http://wh.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pr.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://ud.huanxung.cn

composer require twig/twig
来源：http://hs.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://rt.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://zk.shxzskj.cn

[U79] PHP：静态分析
来源：http://ao.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://yp.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://ic.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nz.colortex.cn

[U81] JS：初始化项目
来源：http://vv.shxzukj.cn

npm init -y;  npm i express
来源：http://hm.nicolike.cn

[U82] JS：package.json 脚本
来源：http://zv.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rn.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://vg.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nj.521024.cn

[U84] JS：CommonJS 写法
来源：http://fl.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pv.bjjhwx.cn

[U85] JS：可选链
来源：http://qp.shtwfgs.cn

a?.b?.c
来源：http://wu.shxzukj.cn

[U86] JS：空值合并
来源：http://jv.521024.cn

a ?? b
来源：http://zd.9csxet.cn

[U87] JS：解构默认值
来源：http://an.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://lg.newstarts.cn

[U88] JS：对象展开合并
来源：http://js.shxzukj.cn

{ ...a, ...b }
来源：http://us.jctech888.com.cn

[U89] JS：数组去重
来源：http://eq.gzmigu.cn

[...new Set(arr)]
来源：http://cp.9csxet.cn

[U90] JS：数字数组排序
来源：http://sx.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://dr.9csxet.cn

[U91] JS：对象键值遍历
来源：http://qt.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ad.huanxung.cn

[U92] JS：深拷贝
来源：http://mr.colortex.cn

structuredClone(obj)
来源：http://gt.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://aj.521024.cn

`共 ${n} 条`
来源：http://bq.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://cq.521024.cn

const double = x => x * 2;
来源：http://vg.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://fw.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://ku.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://pe.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rt.huanxung.cn

[U97] JS：并发请求
来源：http://zy.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fw.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://xa.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ub.shxzskj.cn

[U99] JS：事件监听
来源：http://rs.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://tl.huanxung.cn

[U100] JS：DOM 查询
来源：http://tq.9csxet.cn

document.querySelector(".item")
来源：http://cw.gzmigu.cn

[U101] JS：classList 操作
来源：http://ty.nszjky.cn

el.classList.toggle("active")
来源：http://ws.gzmigu.cn

[U102] JS：本地存储
来源：http://rv.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ul.shxzukj.cn

[U103] JS：定时器
来源：http://rw.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dt.yuexingan06.cn

[U104] JS：防抖
来源：http://cq.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eq.jianghongdianzi.cn

[U105] JS：节流
来源：http://ye.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://da.521024.cn

[U106] JS：日期格式化
来源：http://tc.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ud.wgjwhj.cn

[U107] JS：数字千分位
来源：http://mt.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oi.lnxyls.cn

[U108] JS：随机整数
来源：http://ao.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fa.bjjhwx.cn

[U109] JS：数组分组
来源：http://ps.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://fd.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://xl.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uz.newstarts.cn

[U111] JS：对象转 Map
来源：http://lz.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://zh.szxytkj.cn

[U112] JS：字符串补位
来源：http://jh.521024.cn

"7".padStart(3, "0")
来源：http://qk.9csxet.cn

[U113] JS：正则替换全部
来源：http://zl.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://aj.521024.cn

[U114] JS：JSON 深比较
来源：http://fw.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vj.szsharing.cn

[U115] JS：生成 UUID
来源：http://uf.shxzskj.cn

crypto.randomUUID()
来源：http://lk.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://bi.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://em.chemitech.net.cn

[U117] JS：单元测试
来源：http://sw.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://cw.shxzskj.cn

[U118] JS：开发服务器
来源：http://we.newstarts.cn

npm i -D vite;  npx vite
来源：http://rc.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://le.hnjuh.cn

npx vite build
来源：http://va.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://yy.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://tk.hahajie.cn

================================================================================
来源：http://ms.shxzskj.cn

统计汇总
来源：http://wt.hnjuh.cn

================================================================================
来源：http://io.huixiangedu.cn

按语言统计（条）：
来源：http://tr.bookmarksfly.cn

Python ......... 252
来源：http://hj.jianghongdianzi.cn

PHP ............ 252
来源：http://eb.gzmigu.cn

JavaScript ..... 252
来源：http://fu.muxihuayi.cn

TypeScript ..... 212
来源：http://vx.nicolike.cn

Java ........... 212
来源：http://mb.gzmigu.cn

Go ............. 212
来源：http://nv.jianghongdianzi.cn

Ruby ........... 212
来源：http://sa.shtwfgs.cn

C# ............. 212
来源：http://nj.haigaiapp.cn

C .............. 30
来源：http://iw.gzmigu.cn

C++ ............ 30
来源：http://ei.szsharing.cn

SQL ............ 90
来源：http://ub.shxzskj.cn

Bash ........... 80
来源：http://hi.9csxet.cn

Kotlin ......... 15
来源：http://az.wgjwhj.cn

Swift .......... 15
来源：http://bf.asd995.cn

Lua ............ 10
来源：http://cv.nicolike.cn

Perl ........... 10
来源：http://rc.jianghongdianzi.cn

Scala .......... 10
来源：http://xw.jctech888.com.cn

------------------------------------
来源：http://bw.hnjuh.cn

合计 ........... 2106 条
来源：http://jn.huanxung.cn

按章节统计：
来源：http://xa.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tw.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jc.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ve.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ah.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dr.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sk.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hs.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fb.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ae.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xv.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mk.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mj.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oz.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dy.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xr.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ri.haigaiapp.cn

Q SQL 专题                              90
来源：http://rk.lnxyls.cn

R Bash 专题                             80
来源：http://af.shtwfgs.cn

S C / C++ 专题                          60
来源：http://ng.asd995.cn

T 其他语言补充                          60
来源：http://my.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://uv.chemitech.net.cn

------------------------------------
来源：http://ju.nszjky.cn

合计                                  2106 条
来源：http://rl.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://er.panjiajie.cn

使用提醒
来源：http://tm.huanxung.cn

--------------------------------------------------------------------------------
来源：http://nx.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wo.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bl.shxzskj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vw.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pe.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ru.shxzskj.cn

—— 文件结束 ——
来源：http://ve.newstarts.cn

================================================================================
来源：http://ia.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://xw.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://qm.hahajie.cn

================================================================================
来源：http://eh.nszjky.cn

【收录内容】
来源：http://fl.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://db.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rg.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://xi.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eg.asd995.cn

【使用说明】
来源：http://cc.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uu.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lu.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://la.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ul.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ho.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uo.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vv.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sz.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rd.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://om.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://co.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xm.shxzukj.cn

【文件统计】
来源：http://ws.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tf.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://xi.shtwfgs.cn

目  录
来源：http://ig.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://fc.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://za.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xx.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ga.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pc.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nm.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rh.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sq.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pt.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dw.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aa.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dr.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ug.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xd.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://to.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nz.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vf.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://at.9csxet.cn


<!-- 参考信息 -->