代发 wailian999

[T49] Perl：函数
来源：http://dy.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gc.newstarts.cn

[T50] Perl：逐行读文件
来源：http://bn.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uo.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://me.szsharing.cn

[T51] Scala：Hello World
来源：http://bg.hnjuh.cn

println("Hello")
来源：http://hn.chemitech.net.cn

[T52] Scala：变量
来源：http://ts.szxytkj.cn

val a = 1;  var b = 2
来源：http://ek.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://pa.bookmarksfly.cn

s"值: $b"
来源：http://mf.huixiangedu.cn

[T54] Scala：集合映射
来源：http://bw.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://qq.asd995.cn

[T55] Scala：集合过滤
来源：http://ym.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zf.asd995.cn

[T56] Scala：样例类
来源：http://rh.huanxung.cn

case class User(name: String, age: Int)
来源：http://gc.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://iw.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zw.gzmigu.cn

[T58] Scala：函数定义
来源：http://dx.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bd.wgjwhj.cn

[T59] Scala：循环
来源：http://iw.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://lj.shtwfgs.cn

[T60] Scala：折叠
来源：http://pt.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ve.nszjky.cn

================================================================================
来源：http://rc.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hu.shxzukj.cn

================================================================================
来源：http://ge.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://px.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zt.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://ro.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xw.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://jx.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jm.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://oy.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nr.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://sw.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://xv.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://ft.huixinmuqiang.cn

{**a, **b}
来源：http://km.huanxung.cn

[U07] Py：反转字典键值
来源：http://io.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://dw.szsharing.cn

[U08] Py：展平二维列表
来源：http://wp.hahajie.cn

[y for x in nested for y in x]
来源：http://rv.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://hh.huixiangedu.cn

max(d, key=d.get)
来源：http://ey.9csxet.cn

[U10] Py：按值排序字典
来源：http://gn.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hj.hnjuh.cn

[U11] Py：生成器表达式
来源：http://ei.szxytkj.cn

(x * 2 for x in arr)
来源：http://zf.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://go.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://zr.panjiajie.cn

[U13] Py：固定长度队列
来源：http://rw.jianghongdianzi.cn

deque(maxlen=10)
来源：http://fr.asd995.cn

[U14] Py：分组收集到列表
来源：http://nl.newstarts.cn

defaultdict(list)
来源：http://xp.jctech888.com.cn

[U15] Py：高精度计时
来源：http://gt.hnjuh.cn

t = time.perf_counter()
来源：http://cd.newstarts.cn

[U16] Py：命令行参数解析
来源：http://ur.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oi.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://qo.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://qg.hahajie.cn

[U18] Py：预编译正则
来源：http://or.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://qh.szsharing.cn

[U19] Py：正则替换带回调
来源：http://qu.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mq.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://fn.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://hs.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://zz.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://hq.huanxung.cn

[U22] Py：矩阵转置
来源：http://kz.nicolike.cn

list(zip(*m))
来源：http://el.asd995.cn

[U23] Py：分块读取大文件
来源：http://qr.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yd.nszjky.cn

[U24] Py：路径操作
来源：http://yw.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zp.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://pi.haigaiapp.cn

csv.DictReader(f)
来源：http://xa.muxihuayi.cn

[U26] Py：并发下载
来源：http://ow.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qy.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://yf.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://ns.newstarts.cn

[U28] Py：类型别名
来源：http://uy.hahajie.cn

UserId = int
来源：http://oi.newstarts.cn

[U29] Py：属性校验
来源：http://kt.panjiajie.cn

@property 与 @x.setter 配合
来源：http://xy.hahajie.cn

[U30] Py：数据类
来源：http://kw.wgjwhj.cn

@dataclass(slots=True)
来源：http://cb.shxzukj.cn

[U31] Py：单测
来源：http://ze.asd995.cn

python -m pytest -q
来源：http://gj.521024.cn

[U32] Py：代码格式化
来源：http://nj.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://ks.huanxung.cn

[U33] Py：打包发布
来源：http://tv.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://ox.shxzukj.cn

[U34] Py：判断编码
来源：http://bo.huixinmuqiang.cn

chardet.detect(raw)
来源：http://hl.lnxyls.cn

[U35] Py：发送邮件
来源：http://fc.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vu.huanxung.cn

[U36] Py：定时任务
来源：http://gi.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://ob.hnjuh.cn

[U37] Py：读写 Excel
来源：http://bx.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eh.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://nb.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://zz.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://am.jctech888.com.cn

sys.stdout.isatty()
来源：http://rq.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://od.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://nv.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://cd.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dp.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://zv.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qx.9csxet.cn

[U43] PHP：声明命名空间
来源：http://td.9csxet.cn

namespace App\Http;
来源：http://kb.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://cb.jianghongdianzi.cn

declare(strict_types=1);
来源：http://ur.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://wr.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qh.muxihuayi.cn

[U46] PHP：可空类型
来源：http://at.521024.cn

?string $name = null
来源：http://aa.521024.cn

[U47] PHP：联合类型
来源：http://lh.gzmigu.cn

int|string $id
来源：http://fv.asd995.cn

[U48] PHP：纯枚举
来源：http://vs.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mo.bjjhwx.cn

[U49] PHP：只读属性
来源：http://ol.szxytkj.cn

public readonly string $name
来源：http://aq.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://wl.szxytkj.cn

public function __construct(private int $id) {}
来源：http://au.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://qm.huixiangedu.cn

[$a, $b] = $arr;
来源：http://jt.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://or.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://bw.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://qx.521024.cn

$v = $a ?? $b ?? "default";
来源：http://cb.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://fa.chemitech.net.cn

$obj?->method()
来源：http://ob.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://vj.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lf.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://ek.gzmigu.cn

f(a: 1, b: 2)
来源：http://qo.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://xl.shtwfgs.cn

"值: {$a}"
来源：http://ds.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://ho.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://li.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://lj.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bp.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://hg.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://di.yuexingan06.cn

[U61] PHP：正则
来源：http://mz.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mq.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://hi.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jp.lnxyls.cn

[U63] PHP：文件读写
来源：http://fv.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://of.shxzukj.cn

[U64] PHP：目录遍历
来源：http://sd.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ew.huanxung.cn

[U65] PHP：会话
来源：http://oq.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wp.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://vn.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ky.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://ei.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uo.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://wy.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pw.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://dx.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vq.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://qf.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yv.shxzskj.cn

[U71] PHP：抛出异常
来源：http://uw.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://qc.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://jl.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://nc.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://qt.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://xb.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://np.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://zt.521024.cn

[U75] PHP：依赖注入
来源：http://jd.huixiangedu.cn

composer require psr/container
来源：http://ue.wgjwhj.cn

[U76] PHP：简单路由
来源：http://sp.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ij.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://zi.shxzukj.cn

composer require twig/twig
来源：http://pr.521024.cn

[U78] PHP：单元测试
来源：http://cz.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://oo.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://pm.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://dq.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://kz.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pe.shxzskj.cn

[U81] JS：初始化项目
来源：http://fe.bookmarksfly.cn

npm init -y;  npm i express
来源：http://ft.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://dm.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://td.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://rf.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sa.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://ep.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ti.szxytkj.cn

[U85] JS：可选链
来源：http://oc.yuntaijiaju.cn

a?.b?.c
来源：http://ik.newstarts.cn

[U86] JS：空值合并
来源：http://jv.wgjwhj.cn

a ?? b
来源：http://vu.asd995.cn

[U87] JS：解构默认值
来源：http://vb.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://dv.colortex.cn

[U88] JS：对象展开合并
来源：http://wv.lnxyls.cn

{ ...a, ...b }
来源：http://qv.huanxung.cn

[U89] JS：数组去重
来源：http://mh.hnjuh.cn

[...new Set(arr)]
来源：http://ja.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://nq.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://sy.nicolike.cn

[U91] JS：对象键值遍历
来源：http://ds.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ag.gzmigu.cn

[U92] JS：深拷贝
来源：http://pe.muxihuayi.cn

structuredClone(obj)
来源：http://cx.shxzskj.cn

[U93] JS：模板字符串
来源：http://vy.9csxet.cn

`共 ${n} 条`
来源：http://km.shtwfgs.cn

[U94] JS：箭头函数
来源：http://ui.huixinmuqiang.cn

const double = x => x * 2;
来源：http://um.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://sp.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://ri.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://lr.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gb.gzmigu.cn

[U97] JS：并发请求
来源：http://lz.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sk.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://dg.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wu.huixiangedu.cn

[U99] JS：事件监听
来源：http://zv.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://tc.huanxung.cn

[U100] JS：DOM 查询
来源：http://cp.szxytkj.cn

document.querySelector(".item")
来源：http://lc.lnxyls.cn

[U101] JS：classList 操作
来源：http://hg.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://oa.jctech888.com.cn

[U102] JS：本地存储
来源：http://rn.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bn.huixiangedu.cn

[U103] JS：定时器
来源：http://ao.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bd.colortex.cn

[U104] JS：防抖
来源：http://ps.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rm.bookmarksfly.cn

[U105] JS：节流
来源：http://yx.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hl.szsharing.cn

[U106] JS：日期格式化
来源：http://bl.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oa.muxihuayi.cn

[U107] JS：数字千分位
来源：http://wy.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dq.hnjuh.cn

[U108] JS：随机整数
来源：http://yb.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ai.yuexingan06.cn

[U109] JS：数组分组
来源：http://nu.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://pm.nszjky.cn

[U110] JS：数组分块
来源：http://qr.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ad.newstarts.cn

[U111] JS：对象转 Map
来源：http://ra.panjiajie.cn

new Map(Object.entries(obj))
来源：http://lo.jctech888.com.cn

[U112] JS：字符串补位
来源：http://kn.huanxung.cn

"7".padStart(3, "0")
来源：http://zk.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://ew.shxzskj.cn

s.replaceAll("a", "b")
来源：http://zz.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://cs.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dg.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://qp.shxzskj.cn

crypto.randomUUID()
来源：http://yr.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://co.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://iv.hahajie.cn

[U117] JS：单元测试
来源：http://zm.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://hg.huanxung.cn

[U118] JS：开发服务器
来源：http://rf.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://nt.shtwfgs.cn

[U119] JS：生产构建
来源：http://mu.panjiajie.cn

npx vite build
来源：http://gz.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ky.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://we.muxihuayi.cn

================================================================================
来源：http://nl.szsharing.cn

统计汇总
来源：http://hp.shtwfgs.cn

================================================================================
来源：http://xl.colortex.cn

按语言统计（条）：
来源：http://lu.yuexingan06.cn

Python ......... 252
来源：http://bj.newstarts.cn

PHP ............ 252
来源：http://cw.asd995.cn

JavaScript ..... 252
来源：http://uf.newstarts.cn

TypeScript ..... 212
来源：http://xy.huixiangedu.cn

Java ........... 212
来源：http://fx.chemitech.net.cn

Go ............. 212
来源：http://sl.shtwfgs.cn

Ruby ........... 212
来源：http://oy.nicolike.cn

C# ............. 212
来源：http://uc.shxzukj.cn

C .............. 30
来源：http://ne.nszjky.cn

C++ ............ 30
来源：http://np.bookmarksfly.cn

SQL ............ 90
来源：http://dy.huanxung.cn

Bash ........... 80
来源：http://fx.szxytkj.cn

Kotlin ......... 15
来源：http://uh.shxzskj.cn

Swift .......... 15
来源：http://ay.nszjky.cn

Lua ............ 10
来源：http://qj.hahajie.cn

Perl ........... 10
来源：http://cz.gzmigu.cn

Scala .......... 10
来源：http://nk.wgjwhj.cn

------------------------------------
来源：http://cc.panjiajie.cn

合计 ........... 2106 条
来源：http://jy.chemitech.net.cn

按章节统计：
来源：http://pb.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cy.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iy.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zi.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rs.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fn.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dx.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vk.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dr.yuexingan06.cn


<!-- 参考信息 -->