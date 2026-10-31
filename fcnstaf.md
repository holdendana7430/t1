代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://er.9csxet.cn

@contextlib.contextmanager
来源：http://ma.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://ra.newstarts.cn

list(zip(*m))
来源：http://op.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://qe.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mj.bjjhwx.cn

[U24] Py：路径操作
来源：http://hg.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://so.asd995.cn

[U25] Py：CSV 按字典读
来源：http://pz.9csxet.cn

csv.DictReader(f)
来源：http://pf.colortex.cn

[U26] Py：并发下载
来源：http://tg.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ni.colortex.cn

[U27] Py：异步 HTTP
来源：http://wi.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://ip.haigaiapp.cn

[U28] Py：类型别名
来源：http://ya.newstarts.cn

UserId = int
来源：http://ey.colortex.cn

[U29] Py：属性校验
来源：http://pv.gzmigu.cn

@property 与 @x.setter 配合
来源：http://ir.bjjhwx.cn

[U30] Py：数据类
来源：http://sz.haigaiapp.cn

@dataclass(slots=True)
来源：http://dh.hahajie.cn

[U31] Py：单测
来源：http://jj.hahajie.cn

python -m pytest -q
来源：http://jb.jctech888.com.cn

[U32] Py：代码格式化
来源：http://dk.colortex.cn

ruff format . && ruff check --fix .
来源：http://qx.haigaiapp.cn

[U33] Py：打包发布
来源：http://qp.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://yw.wgjwhj.cn

[U34] Py：判断编码
来源：http://me.szxytkj.cn

chardet.detect(raw)
来源：http://sj.asd995.cn

[U35] Py：发送邮件
来源：http://fe.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ku.nszjky.cn

[U36] Py：定时任务
来源：http://tv.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://ju.shxzskj.cn

[U37] Py：读写 Excel
来源：http://lw.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pi.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://tw.colortex.cn

Path(__file__).resolve().parent
来源：http://mf.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://na.panjiajie.cn

sys.stdout.isatty()
来源：http://lh.colortex.cn

[U40] Py：打印到标准错误
来源：http://gy.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://ln.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://zw.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ia.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://fx.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hc.huanxung.cn

[U43] PHP：声明命名空间
来源：http://tz.newstarts.cn

namespace App\Http;
来源：http://vr.nszjky.cn

[U44] PHP：开启严格类型
来源：http://oe.gzmigu.cn

declare(strict_types=1);
来源：http://ps.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://lf.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pv.huanxung.cn

[U46] PHP：可空类型
来源：http://sv.jctech888.com.cn

?string $name = null
来源：http://nn.szsharing.cn

[U47] PHP：联合类型
来源：http://qx.haigaiapp.cn

int|string $id
来源：http://um.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://vv.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dy.gzmigu.cn

[U49] PHP：只读属性
来源：http://xc.jctech888.com.cn

public readonly string $name
来源：http://yk.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://ou.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://zm.bjjhwx.cn

[U51] PHP：数组解构
来源：http://vv.szxytkj.cn

[$a, $b] = $arr;
来源：http://wi.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://fh.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://kl.hahajie.cn

[U53] PHP：空合并运算符
来源：http://ul.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://fw.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://ta.yuntaijiaju.cn

$obj?->method()
来源：http://rr.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://wr.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iw.yuexingan06.cn

[U56] PHP：命名参数
来源：http://pd.muxihuayi.cn

f(a: 1, b: 2)
来源：http://tc.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ii.gzmigu.cn

"值: {$a}"
来源：http://vx.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://ew.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lu.hnjuh.cn

[U59] PHP：自定义排序
来源：http://ku.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yl.colortex.cn

[U60] PHP：JSON 编解码
来源：http://fm.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oq.hnjuh.cn

[U61] PHP：正则
来源：http://hs.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kq.panjiajie.cn

[U62] PHP：日期对象
来源：http://bi.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lk.huixiangedu.cn

[U63] PHP：文件读写
来源：http://cr.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://st.9csxet.cn

[U64] PHP：目录遍历
来源：http://es.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://ya.szsharing.cn

[U65] PHP：会话
来源：http://ts.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nz.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://pb.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gz.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://gy.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jt.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://ge.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lw.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://yj.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ox.hahajie.cn

[U70] PHP：PDO 事务
来源：http://ro.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qw.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://kd.521024.cn

throw new RuntimeException("失败", 500);
来源：http://dp.nicolike.cn

[U72] PHP：写错误日志
来源：http://nh.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://nf.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://jf.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://jj.szsharing.cn

[U74] PHP：读取环境变量
来源：http://uh.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://au.nicolike.cn

[U75] PHP：依赖注入
来源：http://py.wgjwhj.cn

composer require psr/container
来源：http://tu.521024.cn

[U76] PHP：简单路由
来源：http://ho.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hf.nicolike.cn

[U77] PHP：模板渲染
来源：http://wl.shxzukj.cn

composer require twig/twig
来源：http://sg.gzmigu.cn

[U78] PHP：单元测试
来源：http://qh.521024.cn

composer require --dev phpunit/phpunit
来源：http://qa.shxzskj.cn

[U79] PHP：静态分析
来源：http://rm.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://nw.asd995.cn

[U80] PHP：代码规范修复
来源：http://nb.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eu.jctech888.com.cn

[U81] JS：初始化项目
来源：http://cx.chemitech.net.cn

npm init -y;  npm i express
来源：http://lh.521024.cn

[U82] JS：package.json 脚本
来源：http://ro.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nc.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://bh.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mk.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://tt.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nw.panjiajie.cn

[U85] JS：可选链
来源：http://ty.bookmarksfly.cn

a?.b?.c
来源：http://qy.9csxet.cn

[U86] JS：空值合并
来源：http://th.nicolike.cn

a ?? b
来源：http://vo.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://fr.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://vr.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://el.hnjuh.cn

{ ...a, ...b }
来源：http://fe.shxzskj.cn

[U89] JS：数组去重
来源：http://pn.szsharing.cn

[...new Set(arr)]
来源：http://wt.huanxung.cn

[U90] JS：数字数组排序
来源：http://ow.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://ua.hahajie.cn

[U91] JS：对象键值遍历
来源：http://wl.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gq.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://vc.lnxyls.cn

structuredClone(obj)
来源：http://wf.gzmigu.cn

[U93] JS：模板字符串
来源：http://ly.jctech888.com.cn

`共 ${n} 条`
来源：http://rq.newstarts.cn

[U94] JS：箭头函数
来源：http://hb.chemitech.net.cn

const double = x => x * 2;
来源：http://tx.9csxet.cn

[U95] JS：Promise 包装
来源：http://fp.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://uo.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://oq.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ei.shxzukj.cn

[U97] JS：并发请求
来源：http://ad.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://us.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://mn.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dg.panjiajie.cn

[U99] JS：事件监听
来源：http://xg.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://bo.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://mm.wgjwhj.cn

document.querySelector(".item")
来源：http://nk.shxzskj.cn

[U101] JS：classList 操作
来源：http://kg.asd995.cn

el.classList.toggle("active")
来源：http://zj.shxzukj.cn

[U102] JS：本地存储
来源：http://nm.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vb.colortex.cn

[U103] JS：定时器
来源：http://ro.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ls.gzmigu.cn

[U104] JS：防抖
来源：http://ez.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://td.hahajie.cn

[U105] JS：节流
来源：http://kb.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jj.szsharing.cn

[U106] JS：日期格式化
来源：http://cw.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hp.chemitech.net.cn

[U107] JS：数字千分位
来源：http://oa.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vv.haigaiapp.cn

[U108] JS：随机整数
来源：http://zw.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dm.hahajie.cn

[U109] JS：数组分组
来源：http://ss.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://dp.hnjuh.cn

[U110] JS：数组分块
来源：http://rp.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://su.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://rm.nszjky.cn

new Map(Object.entries(obj))
来源：http://qn.yuexingan06.cn

[U112] JS：字符串补位
来源：http://dd.521024.cn

"7".padStart(3, "0")
来源：http://ad.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://zi.hahajie.cn

s.replaceAll("a", "b")
来源：http://yk.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://zb.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iz.huanxung.cn

[U115] JS：生成 UUID
来源：http://fi.gzmigu.cn

crypto.randomUUID()
来源：http://hk.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://xg.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://oh.panjiajie.cn

[U117] JS：单元测试
来源：http://mu.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://aa.hnjuh.cn

[U118] JS：开发服务器
来源：http://av.9csxet.cn

npm i -D vite;  npx vite
来源：http://tz.bjjhwx.cn

[U119] JS：生产构建
来源：http://hg.yuexingan06.cn

npx vite build
来源：http://ap.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://jq.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://bt.bjjhwx.cn

================================================================================
来源：http://zg.hahajie.cn

统计汇总
来源：http://hr.szsharing.cn

================================================================================
来源：http://il.haigaiapp.cn

按语言统计（条）：
来源：http://zx.hahajie.cn

Python ......... 252
来源：http://ft.wgjwhj.cn

PHP ............ 252
来源：http://bl.yuexingan06.cn

JavaScript ..... 252
来源：http://cf.huixinmuqiang.cn

TypeScript ..... 212
来源：http://qd.521024.cn

Java ........... 212
来源：http://ng.yuexingan06.cn

Go ............. 212
来源：http://mn.colortex.cn

Ruby ........... 212
来源：http://co.asd995.cn

C# ............. 212
来源：http://gm.gzmigu.cn

C .............. 30
来源：http://du.muxihuayi.cn

C++ ............ 30
来源：http://rl.nicolike.cn

SQL ............ 90
来源：http://is.nicolike.cn

Bash ........... 80
来源：http://jw.shxzukj.cn

Kotlin ......... 15
来源：http://lh.chemitech.net.cn

Swift .......... 15
来源：http://rz.yuexingan06.cn

Lua ............ 10
来源：http://qx.colortex.cn

Perl ........... 10
来源：http://ib.haigaiapp.cn

Scala .......... 10
来源：http://rx.colortex.cn

------------------------------------
来源：http://yl.521024.cn

合计 ........... 2106 条
来源：http://to.gzmigu.cn

按章节统计：
来源：http://wt.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oz.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qy.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://od.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ua.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cm.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ox.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qk.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bi.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yz.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ai.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bq.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dj.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hb.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ww.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ul.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mp.shxzukj.cn

Q SQL 专题                              90
来源：http://ya.jctech888.com.cn

R Bash 专题                             80
来源：http://jk.hahajie.cn

S C / C++ 专题                          60
来源：http://wa.nszjky.cn

T 其他语言补充                          60
来源：http://rg.lnxyls.cn

U 高频实用片段                         120
来源：http://ej.chemitech.net.cn

------------------------------------
来源：http://rt.nszjky.cn

合计                                  2106 条
来源：http://la.newstarts.cn

--------------------------------------------------------------------------------
来源：http://cj.shtwfgs.cn

使用提醒
来源：http://ck.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://kf.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xz.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cy.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yv.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lm.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yw.yuexingan06.cn

—— 文件结束 ——
来源：http://uz.newstarts.cn

================================================================================
来源：http://fz.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://vl.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://rv.huixiangedu.cn

================================================================================
来源：http://uy.yuntaijiaju.cn

【收录内容】
来源：http://kl.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xx.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iq.szsharing.cn

SQL · Bash · C · C++
来源：http://he.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ys.chemitech.net.cn

【使用说明】
来源：http://ey.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ok.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ip.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://za.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iw.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fd.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rj.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yd.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uy.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ut.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://al.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ia.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cq.jctech888.com.cn

【文件统计】
来源：http://hg.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ge.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://hk.huixinmuqiang.cn

目  录
来源：http://mu.hahajie.cn

--------------------------------------------------------------------------------
来源：http://lb.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gj.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yw.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vm.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jv.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cp.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rj.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oc.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wf.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://va.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ve.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eh.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vq.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pv.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pl.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://om.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vo.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qe.wgjwhj.cn


<!-- 参考信息 -->