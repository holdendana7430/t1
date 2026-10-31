代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://mn.shxzskj.cn

[T51] Scala：Hello World
来源：http://xr.jianghongdianzi.cn

println("Hello")
来源：http://gs.chemitech.net.cn

[T52] Scala：变量
来源：http://jg.shxzukj.cn

val a = 1;  var b = 2
来源：http://jg.colortex.cn

[T53] Scala：字符串插值
来源：http://mm.huixinmuqiang.cn

s"值: $b"
来源：http://hx.haigaiapp.cn

[T54] Scala：集合映射
来源：http://at.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://kj.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://mm.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hq.wgjwhj.cn

[T56] Scala：样例类
来源：http://qy.shxzukj.cn

case class User(name: String, age: Int)
来源：http://dr.huanxung.cn

[T57] Scala：模式匹配
来源：http://tv.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dv.yuexingan06.cn

[T58] Scala：函数定义
来源：http://gv.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ak.jctech888.com.cn

[T59] Scala：循环
来源：http://er.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://iw.9csxet.cn

[T60] Scala：折叠
来源：http://tw.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qy.9csxet.cn

================================================================================
来源：http://rc.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sq.wgjwhj.cn

================================================================================
来源：http://sh.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://st.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pr.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://af.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jv.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://me.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cg.szsharing.cn

[U04] Py：变量调试打印
来源：http://zz.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lz.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://yp.nszjky.cn

list(dict.fromkeys(arr))
来源：http://pk.nszjky.cn

[U06] Py：合并两个字典
来源：http://vd.shtwfgs.cn

{**a, **b}
来源：http://bc.szxytkj.cn

[U07] Py：反转字典键值
来源：http://yj.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://xe.nicolike.cn

[U08] Py：展平二维列表
来源：http://sd.colortex.cn

[y for x in nested for y in x]
来源：http://ia.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://qf.wgjwhj.cn

max(d, key=d.get)
来源：http://vq.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://tn.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uw.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://mz.wgjwhj.cn

(x * 2 for x in arr)
来源：http://kh.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gx.colortex.cn

Counter(arr).most_common(3)
来源：http://ad.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://fj.bookmarksfly.cn

deque(maxlen=10)
来源：http://gk.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://kz.bookmarksfly.cn

defaultdict(list)
来源：http://sg.szsharing.cn

[U15] Py：高精度计时
来源：http://gz.newstarts.cn

t = time.perf_counter()
来源：http://dw.asd995.cn

[U16] Py：命令行参数解析
来源：http://nd.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ye.hahajie.cn

[U17] Py：初始化日志
来源：http://kx.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://zd.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://sl.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://cr.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://ez.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jx.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://xf.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://jz.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://dr.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://wb.nszjky.cn

[U22] Py：矩阵转置
来源：http://gi.panjiajie.cn

list(zip(*m))
来源：http://es.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://ej.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ac.nicolike.cn

[U24] Py：路径操作
来源：http://rc.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zn.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://el.huanxung.cn

csv.DictReader(f)
来源：http://az.lnxyls.cn

[U26] Py：并发下载
来源：http://uc.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hy.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://ar.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://aw.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://od.9csxet.cn

UserId = int
来源：http://wl.muxihuayi.cn

[U29] Py：属性校验
来源：http://zb.hahajie.cn

@property 与 @x.setter 配合
来源：http://vu.haigaiapp.cn

[U30] Py：数据类
来源：http://ar.jctech888.com.cn

@dataclass(slots=True)
来源：http://zf.bjjhwx.cn

[U31] Py：单测
来源：http://ax.newstarts.cn

python -m pytest -q
来源：http://gr.colortex.cn

[U32] Py：代码格式化
来源：http://sv.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://ur.chemitech.net.cn

[U33] Py：打包发布
来源：http://ye.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://xn.chemitech.net.cn

[U34] Py：判断编码
来源：http://ea.chemitech.net.cn

chardet.detect(raw)
来源：http://ao.haigaiapp.cn

[U35] Py：发送邮件
来源：http://wm.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://av.huanxung.cn

[U36] Py：定时任务
来源：http://sc.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://ei.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://ao.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ga.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://qw.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://xg.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://ry.haigaiapp.cn

sys.stdout.isatty()
来源：http://ag.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://jc.nicolike.cn

print("err", file=sys.stderr)
来源：http://sv.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://fd.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bn.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://vg.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qc.nszjky.cn

[U43] PHP：声明命名空间
来源：http://qk.shxzskj.cn

namespace App\Http;
来源：http://pj.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://ck.lnxyls.cn

declare(strict_types=1);
来源：http://xv.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://vw.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fr.shxzskj.cn

[U46] PHP：可空类型
来源：http://ef.muxihuayi.cn

?string $name = null
来源：http://xu.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://bg.gzmigu.cn

int|string $id
来源：http://wf.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://ni.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://av.yuexingan06.cn

[U49] PHP：只读属性
来源：http://ai.szsharing.cn

public readonly string $name
来源：http://wp.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://ax.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://cd.hahajie.cn

[U51] PHP：数组解构
来源：http://du.nicolike.cn

[$a, $b] = $arr;
来源：http://gj.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://ep.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://bp.newstarts.cn

[U53] PHP：空合并运算符
来源：http://cf.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ce.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://gy.yuexingan06.cn

$obj?->method()
来源：http://dc.lnxyls.cn

[U55] PHP：match 表达式
来源：http://vr.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://by.lnxyls.cn

[U56] PHP：命名参数
来源：http://jw.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://he.panjiajie.cn

[U57] PHP：字符串插值
来源：http://an.chemitech.net.cn

"值: {$a}"
来源：http://ut.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://rv.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vi.nicolike.cn

[U59] PHP：自定义排序
来源：http://sk.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wo.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://ic.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vo.newstarts.cn

[U61] PHP：正则
来源：http://qy.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yc.shxzukj.cn

[U62] PHP：日期对象
来源：http://cf.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jq.lnxyls.cn

[U63] PHP：文件读写
来源：http://ow.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gq.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://pm.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://hb.bjjhwx.cn

[U65] PHP：会话
来源：http://oy.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ab.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://la.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rx.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://vm.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sr.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://qu.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wi.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://ov.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sn.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://rk.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://af.colortex.cn

[U71] PHP：抛出异常
来源：http://ia.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://og.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://qo.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://ah.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://qo.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://ir.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://ko.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://dq.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://sx.muxihuayi.cn

composer require psr/container
来源：http://kp.hahajie.cn

[U76] PHP：简单路由
来源：http://ry.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rw.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://oc.nszjky.cn

composer require twig/twig
来源：http://yb.panjiajie.cn

[U78] PHP：单元测试
来源：http://gs.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://ul.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://zu.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://ur.521024.cn

[U80] PHP：代码规范修复
来源：http://xk.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xs.panjiajie.cn

[U81] JS：初始化项目
来源：http://no.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://tc.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://ks.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ji.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://oq.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sp.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://kp.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hk.yuntaijiaju.cn

[U85] JS：可选链
来源：http://kj.muxihuayi.cn

a?.b?.c
来源：http://pi.nszjky.cn

[U86] JS：空值合并
来源：http://cr.asd995.cn

a ?? b
来源：http://nj.haigaiapp.cn

[U87] JS：解构默认值
来源：http://tn.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://xa.hnjuh.cn

[U88] JS：对象展开合并
来源：http://vx.wgjwhj.cn

{ ...a, ...b }
来源：http://va.panjiajie.cn

[U89] JS：数组去重
来源：http://ju.haigaiapp.cn

[...new Set(arr)]
来源：http://ml.newstarts.cn

[U90] JS：数字数组排序
来源：http://ec.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://bp.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://qf.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ok.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://ws.jctech888.com.cn

structuredClone(obj)
来源：http://nt.shtwfgs.cn

[U93] JS：模板字符串
来源：http://ek.gzmigu.cn

`共 ${n} 条`
来源：http://ej.yuexingan06.cn

[U94] JS：箭头函数
来源：http://nl.colortex.cn

const double = x => x * 2;
来源：http://hk.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://rq.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://jh.nszjky.cn

[U96] JS：async/await 与异常
来源：http://xv.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lw.shxzukj.cn

[U97] JS：并发请求
来源：http://qo.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wf.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://mc.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nz.huanxung.cn

[U99] JS：事件监听
来源：http://uu.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://cb.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://bl.hahajie.cn

document.querySelector(".item")
来源：http://jg.lnxyls.cn

[U101] JS：classList 操作
来源：http://xr.521024.cn

el.classList.toggle("active")
来源：http://yp.shxzukj.cn

[U102] JS：本地存储
来源：http://yj.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://iw.panjiajie.cn

[U103] JS：定时器
来源：http://dk.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mm.szsharing.cn

[U104] JS：防抖
来源：http://mt.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fo.huixinmuqiang.cn

[U105] JS：节流
来源：http://jf.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xl.521024.cn

[U106] JS：日期格式化
来源：http://gq.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://co.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://zv.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rm.szxytkj.cn

[U108] JS：随机整数
来源：http://ir.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://av.hahajie.cn

[U109] JS：数组分组
来源：http://dw.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://hc.wgjwhj.cn

[U110] JS：数组分块
来源：http://sb.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xz.shxzskj.cn

[U111] JS：对象转 Map
来源：http://hm.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://qg.huixiangedu.cn

[U112] JS：字符串补位
来源：http://rv.shxzskj.cn

"7".padStart(3, "0")
来源：http://av.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://xr.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://vt.521024.cn

[U114] JS：JSON 深比较
来源：http://em.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://me.szxytkj.cn

[U115] JS：生成 UUID
来源：http://jf.jctech888.com.cn

crypto.randomUUID()
来源：http://ab.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://se.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://eg.yuexingan06.cn

[U117] JS：单元测试
来源：http://pi.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://nm.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://uu.nicolike.cn

npm i -D vite;  npx vite
来源：http://sy.jctech888.com.cn

[U119] JS：生产构建
来源：http://vu.szxytkj.cn

npx vite build
来源：http://xo.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://fx.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://jp.haigaiapp.cn

================================================================================
来源：http://ih.wgjwhj.cn

统计汇总
来源：http://ev.newstarts.cn

================================================================================
来源：http://vp.gzmigu.cn

按语言统计（条）：
来源：http://bh.nicolike.cn

Python ......... 252
来源：http://fb.gzmigu.cn

PHP ............ 252
来源：http://mo.nicolike.cn

JavaScript ..... 252
来源：http://va.asd995.cn

TypeScript ..... 212
来源：http://uk.chemitech.net.cn

Java ........... 212
来源：http://lx.bjjhwx.cn

Go ............. 212
来源：http://fp.nszjky.cn

Ruby ........... 212
来源：http://si.nicolike.cn

C# ............. 212
来源：http://kl.nszjky.cn

C .............. 30
来源：http://ct.521024.cn

C++ ............ 30
来源：http://xk.shxzskj.cn

SQL ............ 90
来源：http://ns.szxytkj.cn

Bash ........... 80
来源：http://yo.huixinmuqiang.cn

Kotlin ......... 15
来源：http://nk.9csxet.cn

Swift .......... 15
来源：http://fd.shtwfgs.cn

Lua ............ 10
来源：http://ym.shtwfgs.cn

Perl ........... 10
来源：http://sz.gzmigu.cn

Scala .......... 10
来源：http://tq.shxzskj.cn

------------------------------------
来源：http://ts.shxzukj.cn

合计 ........... 2106 条
来源：http://pq.yuexingan06.cn

按章节统计：
来源：http://fg.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ac.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fu.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qa.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ex.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fm.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dt.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lg.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://co.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xt.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zd.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rk.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ac.yuntaijiaju.cn


<!-- 参考信息 -->