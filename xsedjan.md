代发 wailian999

[U17] Py：初始化日志
来源：http://wg.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://bn.shtwfgs.cn

[U18] Py：预编译正则
来源：http://mp.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://ox.521024.cn

[U19] Py：正则替换带回调
来源：http://dl.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dh.szsharing.cn

[U20] Py：缓存函数结果
来源：http://wz.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://yb.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://hm.yuexingan06.cn

@contextlib.contextmanager
来源：http://sp.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://to.haigaiapp.cn

list(zip(*m))
来源：http://uy.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://tq.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dd.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://tr.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yj.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://bw.bjjhwx.cn

csv.DictReader(f)
来源：http://ih.bookmarksfly.cn

[U26] Py：并发下载
来源：http://vn.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mx.szsharing.cn

[U27] Py：异步 HTTP
来源：http://jp.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ei.9csxet.cn

[U28] Py：类型别名
来源：http://ry.wgjwhj.cn

UserId = int
来源：http://tq.haigaiapp.cn

[U29] Py：属性校验
来源：http://in.newstarts.cn

@property 与 @x.setter 配合
来源：http://vu.lnxyls.cn

[U30] Py：数据类
来源：http://kx.jctech888.com.cn

@dataclass(slots=True)
来源：http://zc.jctech888.com.cn

[U31] Py：单测
来源：http://bc.nszjky.cn

python -m pytest -q
来源：http://fh.szsharing.cn

[U32] Py：代码格式化
来源：http://it.521024.cn

ruff format . && ruff check --fix .
来源：http://dx.521024.cn

[U33] Py：打包发布
来源：http://yq.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://kz.9csxet.cn

[U34] Py：判断编码
来源：http://eh.panjiajie.cn

chardet.detect(raw)
来源：http://ab.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://ay.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ww.nszjky.cn

[U36] Py：定时任务
来源：http://hk.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://lf.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://zl.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kd.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://yj.hnjuh.cn

Path(__file__).resolve().parent
来源：http://yt.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://uk.szsharing.cn

sys.stdout.isatty()
来源：http://yo.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://cv.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://qw.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://ae.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://af.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://bc.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ag.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://qn.muxihuayi.cn

namespace App\Http;
来源：http://gl.colortex.cn

[U44] PHP：开启严格类型
来源：http://gs.shxzskj.cn

declare(strict_types=1);
来源：http://eg.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://ki.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tz.shxzskj.cn

[U46] PHP：可空类型
来源：http://fb.szsharing.cn

?string $name = null
来源：http://fx.nicolike.cn

[U47] PHP：联合类型
来源：http://ww.huixinmuqiang.cn

int|string $id
来源：http://ep.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://mx.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vo.szxytkj.cn

[U49] PHP：只读属性
来源：http://ls.nicolike.cn

public readonly string $name
来源：http://ib.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://ry.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://vs.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://nq.shxzukj.cn

[$a, $b] = $arr;
来源：http://eq.shxzukj.cn

[U52] PHP：箭头函数
来源：http://ci.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://gc.nicolike.cn

[U53] PHP：空合并运算符
来源：http://zu.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://eu.hnjuh.cn

[U54] PHP：空安全调用
来源：http://ck.szxytkj.cn

$obj?->method()
来源：http://dp.521024.cn

[U55] PHP：match 表达式
来源：http://vs.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qs.hahajie.cn

[U56] PHP：命名参数
来源：http://gw.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://mj.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://gw.huixinmuqiang.cn

"值: {$a}"
来源：http://vu.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://aa.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vs.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://eb.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kr.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://mv.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nb.yuntaijiaju.cn

[U61] PHP：正则
来源：http://ds.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ch.szsharing.cn

[U62] PHP：日期对象
来源：http://uc.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ry.521024.cn

[U63] PHP：文件读写
来源：http://jq.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://um.shxzskj.cn

[U64] PHP：目录遍历
来源：http://wi.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://ad.asd995.cn

[U65] PHP：会话
来源：http://fc.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nd.colortex.cn

[U66] PHP：设置 Cookie
来源：http://sh.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xc.newstarts.cn

[U67] PHP：处理文件上传
来源：http://ji.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rr.9csxet.cn

[U68] PHP：PDO 连接
来源：http://ih.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://us.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://ly.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tt.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://gw.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zs.panjiajie.cn

[U71] PHP：抛出异常
来源：http://yt.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://qj.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://ho.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://dh.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://dj.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://hg.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://gn.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://bb.colortex.cn

[U75] PHP：依赖注入
来源：http://am.shxzukj.cn

composer require psr/container
来源：http://cr.szsharing.cn

[U76] PHP：简单路由
来源：http://cj.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://by.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://df.asd995.cn

composer require twig/twig
来源：http://zv.nicolike.cn

[U78] PHP：单元测试
来源：http://vs.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://hk.huixiangedu.cn

[U79] PHP：静态分析
来源：http://pw.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://dz.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://lw.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ic.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://hz.bookmarksfly.cn

npm init -y;  npm i express
来源：http://ij.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://um.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yv.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://io.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lg.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://oe.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://el.szxytkj.cn

[U85] JS：可选链
来源：http://kh.yuntaijiaju.cn

a?.b?.c
来源：http://fm.521024.cn

[U86] JS：空值合并
来源：http://be.hahajie.cn

a ?? b
来源：http://sh.hnjuh.cn

[U87] JS：解构默认值
来源：http://bf.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://vd.nicolike.cn

[U88] JS：对象展开合并
来源：http://gu.huanxung.cn

{ ...a, ...b }
来源：http://gc.wgjwhj.cn

[U89] JS：数组去重
来源：http://hq.chemitech.net.cn

[...new Set(arr)]
来源：http://dc.colortex.cn

[U90] JS：数字数组排序
来源：http://rd.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://rv.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://hu.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fh.lnxyls.cn

[U92] JS：深拷贝
来源：http://xo.colortex.cn

structuredClone(obj)
来源：http://zv.huixiangedu.cn

[U93] JS：模板字符串
来源：http://lz.yuexingan06.cn

`共 ${n} 条`
来源：http://iq.lnxyls.cn

[U94] JS：箭头函数
来源：http://tk.shxzukj.cn

const double = x => x * 2;
来源：http://xo.hnjuh.cn

[U95] JS：Promise 包装
来源：http://wa.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://sb.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://bi.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bg.nszjky.cn

[U97] JS：并发请求
来源：http://ru.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ir.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://vz.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rw.nszjky.cn

[U99] JS：事件监听
来源：http://wy.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://ai.nszjky.cn

[U100] JS：DOM 查询
来源：http://br.wgjwhj.cn

document.querySelector(".item")
来源：http://dx.shxzukj.cn

[U101] JS：classList 操作
来源：http://hg.gzmigu.cn

el.classList.toggle("active")
来源：http://la.muxihuayi.cn

[U102] JS：本地存储
来源：http://bf.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wn.hnjuh.cn

[U103] JS：定时器
来源：http://ms.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://td.huanxung.cn

[U104] JS：防抖
来源：http://tk.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vq.nszjky.cn

[U105] JS：节流
来源：http://ti.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gh.9csxet.cn

[U106] JS：日期格式化
来源：http://vd.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hp.jctech888.com.cn

[U107] JS：数字千分位
来源：http://ae.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iq.szxytkj.cn

[U108] JS：随机整数
来源：http://ws.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xe.newstarts.cn

[U109] JS：数组分组
来源：http://lq.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://hb.nicolike.cn

[U110] JS：数组分块
来源：http://tg.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yy.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://rt.9csxet.cn

new Map(Object.entries(obj))
来源：http://cz.jctech888.com.cn

[U112] JS：字符串补位
来源：http://ex.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://ws.newstarts.cn

[U113] JS：正则替换全部
来源：http://vr.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://zn.hahajie.cn

[U114] JS：JSON 深比较
来源：http://zj.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pi.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://wb.jianghongdianzi.cn

crypto.randomUUID()
来源：http://kp.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://eu.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://zo.chemitech.net.cn

[U117] JS：单元测试
来源：http://hz.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://et.jctech888.com.cn

[U118] JS：开发服务器
来源：http://my.gzmigu.cn

npm i -D vite;  npx vite
来源：http://oc.haigaiapp.cn

[U119] JS：生产构建
来源：http://ye.bookmarksfly.cn

npx vite build
来源：http://zc.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://lh.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://th.huixinmuqiang.cn

================================================================================
来源：http://wy.hnjuh.cn

统计汇总
来源：http://my.hnjuh.cn

================================================================================
来源：http://nv.newstarts.cn

按语言统计（条）：
来源：http://dz.jctech888.com.cn

Python ......... 252
来源：http://ki.newstarts.cn

PHP ............ 252
来源：http://ld.jctech888.com.cn

JavaScript ..... 252
来源：http://hi.huixinmuqiang.cn

TypeScript ..... 212
来源：http://ug.jctech888.com.cn

Java ........... 212
来源：http://pl.chemitech.net.cn

Go ............. 212
来源：http://st.wgjwhj.cn

Ruby ........... 212
来源：http://nn.szxytkj.cn

C# ............. 212
来源：http://nc.yuexingan06.cn

C .............. 30
来源：http://pk.bookmarksfly.cn

C++ ............ 30
来源：http://up.huixiangedu.cn

SQL ............ 90
来源：http://pm.gzmigu.cn

Bash ........... 80
来源：http://by.jianghongdianzi.cn

Kotlin ......... 15
来源：http://hl.hahajie.cn

Swift .......... 15
来源：http://kr.newstarts.cn

Lua ............ 10
来源：http://yo.szsharing.cn

Perl ........... 10
来源：http://uk.huanxung.cn

Scala .......... 10
来源：http://cx.huixiangedu.cn

------------------------------------
来源：http://hs.jctech888.com.cn

合计 ........... 2106 条
来源：http://ma.yuexingan06.cn

按章节统计：
来源：http://vw.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pg.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sp.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://an.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bo.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wn.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vc.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vj.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tl.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tx.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fp.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://os.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kz.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ev.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://du.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jw.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dk.hnjuh.cn

Q SQL 专题                              90
来源：http://fl.wgjwhj.cn

R Bash 专题                             80
来源：http://az.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://qk.bookmarksfly.cn

T 其他语言补充                          60
来源：http://tm.jctech888.com.cn

U 高频实用片段                         120
来源：http://xk.hnjuh.cn

------------------------------------
来源：http://yb.gzmigu.cn

合计                                  2106 条
来源：http://zc.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://xa.yuntaijiaju.cn

使用提醒
来源：http://xh.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://sh.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ij.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://om.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tj.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gn.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qa.nszjky.cn

—— 文件结束 ——
来源：http://fs.wgjwhj.cn

================================================================================
来源：http://ao.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://xu.521024.cn

Common Programming Examples Cheat Book
来源：http://hu.shxzskj.cn

================================================================================
来源：http://kg.huanxung.cn

【收录内容】
来源：http://ng.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mj.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oa.jctech888.com.cn

SQL · Bash · C · C++
来源：http://om.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hq.panjiajie.cn

【使用说明】
来源：http://wf.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xo.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://se.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gt.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ye.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sr.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fr.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fw.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pq.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gf.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iy.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qy.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jo.shtwfgs.cn

【文件统计】
来源：http://ei.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lw.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://uj.bookmarksfly.cn

目  录
来源：http://tv.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://wl.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mz.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ul.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vi.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jj.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fn.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uq.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yi.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sh.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ws.bookmarksfly.cn


<!-- 参考信息 -->