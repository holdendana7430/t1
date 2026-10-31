代发 wailian999

[U17] Py：初始化日志
来源：http://qo.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://br.szxytkj.cn

[U18] Py：预编译正则
来源：http://eb.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://ys.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://vc.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hj.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://tf.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://lr.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://oz.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://lu.panjiajie.cn

[U22] Py：矩阵转置
来源：http://pz.chemitech.net.cn

list(zip(*m))
来源：http://yp.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://es.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://io.asd995.cn

[U24] Py：路径操作
来源：http://nv.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dv.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://hf.shxzukj.cn

csv.DictReader(f)
来源：http://kb.hahajie.cn

[U26] Py：并发下载
来源：http://od.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zo.nicolike.cn

[U27] Py：异步 HTTP
来源：http://gs.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://qf.shxzskj.cn

[U28] Py：类型别名
来源：http://ze.haigaiapp.cn

UserId = int
来源：http://jf.asd995.cn

[U29] Py：属性校验
来源：http://qm.panjiajie.cn

@property 与 @x.setter 配合
来源：http://rb.bjjhwx.cn

[U30] Py：数据类
来源：http://ew.gzmigu.cn

@dataclass(slots=True)
来源：http://qt.bookmarksfly.cn

[U31] Py：单测
来源：http://cl.shxzukj.cn

python -m pytest -q
来源：http://kg.nicolike.cn

[U32] Py：代码格式化
来源：http://cy.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://vg.haigaiapp.cn

[U33] Py：打包发布
来源：http://zo.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://ie.hnjuh.cn

[U34] Py：判断编码
来源：http://uq.shxzskj.cn

chardet.detect(raw)
来源：http://nw.newstarts.cn

[U35] Py：发送邮件
来源：http://dk.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xu.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://gu.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://ny.szsharing.cn

[U37] Py：读写 Excel
来源：http://ni.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mo.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://po.huanxung.cn

Path(__file__).resolve().parent
来源：http://yd.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://vi.bookmarksfly.cn

sys.stdout.isatty()
来源：http://fl.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://bj.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://ux.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://ef.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ra.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://lg.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lv.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://lv.shxzukj.cn

namespace App\Http;
来源：http://bd.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://ef.hahajie.cn

declare(strict_types=1);
来源：http://zo.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://va.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qi.shtwfgs.cn

[U46] PHP：可空类型
来源：http://kp.wgjwhj.cn

?string $name = null
来源：http://jt.9csxet.cn

[U47] PHP：联合类型
来源：http://ct.huixiangedu.cn

int|string $id
来源：http://ay.shxzskj.cn

[U48] PHP：纯枚举
来源：http://bb.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pf.chemitech.net.cn

[U49] PHP：只读属性
来源：http://wj.hnjuh.cn

public readonly string $name
来源：http://jv.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://fe.newstarts.cn

public function __construct(private int $id) {}
来源：http://mq.colortex.cn

[U51] PHP：数组解构
来源：http://ar.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://wg.9csxet.cn

[U52] PHP：箭头函数
来源：http://og.521024.cn

$double = fn($x) => $x * 2;
来源：http://ac.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://um.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://wo.newstarts.cn

[U54] PHP：空安全调用
来源：http://ld.bjjhwx.cn

$obj?->method()
来源：http://al.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://wf.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ph.colortex.cn

[U56] PHP：命名参数
来源：http://sq.bjjhwx.cn

f(a: 1, b: 2)
来源：http://zh.newstarts.cn

[U57] PHP：字符串插值
来源：http://ms.nicolike.cn

"值: {$a}"
来源：http://hv.hnjuh.cn

[U58] PHP：数组三件套
来源：http://tj.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ho.shxzukj.cn

[U59] PHP：自定义排序
来源：http://tc.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mf.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://mr.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ka.nicolike.cn

[U61] PHP：正则
来源：http://qu.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rc.bjjhwx.cn

[U62] PHP：日期对象
来源：http://nk.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pz.9csxet.cn

[U63] PHP：文件读写
来源：http://jx.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yn.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://gq.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://sj.jctech888.com.cn

[U65] PHP：会话
来源：http://uf.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mw.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://cd.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mo.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://yy.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ao.nszjky.cn

[U68] PHP：PDO 连接
来源：http://gf.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cr.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://ax.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yk.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://zu.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ve.521024.cn

[U71] PHP：抛出异常
来源：http://jg.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://wo.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://tz.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://lv.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://kt.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://sg.asd995.cn

[U74] PHP：读取环境变量
来源：http://ts.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://ur.shxzskj.cn

[U75] PHP：依赖注入
来源：http://jg.jianghongdianzi.cn

composer require psr/container
来源：http://se.wgjwhj.cn

[U76] PHP：简单路由
来源：http://oh.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kp.hnjuh.cn

[U77] PHP：模板渲染
来源：http://zm.9csxet.cn

composer require twig/twig
来源：http://mp.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://bo.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://rd.panjiajie.cn

[U79] PHP：静态分析
来源：http://gz.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://sy.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://dl.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.asd995.cn

[U81] JS：初始化项目
来源：http://eb.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://pw.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://zi.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jp.521024.cn

[U83] JS：ES Module 导入导出
来源：http://lc.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ad.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://tp.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wc.jianghongdianzi.cn

[U85] JS：可选链
来源：http://dz.shtwfgs.cn

a?.b?.c
来源：http://kv.lnxyls.cn

[U86] JS：空值合并
来源：http://rb.szsharing.cn

a ?? b
来源：http://kj.newstarts.cn

[U87] JS：解构默认值
来源：http://ph.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://eq.szsharing.cn

[U88] JS：对象展开合并
来源：http://yy.9csxet.cn

{ ...a, ...b }
来源：http://pu.gzmigu.cn

[U89] JS：数组去重
来源：http://rc.colortex.cn

[...new Set(arr)]
来源：http://bt.newstarts.cn

[U90] JS：数字数组排序
来源：http://xg.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://eh.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://oe.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qb.muxihuayi.cn

[U92] JS：深拷贝
来源：http://wh.hnjuh.cn

structuredClone(obj)
来源：http://cl.wgjwhj.cn

[U93] JS：模板字符串
来源：http://yg.jianghongdianzi.cn

`共 ${n} 条`
来源：http://ui.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://hv.jctech888.com.cn

const double = x => x * 2;
来源：http://kp.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://bc.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://fr.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://sp.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vy.shxzukj.cn

[U97] JS：并发请求
来源：http://gl.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bg.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://bb.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kk.nicolike.cn

[U99] JS：事件监听
来源：http://bx.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://fn.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://kx.521024.cn

document.querySelector(".item")
来源：http://gq.chemitech.net.cn

[U101] JS：classList 操作
来源：http://yx.jctech888.com.cn

el.classList.toggle("active")
来源：http://hr.hnjuh.cn

[U102] JS：本地存储
来源：http://rc.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jd.shxzukj.cn

[U103] JS：定时器
来源：http://sn.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lb.nszjky.cn

[U104] JS：防抖
来源：http://hi.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mv.lnxyls.cn

[U105] JS：节流
来源：http://dr.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sw.haigaiapp.cn

[U106] JS：日期格式化
来源：http://og.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pi.szxytkj.cn

[U107] JS：数字千分位
来源：http://xj.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ni.nicolike.cn

[U108] JS：随机整数
来源：http://jr.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hc.gzmigu.cn

[U109] JS：数组分组
来源：http://tj.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://tc.asd995.cn

[U110] JS：数组分块
来源：http://pl.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qi.szxytkj.cn

[U111] JS：对象转 Map
来源：http://go.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://ni.yuexingan06.cn

[U112] JS：字符串补位
来源：http://ih.yuexingan06.cn

"7".padStart(3, "0")
来源：http://gc.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://on.asd995.cn

s.replaceAll("a", "b")
来源：http://fe.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://hb.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ek.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://ke.gzmigu.cn

crypto.randomUUID()
来源：http://ba.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://ef.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://ag.jctech888.com.cn

[U117] JS：单元测试
来源：http://xr.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://ep.colortex.cn

[U118] JS：开发服务器
来源：http://pf.hahajie.cn

npm i -D vite;  npx vite
来源：http://gt.haigaiapp.cn

[U119] JS：生产构建
来源：http://dp.yuexingan06.cn

npx vite build
来源：http://ek.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://ah.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://gv.yuexingan06.cn

================================================================================
来源：http://tl.shxzukj.cn

统计汇总
来源：http://ya.szxytkj.cn

================================================================================
来源：http://mb.nicolike.cn

按语言统计（条）：
来源：http://vh.lnxyls.cn

Python ......... 252
来源：http://pm.nszjky.cn

PHP ............ 252
来源：http://pm.szsharing.cn

JavaScript ..... 252
来源：http://dp.newstarts.cn

TypeScript ..... 212
来源：http://wj.lnxyls.cn

Java ........... 212
来源：http://ha.lnxyls.cn

Go ............. 212
来源：http://lu.shtwfgs.cn

Ruby ........... 212
来源：http://ab.wgjwhj.cn

C# ............. 212
来源：http://ao.asd995.cn

C .............. 30
来源：http://tn.szsharing.cn

C++ ............ 30
来源：http://kn.colortex.cn

SQL ............ 90
来源：http://xl.huanxung.cn

Bash ........... 80
来源：http://tp.jianghongdianzi.cn

Kotlin ......... 15
来源：http://zb.9csxet.cn

Swift .......... 15
来源：http://ac.shxzskj.cn

Lua ............ 10
来源：http://sl.bjjhwx.cn

Perl ........... 10
来源：http://uk.nicolike.cn

Scala .......... 10
来源：http://ai.haigaiapp.cn

------------------------------------
来源：http://ww.nicolike.cn

合计 ........... 2106 条
来源：http://xl.521024.cn

按章节统计：
来源：http://sw.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://za.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://td.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://no.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lj.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://br.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rj.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lj.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://av.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jr.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://an.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kp.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hv.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mg.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jy.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eq.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ke.asd995.cn

Q SQL 专题                              90
来源：http://sx.yuntaijiaju.cn

R Bash 专题                             80
来源：http://uk.haigaiapp.cn

S C / C++ 专题                          60
来源：http://qu.shxzukj.cn

T 其他语言补充                          60
来源：http://jj.newstarts.cn

U 高频实用片段                         120
来源：http://vs.lnxyls.cn

------------------------------------
来源：http://vd.hnjuh.cn

合计                                  2106 条
来源：http://ss.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://av.hahajie.cn

使用提醒
来源：http://ni.nszjky.cn

--------------------------------------------------------------------------------
来源：http://vg.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://as.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tk.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tn.newstarts.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rq.gzmigu.cn

—— 文件结束 ——
来源：http://hs.colortex.cn

================================================================================
来源：http://cs.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://ut.colortex.cn

Common Programming Examples Cheat Book
来源：http://qn.nszjky.cn

================================================================================
来源：http://oj.szsharing.cn

【收录内容】
来源：http://bf.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nr.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jm.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://gr.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://my.jianghongdianzi.cn

【使用说明】
来源：http://pq.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tw.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ae.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ve.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qt.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://de.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://or.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ha.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rj.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ju.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lk.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dz.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rq.jianghongdianzi.cn

【文件统计】
来源：http://yv.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gm.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://os.shxzskj.cn

目  录
来源：http://nd.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://mc.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://so.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rp.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xf.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://et.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uc.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bs.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bw.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wh.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cl.jctech888.com.cn


<!-- 参考信息 -->