代发 wailian999

[U13] Py：固定长度队列
来源：http://yc.huixinmuqiang.cn

deque(maxlen=10)
来源：http://gd.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://sg.muxihuayi.cn

defaultdict(list)
来源：http://no.lnxyls.cn

[U15] Py：高精度计时
来源：http://ew.bjjhwx.cn

t = time.perf_counter()
来源：http://hf.huanxung.cn

[U16] Py：命令行参数解析
来源：http://sc.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ih.haigaiapp.cn

[U17] Py：初始化日志
来源：http://my.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://mh.chemitech.net.cn

[U18] Py：预编译正则
来源：http://ux.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://do.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://ix.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ir.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://ve.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://pf.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://kz.szsharing.cn

@contextlib.contextmanager
来源：http://iy.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://ss.yuexingan06.cn

list(zip(*m))
来源：http://ue.9csxet.cn

[U23] Py：分块读取大文件
来源：http://ly.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ky.colortex.cn

[U24] Py：路径操作
来源：http://md.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bf.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://ez.muxihuayi.cn

csv.DictReader(f)
来源：http://xa.hahajie.cn

[U26] Py：并发下载
来源：http://to.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ag.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://hi.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://up.nszjky.cn

[U28] Py：类型别名
来源：http://la.lnxyls.cn

UserId = int
来源：http://th.panjiajie.cn

[U29] Py：属性校验
来源：http://xw.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://sf.521024.cn

[U30] Py：数据类
来源：http://cu.lnxyls.cn

@dataclass(slots=True)
来源：http://ot.hnjuh.cn

[U31] Py：单测
来源：http://cc.szxytkj.cn

python -m pytest -q
来源：http://sd.huixiangedu.cn

[U32] Py：代码格式化
来源：http://pm.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://lk.shtwfgs.cn

[U33] Py：打包发布
来源：http://ci.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://vz.nicolike.cn

[U34] Py：判断编码
来源：http://jd.lnxyls.cn

chardet.detect(raw)
来源：http://nb.shtwfgs.cn

[U35] Py：发送邮件
来源：http://zi.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lu.colortex.cn

[U36] Py：定时任务
来源：http://xr.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://pk.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://nv.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cu.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://qc.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://nv.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://ni.gzmigu.cn

sys.stdout.isatty()
来源：http://ip.asd995.cn

[U40] Py：打印到标准错误
来源：http://tk.hahajie.cn

print("err", file=sys.stderr)
来源：http://io.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://en.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wk.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://wm.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hs.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://pi.hnjuh.cn

namespace App\Http;
来源：http://tb.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://es.yuexingan06.cn

declare(strict_types=1);
来源：http://zv.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://dj.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gc.asd995.cn

[U46] PHP：可空类型
来源：http://ro.panjiajie.cn

?string $name = null
来源：http://hp.shxzukj.cn

[U47] PHP：联合类型
来源：http://lx.shtwfgs.cn

int|string $id
来源：http://yt.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://ql.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mc.hahajie.cn

[U49] PHP：只读属性
来源：http://rq.bjjhwx.cn

public readonly string $name
来源：http://cl.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://qo.szxytkj.cn

public function __construct(private int $id) {}
来源：http://wd.521024.cn

[U51] PHP：数组解构
来源：http://kn.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://eo.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://ao.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://aa.nicolike.cn

[U53] PHP：空合并运算符
来源：http://jg.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://mb.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://wy.panjiajie.cn

$obj?->method()
来源：http://ik.newstarts.cn

[U55] PHP：match 表达式
来源：http://zr.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pd.huanxung.cn

[U56] PHP：命名参数
来源：http://zw.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ms.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://gx.nszjky.cn

"值: {$a}"
来源：http://vx.hnjuh.cn

[U58] PHP：数组三件套
来源：http://rq.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sc.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://eg.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ql.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://eg.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zb.wgjwhj.cn

[U61] PHP：正则
来源：http://hn.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rf.lnxyls.cn

[U62] PHP：日期对象
来源：http://fm.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tp.haigaiapp.cn

[U63] PHP：文件读写
来源：http://ic.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hq.huanxung.cn

[U64] PHP：目录遍历
来源：http://zy.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://xp.shxzukj.cn

[U65] PHP：会话
来源：http://xv.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cu.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://zj.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rd.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://te.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jb.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://qs.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kj.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://dz.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gc.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://jq.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lo.gzmigu.cn

[U71] PHP：抛出异常
来源：http://jp.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://ew.colortex.cn

[U72] PHP：写错误日志
来源：http://lx.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://gq.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://yq.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://kx.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://uw.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://gl.shxzskj.cn

[U75] PHP：依赖注入
来源：http://fx.chemitech.net.cn

composer require psr/container
来源：http://pe.huanxung.cn

[U76] PHP：简单路由
来源：http://mf.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xu.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://et.szxytkj.cn

composer require twig/twig
来源：http://xu.shxzskj.cn

[U78] PHP：单元测试
来源：http://as.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://ov.jctech888.com.cn

[U79] PHP：静态分析
来源：http://ao.521024.cn

composer require --dev phpstan/phpstan
来源：http://pm.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://ov.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dp.521024.cn

[U81] JS：初始化项目
来源：http://wb.szsharing.cn

npm init -y;  npm i express
来源：http://pv.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://as.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ch.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://yn.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rj.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://xv.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yi.nicolike.cn

[U85] JS：可选链
来源：http://ui.panjiajie.cn

a?.b?.c
来源：http://zt.nicolike.cn

[U86] JS：空值合并
来源：http://pp.bjjhwx.cn

a ?? b
来源：http://bd.panjiajie.cn

[U87] JS：解构默认值
来源：http://pp.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://te.newstarts.cn

[U88] JS：对象展开合并
来源：http://vr.shxzskj.cn

{ ...a, ...b }
来源：http://mo.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://wa.yuntaijiaju.cn

[...new Set(arr)]
来源：http://cx.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://eb.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://bk.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://gu.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://de.panjiajie.cn

[U92] JS：深拷贝
来源：http://sp.521024.cn

structuredClone(obj)
来源：http://ub.nicolike.cn

[U93] JS：模板字符串
来源：http://ae.521024.cn

`共 ${n} 条`
来源：http://gd.bjjhwx.cn

[U94] JS：箭头函数
来源：http://ef.szsharing.cn

const double = x => x * 2;
来源：http://ka.gzmigu.cn

[U95] JS：Promise 包装
来源：http://sc.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://qk.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://wx.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lt.muxihuayi.cn

[U97] JS：并发请求
来源：http://vw.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ja.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://of.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kh.9csxet.cn

[U99] JS：事件监听
来源：http://gr.521024.cn

el.addEventListener("click", e => {})
来源：http://aw.hnjuh.cn

[U100] JS：DOM 查询
来源：http://kz.9csxet.cn

document.querySelector(".item")
来源：http://jw.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://so.bjjhwx.cn

el.classList.toggle("active")
来源：http://qs.lnxyls.cn

[U102] JS：本地存储
来源：http://uj.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xa.9csxet.cn

[U103] JS：定时器
来源：http://ia.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ov.jctech888.com.cn

[U104] JS：防抖
来源：http://qp.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hi.hnjuh.cn

[U105] JS：节流
来源：http://bt.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gb.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://gr.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fb.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://gx.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nr.szsharing.cn

[U108] JS：随机整数
来源：http://hv.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://el.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://jt.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://mp.shtwfgs.cn

[U110] JS：数组分块
来源：http://js.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gi.gzmigu.cn

[U111] JS：对象转 Map
来源：http://go.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://rt.szxytkj.cn

[U112] JS：字符串补位
来源：http://kv.newstarts.cn

"7".padStart(3, "0")
来源：http://lz.hnjuh.cn

[U113] JS：正则替换全部
来源：http://oi.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://zt.9csxet.cn

[U114] JS：JSON 深比较
来源：http://rk.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yb.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://bq.bookmarksfly.cn

crypto.randomUUID()
来源：http://ja.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://tx.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://ir.huixiangedu.cn

[U117] JS：单元测试
来源：http://mb.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://jd.shxzskj.cn

[U118] JS：开发服务器
来源：http://da.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://tn.hnjuh.cn

[U119] JS：生产构建
来源：http://dq.newstarts.cn

npx vite build
来源：http://lz.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://tf.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://aq.chemitech.net.cn

================================================================================
来源：http://rg.bookmarksfly.cn

统计汇总
来源：http://gu.shtwfgs.cn

================================================================================
来源：http://th.jianghongdianzi.cn

按语言统计（条）：
来源：http://me.nszjky.cn

Python ......... 252
来源：http://lq.chemitech.net.cn

PHP ............ 252
来源：http://ww.jctech888.com.cn

JavaScript ..... 252
来源：http://xi.nicolike.cn

TypeScript ..... 212
来源：http://vj.521024.cn

Java ........... 212
来源：http://oq.hahajie.cn

Go ............. 212
来源：http://ch.hnjuh.cn

Ruby ........... 212
来源：http://ks.lnxyls.cn

C# ............. 212
来源：http://zx.yuntaijiaju.cn

C .............. 30
来源：http://kt.bjjhwx.cn

C++ ............ 30
来源：http://bz.yuexingan06.cn

SQL ............ 90
来源：http://pn.521024.cn

Bash ........... 80
来源：http://qv.huixinmuqiang.cn

Kotlin ......... 15
来源：http://fh.9csxet.cn

Swift .......... 15
来源：http://ob.nicolike.cn

Lua ............ 10
来源：http://aj.shxzskj.cn

Perl ........... 10
来源：http://tv.jctech888.com.cn

Scala .......... 10
来源：http://pj.huixinmuqiang.cn

------------------------------------
来源：http://uh.szxytkj.cn

合计 ........... 2106 条
来源：http://yt.huanxung.cn

按章节统计：
来源：http://xe.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tt.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xe.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://um.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nb.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lc.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vv.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yy.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fi.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rs.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mu.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vj.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pn.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ee.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uh.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iq.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nu.szsharing.cn

Q SQL 专题                              90
来源：http://xj.jianghongdianzi.cn

R Bash 专题                             80
来源：http://ew.lnxyls.cn

S C / C++ 专题                          60
来源：http://nu.chemitech.net.cn

T 其他语言补充                          60
来源：http://ey.hnjuh.cn

U 高频实用片段                         120
来源：http://va.shxzskj.cn

------------------------------------
来源：http://mu.jianghongdianzi.cn

合计                                  2106 条
来源：http://fr.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://uu.nicolike.cn

使用提醒
来源：http://ot.colortex.cn

--------------------------------------------------------------------------------
来源：http://tp.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gr.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jc.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xy.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://di.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ft.shtwfgs.cn

—— 文件结束 ——
来源：http://gz.bookmarksfly.cn

================================================================================
来源：http://qf.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://kc.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://ip.nszjky.cn

================================================================================
来源：http://uh.colortex.cn

【收录内容】
来源：http://zi.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ie.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sr.nszjky.cn

SQL · Bash · C · C++
来源：http://ui.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://et.shtwfgs.cn

【使用说明】
来源：http://km.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oz.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ye.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gb.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mv.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uy.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yx.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hs.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lw.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vt.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mx.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lk.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wu.shxzukj.cn

【文件统计】
来源：http://ah.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fx.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://vi.muxihuayi.cn

目  录
来源：http://tm.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://az.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ag.haigaiapp.cn


<!-- 参考信息 -->