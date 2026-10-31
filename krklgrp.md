代发 wailian999

[U15] Py：高精度计时
来源：http://eo.jianghongdianzi.cn

t = time.perf_counter()
来源：http://gr.521024.cn

[U16] Py：命令行参数解析
来源：http://gd.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fo.haigaiapp.cn

[U17] Py：初始化日志
来源：http://hd.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://au.haigaiapp.cn

[U18] Py：预编译正则
来源：http://fx.huanxung.cn

pat = re.compile(r"\d+")
来源：http://ab.asd995.cn

[U19] Py：正则替换带回调
来源：http://aa.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xx.huanxung.cn

[U20] Py：缓存函数结果
来源：http://lu.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://qd.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://wi.nszjky.cn

@contextlib.contextmanager
来源：http://oq.hahajie.cn

[U22] Py：矩阵转置
来源：http://ui.hahajie.cn

list(zip(*m))
来源：http://yr.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://ua.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://np.jctech888.com.cn

[U24] Py：路径操作
来源：http://jq.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vu.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://ny.huixinmuqiang.cn

csv.DictReader(f)
来源：http://ah.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://yf.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vc.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://ii.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://yw.szxytkj.cn

[U28] Py：类型别名
来源：http://wm.shtwfgs.cn

UserId = int
来源：http://vu.chemitech.net.cn

[U29] Py：属性校验
来源：http://bq.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://vj.bookmarksfly.cn

[U30] Py：数据类
来源：http://vj.yuexingan06.cn

@dataclass(slots=True)
来源：http://eg.huixinmuqiang.cn

[U31] Py：单测
来源：http://we.huixinmuqiang.cn

python -m pytest -q
来源：http://um.szsharing.cn

[U32] Py：代码格式化
来源：http://pj.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://oc.shxzskj.cn

[U33] Py：打包发布
来源：http://sx.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://fe.bjjhwx.cn

[U34] Py：判断编码
来源：http://dg.hahajie.cn

chardet.detect(raw)
来源：http://rx.haigaiapp.cn

[U35] Py：发送邮件
来源：http://ko.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eh.asd995.cn

[U36] Py：定时任务
来源：http://xj.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://mw.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://xq.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lb.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://mj.shxzskj.cn

Path(__file__).resolve().parent
来源：http://od.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://xa.shtwfgs.cn

sys.stdout.isatty()
来源：http://um.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://mr.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://gl.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://yo.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ce.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://vf.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cq.nszjky.cn

[U43] PHP：声明命名空间
来源：http://hu.jctech888.com.cn

namespace App\Http;
来源：http://dj.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://gh.bookmarksfly.cn

declare(strict_types=1);
来源：http://nu.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://xm.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ul.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://uy.521024.cn

?string $name = null
来源：http://xd.panjiajie.cn

[U47] PHP：联合类型
来源：http://gp.jctech888.com.cn

int|string $id
来源：http://cu.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://jx.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mb.newstarts.cn

[U49] PHP：只读属性
来源：http://gh.jianghongdianzi.cn

public readonly string $name
来源：http://sq.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://ko.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://wd.shtwfgs.cn

[U51] PHP：数组解构
来源：http://ga.chemitech.net.cn

[$a, $b] = $arr;
来源：http://us.gzmigu.cn

[U52] PHP：箭头函数
来源：http://ab.521024.cn

$double = fn($x) => $x * 2;
来源：http://ax.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://jc.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://it.szxytkj.cn

[U54] PHP：空安全调用
来源：http://dt.wgjwhj.cn

$obj?->method()
来源：http://ig.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://fr.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nt.chemitech.net.cn

[U56] PHP：命名参数
来源：http://vs.wgjwhj.cn

f(a: 1, b: 2)
来源：http://my.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://cr.shtwfgs.cn

"值: {$a}"
来源：http://ex.huanxung.cn

[U58] PHP：数组三件套
来源：http://tm.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ax.panjiajie.cn

[U59] PHP：自定义排序
来源：http://kg.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oo.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://lh.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gz.szsharing.cn

[U61] PHP：正则
来源：http://ju.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rf.gzmigu.cn

[U62] PHP：日期对象
来源：http://rj.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ar.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://sk.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kx.hahajie.cn

[U64] PHP：目录遍历
来源：http://kz.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://em.jctech888.com.cn

[U65] PHP：会话
来源：http://ss.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cs.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://mg.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fa.newstarts.cn

[U67] PHP：处理文件上传
来源：http://zt.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hh.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://hm.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iu.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://wj.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bn.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://bm.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gj.newstarts.cn

[U71] PHP：抛出异常
来源：http://oe.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://vd.shxzukj.cn

[U72] PHP：写错误日志
来源：http://sp.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://sz.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://eb.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://lu.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://hh.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://wi.gzmigu.cn

[U75] PHP：依赖注入
来源：http://tw.yuexingan06.cn

composer require psr/container
来源：http://ww.bjjhwx.cn

[U76] PHP：简单路由
来源：http://yi.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iy.lnxyls.cn

[U77] PHP：模板渲染
来源：http://sf.hnjuh.cn

composer require twig/twig
来源：http://qv.szxytkj.cn

[U78] PHP：单元测试
来源：http://xl.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://qt.hnjuh.cn

[U79] PHP：静态分析
来源：http://tl.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://gj.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://gv.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lx.gzmigu.cn

[U81] JS：初始化项目
来源：http://be.colortex.cn

npm init -y;  npm i express
来源：http://ih.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://gy.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lm.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://ia.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://js.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://ky.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cy.gzmigu.cn

[U85] JS：可选链
来源：http://ib.yuntaijiaju.cn

a?.b?.c
来源：http://ae.yuexingan06.cn

[U86] JS：空值合并
来源：http://rm.huixinmuqiang.cn

a ?? b
来源：http://ys.9csxet.cn

[U87] JS：解构默认值
来源：http://ow.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://vb.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://ts.szsharing.cn

{ ...a, ...b }
来源：http://nb.nicolike.cn

[U89] JS：数组去重
来源：http://yn.wgjwhj.cn

[...new Set(arr)]
来源：http://fm.szsharing.cn

[U90] JS：数字数组排序
来源：http://jn.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://jp.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://ks.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rc.521024.cn

[U92] JS：深拷贝
来源：http://lx.huixinmuqiang.cn

structuredClone(obj)
来源：http://sj.nicolike.cn

[U93] JS：模板字符串
来源：http://ya.bookmarksfly.cn

`共 ${n} 条`
来源：http://tq.chemitech.net.cn

[U94] JS：箭头函数
来源：http://wo.huixinmuqiang.cn

const double = x => x * 2;
来源：http://bw.panjiajie.cn

[U95] JS：Promise 包装
来源：http://nd.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://xw.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://cq.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xa.hnjuh.cn

[U97] JS：并发请求
来源：http://fv.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bd.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://ir.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tg.nszjky.cn

[U99] JS：事件监听
来源：http://tu.nicolike.cn

el.addEventListener("click", e => {})
来源：http://fu.hahajie.cn

[U100] JS：DOM 查询
来源：http://ru.szxytkj.cn

document.querySelector(".item")
来源：http://an.shxzskj.cn

[U101] JS：classList 操作
来源：http://hb.asd995.cn

el.classList.toggle("active")
来源：http://ai.gzmigu.cn

[U102] JS：本地存储
来源：http://ho.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bj.gzmigu.cn

[U103] JS：定时器
来源：http://sr.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ac.colortex.cn

[U104] JS：防抖
来源：http://ye.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jo.panjiajie.cn

[U105] JS：节流
来源：http://vo.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pp.asd995.cn

[U106] JS：日期格式化
来源：http://am.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hh.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://mr.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://or.jctech888.com.cn

[U108] JS：随机整数
来源：http://vh.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://br.haigaiapp.cn

[U109] JS：数组分组
来源：http://rs.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://xy.shxzukj.cn

[U110] JS：数组分块
来源：http://ml.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zv.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://kt.9csxet.cn

new Map(Object.entries(obj))
来源：http://tp.yuexingan06.cn

[U112] JS：字符串补位
来源：http://ks.shxzskj.cn

"7".padStart(3, "0")
来源：http://kd.panjiajie.cn

[U113] JS：正则替换全部
来源：http://el.gzmigu.cn

s.replaceAll("a", "b")
来源：http://bs.9csxet.cn

[U114] JS：JSON 深比较
来源：http://vh.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sm.newstarts.cn

[U115] JS：生成 UUID
来源：http://yt.huixinmuqiang.cn

crypto.randomUUID()
来源：http://nb.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://dd.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://ka.shxzukj.cn

[U117] JS：单元测试
来源：http://ga.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://ab.hnjuh.cn

[U118] JS：开发服务器
来源：http://fs.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://uc.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://je.shxzskj.cn

npx vite build
来源：http://nb.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://at.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://hj.nicolike.cn

================================================================================
来源：http://om.huixiangedu.cn

统计汇总
来源：http://ez.wgjwhj.cn

================================================================================
来源：http://sa.jianghongdianzi.cn

按语言统计（条）：
来源：http://qt.yuntaijiaju.cn

Python ......... 252
来源：http://et.yuexingan06.cn

PHP ............ 252
来源：http://kw.nicolike.cn

JavaScript ..... 252
来源：http://sd.huanxung.cn

TypeScript ..... 212
来源：http://xb.hnjuh.cn

Java ........... 212
来源：http://es.muxihuayi.cn

Go ............. 212
来源：http://ay.huixinmuqiang.cn

Ruby ........... 212
来源：http://nj.jctech888.com.cn

C# ............. 212
来源：http://ou.shtwfgs.cn

C .............. 30
来源：http://yr.hnjuh.cn

C++ ............ 30
来源：http://um.newstarts.cn

SQL ............ 90
来源：http://yq.huixinmuqiang.cn

Bash ........... 80
来源：http://xe.jianghongdianzi.cn

Kotlin ......... 15
来源：http://sw.bookmarksfly.cn

Swift .......... 15
来源：http://ra.huanxung.cn

Lua ............ 10
来源：http://bs.haigaiapp.cn

Perl ........... 10
来源：http://ay.colortex.cn

Scala .......... 10
来源：http://uq.gzmigu.cn

------------------------------------
来源：http://he.yuexingan06.cn

合计 ........... 2106 条
来源：http://ml.huixinmuqiang.cn

按章节统计：
来源：http://xl.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vb.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ox.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gx.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ku.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uf.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xf.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hj.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gm.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nl.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fg.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zm.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bs.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bc.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zr.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yi.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ok.asd995.cn

Q SQL 专题                              90
来源：http://np.hnjuh.cn

R Bash 专题                             80
来源：http://vh.newstarts.cn

S C / C++ 专题                          60
来源：http://bj.huixiangedu.cn

T 其他语言补充                          60
来源：http://ho.521024.cn

U 高频实用片段                         120
来源：http://xe.huixinmuqiang.cn

------------------------------------
来源：http://gy.huixinmuqiang.cn

合计                                  2106 条
来源：http://ie.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://as.9csxet.cn

使用提醒
来源：http://lg.9csxet.cn

--------------------------------------------------------------------------------
来源：http://jr.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lm.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cx.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://aa.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qo.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iq.chemitech.net.cn

—— 文件结束 ——
来源：http://tx.huixiangedu.cn

================================================================================
来源：http://ce.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://du.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://sx.huanxung.cn

================================================================================
来源：http://jt.shxzukj.cn

【收录内容】
来源：http://dz.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ag.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mb.huanxung.cn

SQL · Bash · C · C++
来源：http://bf.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ed.9csxet.cn

【使用说明】
来源：http://xn.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://em.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qp.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uw.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://af.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uz.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lp.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hu.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cb.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://se.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ow.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ef.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gd.panjiajie.cn

【文件统计】
来源：http://pb.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nc.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ut.521024.cn

目  录
来源：http://sg.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://lc.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cu.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mn.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xo.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kg.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nk.muxihuayi.cn


<!-- 参考信息 -->