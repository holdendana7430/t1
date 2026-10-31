代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://sg.jctech888.com.cn

[T51] Scala：Hello World
来源：http://md.9csxet.cn

println("Hello")
来源：http://io.chemitech.net.cn

[T52] Scala：变量
来源：http://vp.szsharing.cn

val a = 1;  var b = 2
来源：http://lb.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://kd.521024.cn

s"值: $b"
来源：http://dn.haigaiapp.cn

[T54] Scala：集合映射
来源：http://fh.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://lq.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://uv.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://so.hahajie.cn

[T56] Scala：样例类
来源：http://ap.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://xg.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://jm.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cg.yuexingan06.cn

[T58] Scala：函数定义
来源：http://yn.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://td.bookmarksfly.cn

[T59] Scala：循环
来源：http://ex.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://kp.nicolike.cn

[T60] Scala：折叠
来源：http://io.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dw.muxihuayi.cn

================================================================================
来源：http://gr.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vo.nszjky.cn

================================================================================
来源：http://ei.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://qe.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aq.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://nd.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ud.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://cf.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nv.hahajie.cn

[U04] Py：变量调试打印
来源：http://yb.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zl.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://rc.hahajie.cn

list(dict.fromkeys(arr))
来源：http://ew.asd995.cn

[U06] Py：合并两个字典
来源：http://eh.shxzukj.cn

{**a, **b}
来源：http://bp.panjiajie.cn

[U07] Py：反转字典键值
来源：http://it.nszjky.cn

{v: k for k, v in d.items()}
来源：http://fn.asd995.cn

[U08] Py：展平二维列表
来源：http://fl.bjjhwx.cn

[y for x in nested for y in x]
来源：http://xp.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://ni.jctech888.com.cn

max(d, key=d.get)
来源：http://sk.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://zf.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cp.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://do.hnjuh.cn

(x * 2 for x in arr)
来源：http://wj.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lg.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://on.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://xt.muxihuayi.cn

deque(maxlen=10)
来源：http://oe.huanxung.cn

[U14] Py：分组收集到列表
来源：http://pl.shxzskj.cn

defaultdict(list)
来源：http://ic.lnxyls.cn

[U15] Py：高精度计时
来源：http://qx.jctech888.com.cn

t = time.perf_counter()
来源：http://zs.asd995.cn

[U16] Py：命令行参数解析
来源：http://aj.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mx.yuexingan06.cn

[U17] Py：初始化日志
来源：http://iz.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://qw.szxytkj.cn

[U18] Py：预编译正则
来源：http://sv.szsharing.cn

pat = re.compile(r"\d+")
来源：http://dv.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://ys.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ad.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://aa.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://dt.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://nj.panjiajie.cn

@contextlib.contextmanager
来源：http://lu.asd995.cn

[U22] Py：矩阵转置
来源：http://iq.panjiajie.cn

list(zip(*m))
来源：http://vs.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://js.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gc.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://ik.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://il.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://bi.shtwfgs.cn

csv.DictReader(f)
来源：http://id.shtwfgs.cn

[U26] Py：并发下载
来源：http://mz.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cb.newstarts.cn

[U27] Py：异步 HTTP
来源：http://pp.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://dh.shtwfgs.cn

[U28] Py：类型别名
来源：http://zq.shxzskj.cn

UserId = int
来源：http://ed.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://nw.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://du.9csxet.cn

[U30] Py：数据类
来源：http://fm.shtwfgs.cn

@dataclass(slots=True)
来源：http://fd.jctech888.com.cn

[U31] Py：单测
来源：http://ac.9csxet.cn

python -m pytest -q
来源：http://fc.nicolike.cn

[U32] Py：代码格式化
来源：http://kj.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://ra.shtwfgs.cn

[U33] Py：打包发布
来源：http://zf.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://kg.muxihuayi.cn

[U34] Py：判断编码
来源：http://jb.huanxung.cn

chardet.detect(raw)
来源：http://db.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://qc.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yz.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://my.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://xf.gzmigu.cn

[U37] Py：读写 Excel
来源：http://lc.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rl.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://fj.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://bd.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://xq.szsharing.cn

sys.stdout.isatty()
来源：http://mf.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://kq.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://ko.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://ev.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rx.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://iu.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uk.huanxung.cn

[U43] PHP：声明命名空间
来源：http://hg.shxzukj.cn

namespace App\Http;
来源：http://ii.nicolike.cn

[U44] PHP：开启严格类型
来源：http://hl.szxytkj.cn

declare(strict_types=1);
来源：http://bq.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://ra.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://hq.gzmigu.cn

?string $name = null
来源：http://lo.shxzskj.cn

[U47] PHP：联合类型
来源：http://wh.szsharing.cn

int|string $id
来源：http://ub.panjiajie.cn

[U48] PHP：纯枚举
来源：http://ep.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gt.chemitech.net.cn

[U49] PHP：只读属性
来源：http://eb.bookmarksfly.cn

public readonly string $name
来源：http://bu.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://pr.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://di.huixiangedu.cn

[U51] PHP：数组解构
来源：http://gs.colortex.cn

[$a, $b] = $arr;
来源：http://lb.huanxung.cn

[U52] PHP：箭头函数
来源：http://dn.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://fj.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://cr.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://gh.nicolike.cn

[U54] PHP：空安全调用
来源：http://js.jctech888.com.cn

$obj?->method()
来源：http://ct.szxytkj.cn

[U55] PHP：match 表达式
来源：http://jo.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ue.shxzskj.cn

[U56] PHP：命名参数
来源：http://ek.bjjhwx.cn

f(a: 1, b: 2)
来源：http://mv.huanxung.cn

[U57] PHP：字符串插值
来源：http://lq.muxihuayi.cn

"值: {$a}"
来源：http://wl.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://fr.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zp.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://qe.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sc.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://sh.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mg.521024.cn

[U61] PHP：正则
来源：http://gz.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ms.lnxyls.cn

[U62] PHP：日期对象
来源：http://yn.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gf.521024.cn

[U63] PHP：文件读写
来源：http://gm.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ku.panjiajie.cn

[U64] PHP：目录遍历
来源：http://wz.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://ch.muxihuayi.cn

[U65] PHP：会话
来源：http://mw.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ny.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://jr.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pk.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://le.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nq.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://ah.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ep.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://rw.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hp.szsharing.cn

[U70] PHP：PDO 事务
来源：http://ph.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lf.shxzskj.cn

[U71] PHP：抛出异常
来源：http://tn.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://zj.newstarts.cn

[U72] PHP：写错误日志
来源：http://fg.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://zy.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://kd.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://tm.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://iz.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://nq.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://me.bjjhwx.cn

composer require psr/container
来源：http://py.muxihuayi.cn

[U76] PHP：简单路由
来源：http://ei.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sb.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://gp.chemitech.net.cn

composer require twig/twig
来源：http://sa.shxzskj.cn

[U78] PHP：单元测试
来源：http://jw.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://ud.9csxet.cn

[U79] PHP：静态分析
来源：http://bk.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://bo.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://bq.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://px.nszjky.cn

[U81] JS：初始化项目
来源：http://mq.bookmarksfly.cn

npm init -y;  npm i express
来源：http://ba.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://ue.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://is.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://ax.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xj.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://im.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ia.newstarts.cn

[U85] JS：可选链
来源：http://hp.huixiangedu.cn

a?.b?.c
来源：http://gp.nszjky.cn

[U86] JS：空值合并
来源：http://jn.521024.cn

a ?? b
来源：http://dl.szsharing.cn

[U87] JS：解构默认值
来源：http://qd.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://zr.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://ie.lnxyls.cn

{ ...a, ...b }
来源：http://qg.newstarts.cn

[U89] JS：数组去重
来源：http://po.lnxyls.cn

[...new Set(arr)]
来源：http://ik.szxytkj.cn

[U90] JS：数字数组排序
来源：http://gf.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://om.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://vg.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ng.shtwfgs.cn

[U92] JS：深拷贝
来源：http://no.newstarts.cn

structuredClone(obj)
来源：http://ok.521024.cn

[U93] JS：模板字符串
来源：http://tr.bookmarksfly.cn

`共 ${n} 条`
来源：http://ef.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://dp.huanxung.cn

const double = x => x * 2;
来源：http://ci.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://rc.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://gp.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://jl.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jw.chemitech.net.cn

[U97] JS：并发请求
来源：http://ua.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ku.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://gc.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://py.newstarts.cn

[U99] JS：事件监听
来源：http://ip.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://bg.shxzskj.cn

[U100] JS：DOM 查询
来源：http://yu.yuexingan06.cn

document.querySelector(".item")
来源：http://lt.yuexingan06.cn

[U101] JS：classList 操作
来源：http://rf.yuexingan06.cn

el.classList.toggle("active")
来源：http://ga.shxzukj.cn

[U102] JS：本地存储
来源：http://vu.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cr.521024.cn

[U103] JS：定时器
来源：http://kt.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ev.hnjuh.cn

[U104] JS：防抖
来源：http://yr.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hq.yuntaijiaju.cn

[U105] JS：节流
来源：http://kn.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hi.panjiajie.cn

[U106] JS：日期格式化
来源：http://de.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jc.colortex.cn

[U107] JS：数字千分位
来源：http://zj.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ig.muxihuayi.cn

[U108] JS：随机整数
来源：http://mt.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zc.shxzukj.cn

[U109] JS：数组分组
来源：http://uk.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://ou.wgjwhj.cn

[U110] JS：数组分块
来源：http://kf.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qh.nszjky.cn

[U111] JS：对象转 Map
来源：http://gc.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://ny.gzmigu.cn

[U112] JS：字符串补位
来源：http://yz.nszjky.cn

"7".padStart(3, "0")
来源：http://yq.521024.cn

[U113] JS：正则替换全部
来源：http://ic.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://wt.asd995.cn

[U114] JS：JSON 深比较
来源：http://rw.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ag.szsharing.cn

[U115] JS：生成 UUID
来源：http://ch.chemitech.net.cn

crypto.randomUUID()
来源：http://rk.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://mi.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://sf.szxytkj.cn

[U117] JS：单元测试
来源：http://fc.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://ob.muxihuayi.cn

[U118] JS：开发服务器
来源：http://av.huanxung.cn

npm i -D vite;  npx vite
来源：http://vl.szxytkj.cn

[U119] JS：生产构建
来源：http://tr.bjjhwx.cn

npx vite build
来源：http://cr.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://vt.asd995.cn

import.meta.env.VITE_API_URL
来源：http://hb.panjiajie.cn

================================================================================
来源：http://vw.chemitech.net.cn

统计汇总
来源：http://pu.wgjwhj.cn

================================================================================
来源：http://oj.newstarts.cn

按语言统计（条）：
来源：http://qf.yuntaijiaju.cn

Python ......... 252
来源：http://tt.gzmigu.cn

PHP ............ 252
来源：http://ld.jctech888.com.cn

JavaScript ..... 252
来源：http://em.jctech888.com.cn

TypeScript ..... 212
来源：http://rz.9csxet.cn

Java ........... 212
来源：http://lw.jctech888.com.cn

Go ............. 212
来源：http://bb.haigaiapp.cn

Ruby ........... 212
来源：http://ez.szsharing.cn

C# ............. 212
来源：http://wt.9csxet.cn

C .............. 30
来源：http://hc.shtwfgs.cn

C++ ............ 30
来源：http://we.bjjhwx.cn

SQL ............ 90
来源：http://gj.huixiangedu.cn

Bash ........... 80
来源：http://dv.shxzskj.cn

Kotlin ......... 15
来源：http://yt.gzmigu.cn

Swift .......... 15
来源：http://df.jctech888.com.cn

Lua ............ 10
来源：http://oa.muxihuayi.cn

Perl ........... 10
来源：http://wq.shxzskj.cn

Scala .......... 10
来源：http://pr.colortex.cn

------------------------------------
来源：http://xr.muxihuayi.cn

合计 ........... 2106 条
来源：http://ag.shtwfgs.cn

按章节统计：
来源：http://nu.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vc.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gc.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://en.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://db.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vi.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ik.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vu.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iq.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sh.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dn.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zi.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://or.jianghongdianzi.cn


<!-- 参考信息 -->