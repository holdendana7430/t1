代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fl.asd995.cn

================================================================================
来源：http://fs.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qc.newstarts.cn

================================================================================
来源：http://hb.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://zj.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lx.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ai.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fj.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://hd.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xy.szxytkj.cn

[U04] Py：变量调试打印
来源：http://zu.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nm.szsharing.cn

[U05] Py：列表去重且保序
来源：http://pt.521024.cn

list(dict.fromkeys(arr))
来源：http://es.hnjuh.cn

[U06] Py：合并两个字典
来源：http://dj.newstarts.cn

{**a, **b}
来源：http://uo.lnxyls.cn

[U07] Py：反转字典键值
来源：http://wd.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://is.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://bm.jctech888.com.cn

[y for x in nested for y in x]
来源：http://aq.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://bm.wgjwhj.cn

max(d, key=d.get)
来源：http://th.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://xl.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rf.newstarts.cn

[U11] Py：生成器表达式
来源：http://qi.gzmigu.cn

(x * 2 for x in arr)
来源：http://qw.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ji.9csxet.cn

Counter(arr).most_common(3)
来源：http://ni.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://pq.9csxet.cn

deque(maxlen=10)
来源：http://yt.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://ri.hahajie.cn

defaultdict(list)
来源：http://cp.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ip.nszjky.cn

t = time.perf_counter()
来源：http://iv.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://zj.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ve.shtwfgs.cn

[U17] Py：初始化日志
来源：http://qn.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://zc.9csxet.cn

[U18] Py：预编译正则
来源：http://ow.hahajie.cn

pat = re.compile(r"\d+")
来源：http://vx.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://za.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uj.colortex.cn

[U20] Py：缓存函数结果
来源：http://vh.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://cw.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://an.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://lb.huanxung.cn

[U22] Py：矩阵转置
来源：http://wh.yuntaijiaju.cn

list(zip(*m))
来源：http://zl.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://rn.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jb.muxihuayi.cn

[U24] Py：路径操作
来源：http://jt.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zw.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://lp.hahajie.cn

csv.DictReader(f)
来源：http://bv.huanxung.cn

[U26] Py：并发下载
来源：http://tw.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ne.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://jh.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://rf.wgjwhj.cn

[U28] Py：类型别名
来源：http://kb.nicolike.cn

UserId = int
来源：http://mm.colortex.cn

[U29] Py：属性校验
来源：http://fx.panjiajie.cn

@property 与 @x.setter 配合
来源：http://qu.hnjuh.cn

[U30] Py：数据类
来源：http://ei.shxzukj.cn

@dataclass(slots=True)
来源：http://bu.hnjuh.cn

[U31] Py：单测
来源：http://ol.haigaiapp.cn

python -m pytest -q
来源：http://re.hahajie.cn

[U32] Py：代码格式化
来源：http://md.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://wp.huixiangedu.cn

[U33] Py：打包发布
来源：http://et.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://rr.hnjuh.cn

[U34] Py：判断编码
来源：http://df.yuexingan06.cn

chardet.detect(raw)
来源：http://jh.panjiajie.cn

[U35] Py：发送邮件
来源：http://qs.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zb.521024.cn

[U36] Py：定时任务
来源：http://qa.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://zk.szxytkj.cn

[U37] Py：读写 Excel
来源：http://gb.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rd.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://wj.9csxet.cn

Path(__file__).resolve().parent
来源：http://zb.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://yg.nszjky.cn

sys.stdout.isatty()
来源：http://ru.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://yw.huanxung.cn

print("err", file=sys.stderr)
来源：http://ub.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://jb.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yy.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://um.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yi.szsharing.cn

[U43] PHP：声明命名空间
来源：http://bp.yuexingan06.cn

namespace App\Http;
来源：http://ng.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://ha.muxihuayi.cn

declare(strict_types=1);
来源：http://rz.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://ni.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xg.haigaiapp.cn

[U46] PHP：可空类型
来源：http://fc.panjiajie.cn

?string $name = null
来源：http://ze.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://se.jianghongdianzi.cn

int|string $id
来源：http://xk.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://kw.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ys.wgjwhj.cn

[U49] PHP：只读属性
来源：http://iy.colortex.cn

public readonly string $name
来源：http://uj.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://tz.hnjuh.cn

public function __construct(private int $id) {}
来源：http://pe.huixiangedu.cn

[U51] PHP：数组解构
来源：http://cb.9csxet.cn

[$a, $b] = $arr;
来源：http://ob.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://ky.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://yn.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://mh.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://zt.hnjuh.cn

[U54] PHP：空安全调用
来源：http://ev.muxihuayi.cn

$obj?->method()
来源：http://lg.nicolike.cn

[U55] PHP：match 表达式
来源：http://ys.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ja.muxihuayi.cn

[U56] PHP：命名参数
来源：http://ag.shxzskj.cn

f(a: 1, b: 2)
来源：http://da.nicolike.cn

[U57] PHP：字符串插值
来源：http://hq.yuexingan06.cn

"值: {$a}"
来源：http://ds.9csxet.cn

[U58] PHP：数组三件套
来源：http://rm.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ch.huanxung.cn

[U59] PHP：自定义排序
来源：http://bi.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://di.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://uk.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qc.asd995.cn

[U61] PHP：正则
来源：http://jj.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uq.jctech888.com.cn

[U62] PHP：日期对象
来源：http://ts.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sv.shxzukj.cn

[U63] PHP：文件读写
来源：http://ah.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://np.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://lj.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://et.chemitech.net.cn

[U65] PHP：会话
来源：http://eb.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ym.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://dm.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ur.9csxet.cn

[U67] PHP：处理文件上传
来源：http://ol.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://to.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://dt.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oi.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://om.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wx.newstarts.cn

[U70] PHP：PDO 事务
来源：http://tm.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hq.nicolike.cn

[U71] PHP：抛出异常
来源：http://qg.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://fs.colortex.cn

[U72] PHP：写错误日志
来源：http://gj.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://qm.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://of.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://nx.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://zp.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://vp.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://gr.newstarts.cn

composer require psr/container
来源：http://rr.shxzskj.cn

[U76] PHP：简单路由
来源：http://ci.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://go.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://ld.hnjuh.cn

composer require twig/twig
来源：http://xr.panjiajie.cn

[U78] PHP：单元测试
来源：http://fc.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://bn.colortex.cn

[U79] PHP：静态分析
来源：http://et.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://ip.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://pm.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xv.lnxyls.cn

[U81] JS：初始化项目
来源：http://xe.szsharing.cn

npm init -y;  npm i express
来源：http://ys.szsharing.cn

[U82] JS：package.json 脚本
来源：http://fp.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pg.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://vk.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vu.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://la.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dg.nszjky.cn

[U85] JS：可选链
来源：http://qm.chemitech.net.cn

a?.b?.c
来源：http://mf.9csxet.cn

[U86] JS：空值合并
来源：http://my.yuntaijiaju.cn

a ?? b
来源：http://wy.hahajie.cn

[U87] JS：解构默认值
来源：http://jr.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://hc.asd995.cn

[U88] JS：对象展开合并
来源：http://iw.jianghongdianzi.cn

{ ...a, ...b }
来源：http://og.chemitech.net.cn

[U89] JS：数组去重
来源：http://jc.muxihuayi.cn

[...new Set(arr)]
来源：http://ka.huanxung.cn

[U90] JS：数字数组排序
来源：http://ir.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://no.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://cm.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pk.colortex.cn

[U92] JS：深拷贝
来源：http://cf.bookmarksfly.cn

structuredClone(obj)
来源：http://an.jctech888.com.cn

[U93] JS：模板字符串
来源：http://ci.bjjhwx.cn

`共 ${n} 条`
来源：http://oq.panjiajie.cn

[U94] JS：箭头函数
来源：http://et.wgjwhj.cn

const double = x => x * 2;
来源：http://gg.hnjuh.cn

[U95] JS：Promise 包装
来源：http://kk.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://fq.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://zg.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ai.yuexingan06.cn

[U97] JS：并发请求
来源：http://un.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ce.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://fl.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ys.shtwfgs.cn

[U99] JS：事件监听
来源：http://ix.hahajie.cn

el.addEventListener("click", e => {})
来源：http://ml.panjiajie.cn

[U100] JS：DOM 查询
来源：http://wr.haigaiapp.cn

document.querySelector(".item")
来源：http://fy.chemitech.net.cn

[U101] JS：classList 操作
来源：http://as.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://da.szsharing.cn

[U102] JS：本地存储
来源：http://eh.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xs.huanxung.cn

[U103] JS：定时器
来源：http://kl.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rq.521024.cn

[U104] JS：防抖
来源：http://va.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nw.9csxet.cn

[U105] JS：节流
来源：http://va.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vv.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://qz.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sy.szsharing.cn

[U107] JS：数字千分位
来源：http://ws.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nu.nicolike.cn

[U108] JS：随机整数
来源：http://md.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rt.shtwfgs.cn

[U109] JS：数组分组
来源：http://ak.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://ji.chemitech.net.cn

[U110] JS：数组分块
来源：http://hu.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cv.shxzukj.cn

[U111] JS：对象转 Map
来源：http://xp.szxytkj.cn

new Map(Object.entries(obj))
来源：http://go.bjjhwx.cn

[U112] JS：字符串补位
来源：http://px.chemitech.net.cn

"7".padStart(3, "0")
来源：http://ws.asd995.cn

[U113] JS：正则替换全部
来源：http://tp.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://al.nicolike.cn

[U114] JS：JSON 深比较
来源：http://ui.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hu.9csxet.cn

[U115] JS：生成 UUID
来源：http://di.shxzukj.cn

crypto.randomUUID()
来源：http://bn.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://zs.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://fi.chemitech.net.cn

[U117] JS：单元测试
来源：http://hg.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://xz.muxihuayi.cn

[U118] JS：开发服务器
来源：http://yd.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://tr.yuexingan06.cn

[U119] JS：生产构建
来源：http://wm.lnxyls.cn

npx vite build
来源：http://em.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ym.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://dh.chemitech.net.cn

================================================================================
来源：http://xh.muxihuayi.cn

统计汇总
来源：http://mk.shxzukj.cn

================================================================================
来源：http://kr.521024.cn

按语言统计（条）：
来源：http://ih.szsharing.cn

Python ......... 252
来源：http://sv.nicolike.cn

PHP ............ 252
来源：http://vv.huixiangedu.cn

JavaScript ..... 252
来源：http://ax.jctech888.com.cn

TypeScript ..... 212
来源：http://kf.jctech888.com.cn

Java ........... 212
来源：http://zp.hahajie.cn

Go ............. 212
来源：http://bw.huixinmuqiang.cn

Ruby ........... 212
来源：http://wk.huixiangedu.cn

C# ............. 212
来源：http://qc.yuntaijiaju.cn

C .............. 30
来源：http://yx.huanxung.cn

C++ ............ 30
来源：http://ss.jianghongdianzi.cn

SQL ............ 90
来源：http://nv.panjiajie.cn

Bash ........... 80
来源：http://sz.colortex.cn

Kotlin ......... 15
来源：http://aj.hnjuh.cn

Swift .......... 15
来源：http://zi.nszjky.cn

Lua ............ 10
来源：http://hr.huixinmuqiang.cn

Perl ........... 10
来源：http://se.huanxung.cn

Scala .......... 10
来源：http://zv.huixiangedu.cn

------------------------------------
来源：http://qw.yuexingan06.cn

合计 ........... 2106 条
来源：http://yh.shxzukj.cn

按章节统计：
来源：http://mw.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tf.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zp.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oi.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ze.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yn.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ov.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zc.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ut.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vo.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oi.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fb.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pv.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pm.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fb.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wr.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ks.chemitech.net.cn

Q SQL 专题                              90
来源：http://ab.huixinmuqiang.cn

R Bash 专题                             80
来源：http://sl.lnxyls.cn

S C / C++ 专题                          60
来源：http://hz.lnxyls.cn

T 其他语言补充                          60
来源：http://us.huanxung.cn

U 高频实用片段                         120
来源：http://sj.yuntaijiaju.cn

------------------------------------
来源：http://js.huanxung.cn

合计                                  2106 条
来源：http://ll.asd995.cn

--------------------------------------------------------------------------------
来源：http://bw.hahajie.cn

使用提醒
来源：http://qy.huanxung.cn

--------------------------------------------------------------------------------
来源：http://sl.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lp.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mw.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yu.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xb.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ao.nicolike.cn

—— 文件结束 ——
来源：http://uw.bjjhwx.cn


<!-- 参考信息 -->